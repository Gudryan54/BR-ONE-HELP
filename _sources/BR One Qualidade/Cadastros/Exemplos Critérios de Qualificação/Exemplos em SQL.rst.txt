Exemplos em SQL 
~~~~~~~~~~~~~~~~~~~

Importante ressaltar que o **ID** da chamada dos critérios deve corresponder com o cadastro na tela do SAP e que o script deve ser inserido dentro do parâmetro **BEGIN**, que por sua vez é chamado dentro da função criada, conforme exemplificado no tópico **Critérios automáticos**.

Segue abaixo exemplos de critérios automáticos para bancos SQL:

- **Atraso na entrega**

(Quantidade de peças em atraso (Data de lançamento do pedido - Data programada para chegada))/ Quantidade total de peças recebidas no mês

.. code-block:: sql

	IF @id = 1
	BEGIN
		SELECT @valorEncontrado = CASE WHEN COUNT(T0.dias_atraso) > 0 
		THEN  'Sim' ELSE 'Não' END
		
		FROM (
				SELECT  DATEDIFF (day, T3.TaxDate,t1.ShipDate) AS dias_atraso
				FROM ORDR T0
				INNER JOIN RDR1 T1 ON T0.DocEntry = T1.DocEntry
				INNER JOIN PCH1 T2 ON T0.DocEntry = T2.BaseEntry
				INNER JOIN OPCH T3 ON T3.DocEntry = T2.DocEntry
				WHERE T2.BaseType=22 and DATEDIFF (day, T3.TaxDate,t1.ShipDate)  >= 0
				and T3.CreateDate = MONTH(GETDATE())
				and T3.CardCode = @fornecedor
			) T0
	END
	
- **Material avariado maior que 71% do total**

(Quantidade de peças avariadas identificadas no momento da inspeção / Quantidade total de peças recebidas no mês)

.. code-block:: sql
	
	IF @ID = 2
	BEGIN
		SELECT @valorEncontrado = case when count(*) > 0 then  'Sim' else 'Não' end
		FROM (
				SELECT 
				T0.[U_UPItmQty],
				T2.qtd_recebida,
				SUM(T0.[U_UPItmQty]) * 100 / ISNULL(T2.qtd_recebida,1) as 'qtd_reprovada',
				T0.U_UPCrdCod
				FROM [@UPQ_OFCA] T0
				INNER JOIN [@UPQ_FCA1] T1 ON T0.[DocEntry] = T1.[DocEntry]
				INNER JOIN (SELECT SUM(T0.Quantity)as qtd_recebida,
								T0.ItemCode, T1.CardCode
							FROM PCH1 T0
							INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
							WHERE T1.DOCDATE = MONTH(GETDATE())
							GROUP BY T0.ItemCode, T1.CardCode
							) T2 ON T2.CardCode = T0.U_UPCrdCod
				WHERE T1.[U_UPAprovd] = 'N' AND  T1.[U_UPNCnfrm] = 00000002 and T0.CreateDate = MONTH(GETDATE())
				AND T0.U_UPCrdCod = @fornecedor
				GROUP BY T2.qtd_recebida, T0.U_UPCrdCod,T0.[U_UPItmQty]
			) T0
		WHERE T0.qtd_reprovada > 71
	END
	
- **Material incorreto maior que 71% do total**

Quantidade de peças incorretas identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql
	
	IF @id = 3
	BEGIN
		SELECT @valorEncontrado = case when count(*) > 0 then  'Sim' else 'Não' end
		FROM (
				SELECT SUM(T0.[U_UPItmQty]) * 100 / ISNULL(T2.qtd_recebida,1) as qtd_reprovada,
				T0.U_UPCrdCod
				FROM [@UPQ_OFCA] T0
				INNER JOIN [@UPQ_FCA1] T1 ON T0.[DocEntry] = T1.[DocEntry]
				INNER JOIN (SELECT SUM(T0.Quantity)as qtd_recebida,
								T0.ItemCode, T1.CardCode
							FROM PCH1 T0
							INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
							WHERE T1.DOCDATE = MONTH(GETDATE())
							GROUP BY T0.ItemCode, T1.CardCode
							) T2 ON T2.CardCode = T0.U_UPCrdCod
				WHERE T1.[U_UPAprovd] = 'N' AND  T1.[U_UPNCnfrm] = 00000003
				AND T0.U_UPCrdCod = @fornecedor
				GROUP BY T2.qtd_recebida, T0.U_UPCrdCod
			) T0
			WHERE T0.qtd_reprovada > 71
	END
	
