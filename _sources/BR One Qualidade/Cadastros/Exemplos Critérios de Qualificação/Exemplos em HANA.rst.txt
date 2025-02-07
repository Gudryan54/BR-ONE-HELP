Exemplos em HANA
~~~~~~~~~~~~~~~~~~~~~

Importante ressaltar que o **ID** da chamada dos critérios deve corresponder com o cadastro na tela do SAP e que o script deve ser inserido dentro do parâmetro **BEGIN**, que por sua vez é chamado dentro da função criada, conforme exemplificado no tópico **Critérios automáticos**.

Segue abaixo exemplos de critérios automáticos para bancos HANA:

- **Atraso na entrega**

(Quantidade de peças em atraso (Data de lançamento do pedido - Data programada para chegada))/ Quantidade total de peças recebidas no mês

.. code-block:: sql

	IF :id = 1 THEN
		SELECT
			CASE
				WHEN COUNT("dias_atraso") > 0 THEN 'Sim'
				ELSE 'Não'
			END
		INTO :valorEncontrado
		FROM (
			SELECT
				DAYS_BETWEEN("TaxDate", "ShipDate") AS "dias_atraso"
			FROM
				ORDR T0
				INNER JOIN RDR1 T1 ON T0."DocEntry" = T1."DocEntry"
				INNER JOIN PCH1 T2 ON T0."DocEntry" = T2."BaseEntry"
				INNER JOIN OPCH T3 ON T3."DocEntry" = T2."DocEntry"
			WHERE
				T2."BaseType" = 22
				AND DAYS_BETWEEN(T3."TaxDate", T1."ShipDate") >= 0
				AND EXTRACT(MONTH FROM CURRENT_DATE) = EXTRACT(MONTH FROM T3."CreateDate")
				AND T3."CardCode" = :fornecedor
		) AS T0;
	END IF;
	
- **Material avariado maior que 71% do total**

(Quantidade de peças avariadas identificadas no momento da inspeção / Quantidade total de peças recebidas no mês)

.. code-block:: sql

	IF :ID = 2 THEN
		SELECT
			CASE
				WHEN COUNT(*) > 0 THEN 'Sim'
				ELSE 'Não'
			END
		INTO valorEncontrado
		FROM (
			SELECT
				T0."U_UPItmQty",
				T2."qtd_recebida",
				SUM(T0."U_UPItmQty") * 100 / IFNULL(T2."qtd_recebida", 1) AS "qtd_reprovada",
				T0."U_UPCrdCod"
			FROM
				"@UPQ_OFCA" T0
				INNER JOIN "@UPQ_FCA1" T1 ON T0."DocEntry" = T1."DocEntry"
				INNER JOIN (
					SELECT
						SUM(T0."Quantity") AS "qtd_recebida",
						T0."ItemCode",
						T1."CardCode"
					FROM
						PCH1 T0
						INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
					WHERE
						T1.DOCDATE = MONTH(NOW())
					GROUP BY
						T0."ItemCode", T1."CardCode"
				) AS T2 ON T2."CardCode" = T0."U_UPCrdCod"
			WHERE
				T1."U_UPAprovd" = 'N'
				AND T1."U_UPNCnfrm" = 2
				AND T0."CreateDate" = MONTH(NOW())
				AND T0."U_UPCrdCod" = :fornecedor
			GROUP BY
				T2."qtd_recebida", T0."U_UPCrdCod", T0."U_UPItmQty"
		) AS T0;
	END IF;
	
- **Material incorreto maior que 71% do total**

Quantidade de peças incorretas identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql

	IF :id = 3 THEN
		SELECT
			CASE
				WHEN COUNT(*) > 0 THEN 'Sim'
				ELSE 'Não'
			END
		INTO valorEncontrado
		FROM (
			SELECT
				SUM(T0."U_UPItmQty") * 100 / IFNULL(T2."qtd_recebida", 1) AS "qtd_reprovada",
				T0."U_UPCrdCod"
			FROM
				"@UPQ_OFCA" T0
				INNER JOIN "@UPQ_FCA1" T1 ON T0."DocEntry" = T1."DocEntry"
				INNER JOIN (
					SELECT
						SUM(T0."Quantity") AS "qtd_recebida",
						T0."ItemCode",
						T1."CardCode"
					FROM
						PCH1 T0
						INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
					WHERE
						T1.DOCDATE = MONTH(NOW())
					GROUP BY
						T0."ItemCode", T1."CardCode"
				) AS T2 ON T2."CardCode" = T0."U_UPCrdCod"
			WHERE
				T1."U_UPAprovd" = 'N'
				AND T1."U_UPNCnfrm" = 3
				AND T0."U_UPCrdCod" = :fornecedor
			GROUP BY
				T2."qtd_recebida", T0."U_UPCrdCod"
		) AS T0;
	END IF;
	
