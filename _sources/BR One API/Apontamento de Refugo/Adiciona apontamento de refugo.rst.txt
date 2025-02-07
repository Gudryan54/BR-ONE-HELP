
Adiciona apontamento de refugo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint, possibilita realizar a adição de um apontamento de refugo, para isso, o usuário deve utilizar a requisão POST e enviar o JSON abaixo:

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Refugo/030.png
   :scale: 75%

.. code-block:: json
   :caption: JSON para Adição de Apontamento de Refugo

   {
     "docNumOrdemProducao": 0,
     "dataDocumento": "2024-07-17",
     "quantidade": 0,
     "codigoProjeto": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "classificacaoRefugo": "",
     "idIntegracao": "",
     "lotes": [
       {
         "lote": "",
         "quantidade": 0
       }
     ],
     "series": [
       {
         "numSerie": ""
       }
     ]
   }

Importante ressaltar que para inserir um apontamento de refugo a OP deve possuir status **'Liberado'** e possuir entrada de PA realizada.

Segue abaixo exemplos de adição de apontamento de refugo na API: 

.. code-block:: json
   :caption: PA administrado por Nenhum

   {
     "docNumOrdemProducao": 0,
     "dataDocumento": "2024-07-17",
     "quantidade": 0,
     "codigoProjeto": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "classificacaoRefugo": "",
     "idIntegracao": ""
   }

.. code-block:: json
   :caption: PA administrado por Lote

   {
     "docNumOrdemProducao": 0,
     "dataDocumento": "2024-07-17",
     "quantidade": 0,
     "codigoProjeto": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "classificacaoRefugo": "",
     "idIntegracao": "",
     "lotes": [
       {
         "lote": "",
         "quantidade": 0
       }
     ]
   }

.. code-block:: json
   :caption: PA administrado por Série

   {
     "docNumOrdemProducao": 0,
     "dataDocumento": "2024-07-17",
     "quantidade": 0,
     "codigoProjeto": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "classificacaoRefugo": "",
     "idIntegracao": "",
     "series": [
       {
         "numSerie": ""
       }
     ]
   }

Campos obrigatórios:

- docNumOrdemProducao
- dataDocumento
- quantidade
- classificacaoRefugo
- lote
- numSerie

