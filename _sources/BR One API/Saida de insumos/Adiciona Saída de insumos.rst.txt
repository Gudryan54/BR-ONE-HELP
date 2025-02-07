
Adiciona Saída de Insumos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint, possibilita realizar uma saída de insumos, para isso o usuário deve utilizar a URL e enviar o JSON mostrado abaixo:

.. image:: /_static/BR\ One\ API/Saida\ de\ Insumos/094.png
   :scale: 90%

.. code-block:: json
   :caption: JSON para Adição de Saída de Insumos

   {
     "docNumOrdemProducao": 0,
     "sequenciaOperacao": 0,
     "codigoProjeto": "",
     "dataDocumento": "2024-07-18",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": false,
     "linhas": [
       {
         "lineId": 0,
         "codigoItem": "",
         "codigoDeposito": "",
         "quantidade": 0,
         "classificacaoRefugo": "",
         "lotes": [
           {
             "lote": "",
             "quantidade": 0
           }
         ],
         "series": [
           {
             "serie": "",
             "quantidade": 0
           }
         ]
       }
     ]
   }

Segue abaixo exemplos de adição de saídas de insumos na API: 

.. code-block:: json
   :caption: PA administrado por Nenhum

   {
     "docNumOrdemProducao": 0,
     "sequenciaOperacao": 0,
     "codigoProjeto": "",
     "dataDocumento": "2024-07-18",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": false,
     "linhas": [
       {
         "lineId": 0,
         "codigoItem": "",
         "codigoDeposito": "",
         "quantidade": 0,
         "classificacaoRefugo": ""
       }
     ]
   }

.. code-block:: json
   :caption: PA administrado por Lote

   {
     "docNumOrdemProducao": 0,
     "sequenciaOperacao": 0,
     "codigoProjeto": "",
     "dataDocumento": "2024-07-18",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": false,
     "linhas": [
       {
         "lineId": 0,
         "codigoItem": "",
         "codigoDeposito": "",
         "quantidade": 0,
         "classificacaoRefugo": "",
         "lotes": [
           {
             "lote": "",
             "quantidade": 0
           }
         ]
       }
     ]
   }

.. code-block:: json
   :caption: PA administrado por Série

   {
     "docNumOrdemProducao": 0,
     "sequenciaOperacao": 0,
     "codigoProjeto": "",
     "dataDocumento": "2024-07-18",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": false,
     "linhas": [
       {
         "lineId": 0,
         "codigoItem": "",
         "codigoDeposito": "",
         "quantidade": 0,
         "classificacaoRefugo": "",
         "series": [
           {
             "serie": "",
             "quantidade": 0
           }
         ]
       }
     ]
   }

É possível também realizar a saída de insumos com o flag refugo marcado, para isso, o campo '**refugo**' deve ser verdadeiro e o campo '**classificacaoRefugo**' informado:

.. code-block:: json
   :caption: Saída de insumos do tipo refugo

   {
     "docNumOrdemProducao": 0,
     "sequenciaOperacao": 0,
     "codigoProjeto": "",
     "dataDocumento": "2024-07-18",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": true,
     "linhas": [
       {
         "lineId": 0,
         "codigoItem": "",
         "codigoDeposito": "",
         "quantidade": 0,
         "classificacaoRefugo": "-1"
       }
     ]
   }


**Campos obrigatórios:**

- "docNumOrdemProducao"
- "sequenciaOperacao"
- "dataDocumento"
- "lineId"
- "codigoItem"
- "codigoDeposito"
- "quantidade"




