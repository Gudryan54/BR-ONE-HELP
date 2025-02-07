Busca de operações que possam receber apontamentos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint realiza a busca das operações de uma ordem de produção que estão disponíveis para receber apontamentos. 

Para realizar a busca o usuário deve informar o “**DocEntry**” da OP desejada, caso a mesma possua operações que possam receber apontamento a API retornará um JSON dizendo qual operação está disponível.

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/015.png
   :scale: 60%
   :align: center

| \

Exemplo de retorno da API, onde é informado os dados da operação:

.. code-block:: json

   [
     {
       "docEntry": 1,
       "codigo": 1,
       "sequencia": 10,
       "nome": "CT01",
       "descricao": "Cortar01",
       "recursos": [
         {
           "codigo": "1",
           "grupo": "1",
           "tipo": "MQ",
           "nome": "Maquina01",
           "descricao": "Maquina01"
         },
         {
           "codigo": "2",
           "grupo": "2",
           "tipo": "MO",
           "nome": "Mão de Obra01",
           "descricao": "Mão de Obra01"
         }
       ]
     }
   ]

