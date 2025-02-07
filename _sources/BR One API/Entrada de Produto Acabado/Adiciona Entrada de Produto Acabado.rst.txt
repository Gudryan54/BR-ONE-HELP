Adiciona Entrada de Produto Acabado
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

É possível utilizar a API para realizar a entrada de PA, atualmente existe duas versões de URL do endpoint.

.. image:: /_static/BR\ One\ API/Entrada \ de \ PA/034.png
   :scale: 80%
   :align: center

| \

A diferença entre as duas versões está basicamente na forma como a v2 retorna as informações dos documentos gerados no processo de entrada de PA, é indicado utilizar sempre a versão mais atualizada. 

Portanto, para realizar a entrada de PA utilizando a API, o usuário deve utilizar o endpoint de entrada de produto acabado e enviar o JSON abaixo: 

.. code-block:: json
   :caption: Exemplo de JSON para Adição de Entrada de PA

   {
      "usuarioIntegracao": "",
      "idIntegracao": "",
      "docNumOrdemProducao": 0,
      "docEntryOrdemProducao": 0,
      "codigoItem": "",
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 0,
      "codigoProjeto": "",
      "codigoRegraDistribuicao": "",
      "observacoes": "",
      "refugo": false,
      "classificacaoRefugo": "",
      "trocaLoteEntradaRetrabalho": false,
      "trocaSerieEntradaRetrabalho": false,
      "lotes": [
         {
            "lote": "",
            "quantidade": 0,
            "lineNumBase": 0,
            "atributo1": "",
            "atributo2": "",
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01",
            "local": "",
            "detalhes": ""
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "",
            "quantidade": 0,
            "lineNumBase": 0,
            "atributo1": "",
            "atributo2": "",
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01",
            "local": "",
            "detalhes": ""
         }
      ],
      "series": [
         {
            "numSerieLote": "",
            "quantidade": 0,
            "numSerieFabricante": "",
            "numSerie": "",
            "systemSerialNumber": 0,
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01",
            "dataInicioGarantiaFabricante": "2024-11-01",
            "dataFimGarantiaFabricante": "2024-11-01",
            "localizacao": "",
            "detalhes": ""
         }
      ],
      "seriesTransferenciaEstoque": [
         {
            "numSerie": "",
            "quantidade": 0,
            "systemSerialNumber": 0,
            "lineNumBase": 0,
            "numeroSerieFabricante": "",
            "numeroSerieDoLote": "",
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01",
            "local": "",
            "detalhes": ""
         }
      ],
      "subProdutos": [
         {
            "codigoItem": "",
            "codigoDeposito": "",
            "quantidade": 0,
            "lotes": [
               {
                  "lote": "",
                  "quantidade": 0,
                  "lineNumBase": 0,
                  "atributo1": "",
                  "atributo2": "",
                  "dataVencimento": "2024-11-01",
                  "dataFabricacao": "2024-11-01",
                  "dataAdmissao": "2024-11-01",
                  "local": "",
                  "detalhes": ""
               }
            ]
         }
      ]
   }



Segue abaixo exemplo de JSON preenchido e enviado na API para realizar a entrada de PA para uma Ordem de Produção Padrão:

.. code-block:: json
   :caption: Exemplo de JSON para Adição de Entrada de PA com Dados Preenchidos

   {
      "docNumOrdemProducao": 761,
      "dataDocumento": "2023-04-20",
      "codigoDeposito": "01",
      "quantidade": 1,
      "codigoProjeto": "API",
      "observacoes": "Teste API",
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 1
         }
      ],
      "subProdutos": [
         {
            "codigoItem": "Sub-Produto_001",
            "codigoDeposito": "01",
            "quantidade": 1,
            "lotes": []
         }
      ]
   }


- Entrada de PA realizada no add-on:

.. image:: /_static/BR\ One\ API/Entrada \ de \ PA/037.png
   :scale: 70%
   :align: center

| \

Segue abaixo exemplos de JSON preenchido e enviado na API para realizar a entrada de PA para uma Ordem de Produção de Retrabalho:

.. code-block:: json
   :caption: Exemplo de JSON para Entrada de Retrabalho sem Troca de Lote

   {
      "docNumOrdemProducao": 753,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "01-RET",
      "quantidade": 1,
      "trocaLoteEntradaRetrabalho": false,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 1,
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01"
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L01",
            "quantidade": 1,
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01"
         }
      ]
   }

