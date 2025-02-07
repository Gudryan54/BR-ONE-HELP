Adiciona uma Ordem de Produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint permite realizar a adição de uma ordem de produção, ao executar o JSON abaixo a OP será adicionada conforme dados preenchidos nos campos do JSON, é possível inserir uma OP dos seguintes tipos: 

- OP Padrão (S)
- OP de Retrabalho (R)
- OP de Beneficiamento de Compra (S)

.. image:: /_static/BR\ One\ API/OP/067.png
   :scale: 90%

.. code-block:: json
   :caption: Adicionar OP

   {
     "tipoOrdemProducao": "",
     "codigoItem": "",
     "codigoRoteiro": "",
     "quantidadePlanejada": 0,
     "codigoDeposito": "",
     "calculoManual": true,
     "dataVencimento": "2024-11-14",
     "programacao": "",
     "permitirEdicaoAposLiberacao": true,
     "fichaQualidade": "",
     "destinoQualidade": "",
     "codigoProjeto": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "conteudo": [
       {
         "operacao": "",
         "sequenciaOperacao": 0,
         "modeloAnalise": "",
         "desconsiderarLeadTime": true,
         "dataInicio": "2024-11-14",
         "horaInicio": 0,
         "dataTermino": "2024-11-14",
         "horaTermino": 0,
         "linhasOperacao": [
           {
             "tipoRecurso": "",
             "codigoRecurso": "",
             "quantidadeBase": 0,
             "quantidadeFixa": 0,
             "quantidadePlanejada": 0,
             "tempoFixo": 0,
             "tempoVariavel": 0,
             "tempoPlanejado": 0,
             "dimensao1": 0,
             "dimensao2": 0,
             "depositoComponente": "",
             "metodoBaixa": "",
             "dataInicio": "2024-11-14",
             "horaInicio": 0,
             "dataTermino": "2024-11-14",
             "horaTermino": 0,
             "observacao": "",
             "observacao2": "",
             "percentualPerda": 0,
             "recursos": [
               {
                 "codigoRecurso": "",
                 "utilizado": true
               }
             ]
           }
         ]
       }
     ],
     "subProduto": [
       {
         "codigoItem": "",
         "codigoDeposito": "",
         "percentualCusto": 0,
         "unidadeMedida": ""
       }
     ]
   }




Importante ressaltar que se for informado os campos do array '**conteúdo**', a API não irá utilizar os dados do roteiro para realizar a adição da OP. 

**Exemplos de adição de OPs:**

- **Adição de OP Padrão:**

Adição de OP informando o roteiro do item:

.. code-block:: json
   :caption: Adicionar OP Padrão

   {
     "tipoOrdemProducao": "S",
     "codigoItem": "pa lote",
     "codigoRoteiro": "pa lote-01",
     "quantidadePlanejada": 10,
     "dataVencimento": "2024-11-12"
   }  

Resultado no SAP: 

.. image:: /_static/BR\ One\ API/OP/070.png
   :scale: 90%

Adição de OP informando as linhas dos grids:

.. code-block:: json
   :caption: Exemplo de Atualização de Ordem de Produção

   {
     "tipoOrdemProducao": "S",
     "codigoItem": "pa lote",
     "quantidadePlanejada": 15,
     "codigoDeposito": "01",
     "dataVencimento": "2024-11-14",
     "fichaQualidade": "PA",
     "destinoQualidade": "0000001",
     "conteudo": [
       {
         "operacao": "8",
         "sequenciaOperacao": 10,
         "linhasOperacao": [
           {
             "tipoRecurso": "MQ",
             "codigoRecurso": "GRAPI",
             "quantidadeBase": 1,
             "tempoFixo": 5,
             "tempoVariavel": 2,
             "recursos": [
               {
                 "codigoRecurso": "MAQ01",
                 "utilizado": true
               }
             ]
           },
           {
             "tipoRecurso": "cp",
             "codigoRecurso": "item_nenhum_01",
             "quantidadeBase": 1,
             "quantidadeFixa": 5,
             "depositoComponente": "01",
             "metodoBaixa": "B"
           }
         ]
       }
     ]
   }


Resultado no SAP: 

.. image:: /_static/BR\ One\ API/OP/072.png
   :scale: 90%

- **Adição de OP Retrabalho:**

Adição de OP de Retrabalho informando o roteiro do item:

.. code-block:: json
   :caption: Adicionar OP de Retrabalho

   {
     "tipoOrdemProducao": "R",
     "codigoItem": "pa lote",
     "codigoRoteiro": "pa lote-01",
     "quantidadePlanejada": 10,
     "codigoDeposito": "01-RET",
     "dataVencimento": "2024-11-12"
   }  

Resultado no SAP: 

.. image:: /_static/BR\ One\ API/OP/074.png
   :scale: 90%

3. **Adição de OP de Beneficiamento de Compra:** 

.. code-block:: json
   :caption: Adicionar OP Beneficiamento de Compra

   {
     "tipoOrdemProducao": "S",
     "codigoItem": "SA-mioloBeneficiamento",
     "codigoRoteiro": "SA-mioloBeneficiamento-01",
     "quantidadePlanejada": 10,
     "dataVencimento": "2024-11-12"
   }  

.. image:: /_static/BR\ One\ API/OP/076.png
   :scale: 90%