- **Quantidade não conforme maior que 71% do total**

Quantidade de peças em quantidade não conforme identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql

	IF :id = 4 THEN
		SELECT
			CASE
				WHEN COUNT(*) > 0 THEN 'Sim'
				ELSE 'Não'
			END
		INTO valorEncontrado
		FROM (
			SELECT
				SUM(T0."U_UPItmQty") * 100 / IFNULL(T2.qtd_recebida, 1) AS "qtd_reprovada",
				T0.U_UPCrdCod
			FROM
				"@UPQ_OFCA" T0
				INNER JOIN "@UPQ_FCA1" T1 ON T0."DocEntry" = T1."DocEntry"
				INNER JOIN (
					SELECT
						SUM(T0.Quantity) AS "qtd_recebida",
						T0.ItemCode,
						T1.CardCode
					FROM
						PCH1 T0
						INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
					WHERE
						T1.DOCDATE = MONTH(NOW())
					GROUP BY
						T0.ItemCode, T1.CardCode
				) AS T2 ON T2.CardCode = T0.U_UPCrdCod
			WHERE
				T1."U_UPAprovd" = 'N'
				AND T1."U_UPNCnfrm" = 4
				AND T0.U_UPCrdCod = :fornecedor
			GROUP BY
				T2.qtd_recebida, T0.U_UPCrdCod
		) AS T0;
	END IF;
	
- **Dimensional fora do especificado entre 1% e 10% do total**

Quantidade de peças com dimensional fora do especificado identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql

	IF :id = 5 THEN
		SELECT
			CASE
				WHEN COUNT(*) > 0 THEN 'Sim'
				ELSE 'Não'
			END INTO valorEncontrado
		FROM (
			SELECT
				SUM(T0."U_UPItmQty") * 100 / IFNULL(T2.qtd_recebida, 1) AS "qtd_reprovada",
				T0.U_UPCrdCod
			FROM
				"@UPQ_OFCA" T0
				INNER JOIN "@UPQ_FCA1" T1 ON T0."DocEntry" = T1."DocEntry"
				INNER JOIN (
					SELECT
						SUM(T0.Quantity) AS "qtd_recebida", T0.ItemCode, T1.CardCode
					FROM
						PCH1 T0
						INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
					WHERE
						T1.DOCDATE = MONTH(NOW())
					GROUP BY
						T0.ItemCode, T1.CardCode
				) AS T2 ON T2.CardCode = T0.U_UPCrdCod
			WHERE
				T1."U_UPAprovd" = 'N'
				AND T1."U_UPNCnfrm" = 1
				AND T0.U_UPCrdCod = :fornecedor
			GROUP BY
				T2.qtd_recebida, T0.U_UPCrdCod
		) AS T0;
	END IF;
	
- **Tratamento superficial fora do especificado entre 11% e 25% do total**

Quantidade de peças com tratamento superficial fora do especificado identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql

	IF :id = 6 THEN
		SELECT
			CASE
				WHEN COUNT(*) > 0 THEN 'Sim'
				ELSE 'Não'
			END INTO valorEncontrado
		FROM (
			SELECT
				SUM(T0."U_UPItmQty") * 100 / IFNULL(T2.qtd_recebida, 1) AS "qtd_reprovada",
				T0.U_UPCrdCod
			FROM
				"@UPQ_OFCA" T0
				INNER JOIN "@UPQ_FCA1" T1 ON T0."DocEntry" = T1."DocEntry"
				INNER JOIN (
					SELECT
						SUM(T0.Quantity) AS "qtd_recebida", T0.ItemCode, T1.CardCode
					FROM
						PCH1 T0
						INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
					WHERE
						T1.DOCDATE = MONTH(NOW())
					GROUP BY
						T0.ItemCode, T1.CardCode
				) AS T2 ON T2.CardCode = T0.U_UPCrdCod
			WHERE
				T1."U_UPAprovd" = 'N'
				AND T1."U_UPNCnfrm" = 5
				AND T0.U_UPCrdCod = :fornecedor
			GROUP BY
				T2.qtd_recebida, T0.U_UPCrdCod
		) AS T0;
	END IF;