- **Quantidade não conforme maior que 71% do total**

Quantidade de peças em quantidade não conforme identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql
	
	IF @id = 4
	BEGIN
		SELECT @valorEncontrado = case when count(*) > 0 then  'Sim' else 'Não' end
		FROM (
				SELECT SUM(T0.[U_UPItmQty]) * 100 / ISNULL(T2.qtd_recebida,1) as qtd_reprovada,
				T0.U_UPCrdCod
				FROM [@UPQ_OFCA] T0
				INNER JOIN [@UPQ_FCA1] T1 ON T0.[DocEntry] = T1.[DocEntry]
				INNER JOIN (SELECT SUM(T0.Quantity)as qtd_recebida,
								T0.ItemCode, T1.CardCode
							FROM PCH1 T0
							INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
							WHERE T1.DOCDATE = MONTH(GETDATE())
							GROUP BY T0.ItemCode, T1.CardCode
							) T2 ON T2.CardCode = T0.U_UPCrdCod
				WHERE T1.[U_UPAprovd] = 'N' AND  T1.[U_UPNCnfrm] = 00000004
				AND T0.U_UPCrdCod = @fornecedor
				GROUP BY T2.qtd_recebida, T0.U_UPCrdCod
			) T0
			WHERE T0.qtd_reprovada > 71
	END
	
- **Dimensional fora do especificado entre 1% e 10% do total**

Quantidade de peças com dimensional fora do especificado identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql
	
	IF @id = 5
	BEGIN
		SELECT @valorEncontrado = case when count(*) > 0 then  'Sim' else 'Não' end
		FROM (
				SELECT SUM(T0.[U_UPItmQty]) * 100 / ISNULL(T2.qtd_recebida,1) as qtd_reprovada,
				T0.U_UPCrdCod
				FROM [@UPQ_OFCA] T0
				INNER JOIN [@UPQ_FCA1] T1 ON T0.[DocEntry] = T1.[DocEntry]
				INNER JOIN (SELECT SUM(T0.Quantity)as qtd_recebida,
								T0.ItemCode, T1.CardCode
							FROM PCH1 T0
							INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
							WHERE T1.DOCDATE = MONTH(GETDATE())
							GROUP BY T0.ItemCode, T1.CardCode
							) T2 ON T2.CardCode = T0.U_UPCrdCod
				WHERE T1.[U_UPAprovd] = 'N' AND  T1.[U_UPNCnfrm] = 00000001
				AND T0.U_UPCrdCod = @fornecedor
				GROUP BY T2.qtd_recebida, T0.U_UPCrdCod
			) T0
			WHERE T0.qtd_reprovada between 1 and 10
	END
	
- **Tratamento superficial fora do especificado entre 11% e 25% do total**

Quantidade de peças com tratamento superficial fora do especificado identificadas no momento da inspeção / Quantidade total de peças recebidas no mês

.. code-block:: sql 
	
	IF @id = 6
	BEGIN
		SELECT @valorEncontrado = case when count(*) > 0 then  'Sim' else 'Não' end
		FROM (
				SELECT SUM(T0.[U_UPItmQty]) * 100 / ISNULL(T2.qtd_recebida,1) as qtd_reprovada,
				T0.U_UPCrdCod
				FROM [@UPQ_OFCA] T0
				INNER JOIN [@UPQ_FCA1] T1 ON T0.[DocEntry] = T1.[DocEntry]
				INNER JOIN (SELECT SUM(T0.Quantity)as qtd_recebida,
								T0.ItemCode, T1.CardCode
							FROM PCH1 T0
							INNER JOIN OPCH T1 ON T0.DOCENTRY = T1.DOCENTRY
							WHERE T1.DOCDATE = MONTH(GETDATE())
							GROUP BY T0.ItemCode, T1.CardCode
							) T2 ON T2.CardCode = T0.U_UPCrdCod
				WHERE T1.[U_UPAprovd] = 'N' AND  T1.[U_UPNCnfrm] = 00000005
				AND T0.U_UPCrdCod = @fornecedor
				GROUP BY T2.qtd_recebida, T0.U_UPCrdCod
			) T0
			WHERE T0.qtd_reprovada between 11 and 25
	END