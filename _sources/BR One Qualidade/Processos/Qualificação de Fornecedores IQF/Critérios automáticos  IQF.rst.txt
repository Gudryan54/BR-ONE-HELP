Critérios automáticos – IQF
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para acessar a tela de **Critérios automáticos – IQF**, é necessatio ir ao menu:

**Administração -> Definição -> Qualidade -> Critérios automáticos – IQF**

Nessa tela, é possível cadastrar os critérios automáticos das funções cadastradas no banco manualmente.

.. image:: /_static/BR\ One\ Qualidade/Processo/Qualificação\ de\ fornecedores/Aspose.Words.67881489-10be-41d8-9938-4848d61ce893.007.png
   :scale: 100%

Caso o usuário queira inserir linhas quando a tela estiver no modo atualizar, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Qualidade/Processo/Qualificação\ de\ fornecedores/Aspose.Words.67881489-10be-41d8-9938-4848d61ce893.008.png
   :scale: 100%

*BR One :: O cadastro deve ser atualizado antes de inserir linhas.*

Também é possível remover linhas desde que o critério automático que estiver sendo removido não esteja vinculado a nenhum modelo de qualificação.

Exemplo de criação da function **F\_Br1\_QualifFornec\_CalcValEsp**:

- **SQL**

.. code-block:: sql

	CREATE FUNCTION dbo.F_Br1_QualifFornec_CalcValEsp
	(
		@fornecedor NVARCHAR(500),
		@id INT
	)
	RETURNS NVARCHAR(500) 
	AS 
	BEGIN
		DECLARE @valorEncontrado NVARCHAR(50)

		-- Irá trazer a quantidade de Nota Fiscal de Entrada canceladas
		IF @id = 1
		BEGIN 
			SELECT @valorEncontrado = COUNT(*)
			FROM OPCH
			WHERE CANCELED = 'Y' 
			AND CardCode = @fornecedor
		END

		RETURN @valorEncontrado 
	END

- **HANA**

.. code-block:: sql

	CREATE FUNCTION "F_Br1_QualifFornec_CalcValEsp"
	(
		codigoFornecedor NVARCHAR(20), 
		codigoEspecificacao INT
	)
	RETURNS valorEncontrado NVARCHAR(50) LANGUAGE SQLSCRIPT AS
	BEGIN
		IF codigoEspecificacao = 1 THEN
			-- Irá trazer a quantidade de Nota Fiscal de Entrada canceladas
			SELECT COUNT(*)
			INTO valorEncontrado
			FROM "OPCH"
			WHERE "CANCELED" = 'Y'
			AND "CardCode" = codigoFornecedor;
		END IF;
	END;