.. code-block:: json
   :caption: Exemplo de JSON para Entrada de Retrabalho com Troca de Lote

   {
      "docNumOrdemProducao": 753,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "01-RET",
      "quantidade": 1,
      "trocaLoteEntradaRetrabalho": true,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 1,
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01"
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L02",
            "quantidade": 1,
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01"
         }
      ]
   }


- Entradas de PA realizada no add-on:

.. image:: /_static/BR\ One\ API/Entrada \ de \ PA/040.png
   :scale: 70%
   :align: center

| \

Segue abaixo exemplos de JSON preenchido e enviado na API para realizar a entrada de PA para uma Ordem de Produção de Beneficiamento de Compra:

.. code-block:: json
   :caption: Exemplo de JSON para Entrada de Produção na OP de Beneficiamento de Compra

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "lotes": [
         {
            "lote": "",
            "quantidade": 1,
            "dataVencimento": "2024-11-01",
            "dataFabricacao": "2024-11-01",
            "dataAdmissao": "2024-11-01"
         }
      ]
   }


**Campos obrigatórios:**

Os campos obrigatórios do JSON para realizar a entrada de PA podem variar conforme o tipo da ordem de produção, método de administração do PA e se a entrada de PA irá gerar a entrada de sub-produto.

Segue abaixo exemplo de JSON enviados (campos obrigatórios) para realizar a entrada de PA conforme a especificidade da ordem de produção.

- OP Padrão, PA administrado por nenhum:

.. code-block:: json

   {
      "docNumOrdemProducao": 1,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1
   }


- OP Padrão com sub-produto e PA administrado por nenhum:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "codigoItem": "",
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "subProdutos": [
         {
            "codigoItem": "",
            "codigoDeposito": "",
            "quantidade": 1
         }
      ]
   }


- OP Padrão, PA administrado por lote:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "lotes": [
         {
            "lote": "",
            "quantidade": 1
         }
      ]
   }


- OP Padrão com sub-produto e PA administrado por lote:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "codigoItem": "",
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "subProdutos": [
         {
            "codigoItem": "",
            "codigoDeposito": "",
            "quantidade": 1,
            "lotes": [
               {
                  "lote": "",
                  "quantidade": 1
               }
            ]
         }
      ]
   }

- OP Padrão, PA administrado por série:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "series": [
         {
            "quantidade": 1,
            "numSerie": ""
         }
      ],
      "seriesTransferenciaEstoque": [
         {
            "numSerie": "",
            "quantidade": 1
         }
      ]
   }


- OP Padrão com sub-produto e PA administrado por série:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "series": [
         {
            "quantidade": 1,
            "numSerie": ""
         }
      ],
      "seriesTransferenciaEstoque": [
         {
            "numSerie": "",
            "quantidade": 1
         }
      ],
      "subProdutos": [
         {
            "codigoItem": "",
            "codigoDeposito": "",
            "quantidade": 1
         }
      ]
   }


- OP de Retrabalho, PA administrado por nenhum:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1
   }


- OP de Retrabalho, PA administrado por lote sem troca de lote na entrada:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "codigoItem": "",
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "trocaLoteEntradaRetrabalho": false,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 1
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L01",
            "quantidade": 1
         }
      ]
   }


- OP de Retrabalho, PA administrado por lote com troca de lote na entrada:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "codigoItem": "",
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "trocaLoteEntradaRetrabalho": true,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 1
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L02",
            "quantidade": 1
         }
      ]
   }

- OP de Retrabalho com desvio configurado, PA administrado por nenhum

.. code-block:: json

   {
      "docNumOrdemProducao": 1,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1
   }

- OP de Retrabalho com desvio configurado, PA administrado por lote

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "trocaLoteEntradaRetrabalho": false,
      "lotesTransferenciaEstoque": [
         {
            "lote": "",
            "quantidade": 1
         }
      ]
   }


- OP de Beneficiamento de Compra, PA administrado por nenhum:

.. code-block:: json

   {
      "docNumOrdemProducao": 1,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1
   }

- OP de Beneficiamento de Compra, PA administrado por lote:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "lotes": [
         {
            "lote": "",
            "quantidade": 1
         }
      ]
   }


- OP de Beneficiamento de Compra, PA administrado por série:

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 1,
      "series": [
         {
            "quantidade": 1,
            "numSerie": ""
         }
      ],
      "seriesTransferenciaEstoque": [
         {
            "numSerie": "",
            "quantidade": 1
         }
      ]
   }



