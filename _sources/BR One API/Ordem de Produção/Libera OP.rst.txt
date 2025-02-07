Liberar Ordens de Produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint altera o status da ordem de produção para '**Liberado**', para realizar a atualização do status da OP, deve-se informar o campo '**docNumOrdemProducao**' e o JSON '**transferenciaEstoqueLiberacaoOPRetrabalho**' demonstrados abaixo.

.. image:: /_static/BR\ One\ API/OP/058.png
   :scale: 80%

.. code-block:: json
   :caption: Exemplo de estrutura de transferência de estoque para liberação de OP

   {
     "transferenciaEstoqueLiberacaoOPRetrabalho": {
       "doDeposito": "",
       "lotesLiberacaoPA": [
         {
           "lote": "",
           "quantidade": 0
         }
       ]
     }
   }

O campo "**transferenciaEstoqueLiberacaoOPRetrabalho**" é utilizado apenas para a liberação de OPs de Retrabalho, pois ele indica o depósito e o lote utilizado na transferência de estoque gerado na liberação da OP de Retrabalho, com isso para o usuário realizar a liberação deste tipo de OP, ele deve executar a API informando o campo '**docNumOrdemProducao**' e os campos disponíveis do JSON, segue abaixo exemplo: 

.. image:: /_static/BR\ One\ API/OP/060.png
   :scale: 80%

.. code-block:: json
   :caption: Exemplo de estrutura de transferência de estoque para liberação de OP

   {
     "transferenciaEstoqueLiberacaoOPRetrabalho": {
       "doDeposito": "",
       "lotesLiberacaoPA": [
         {
           "lote": "",
           "quantidade": 0
         }
       ],
       "seriesLiberacaoPA": [
         {
           "numeroSistema": 0,
           "serie": "",
           "quantidade": 0
         }
       ]
     }
   }


Para Ordens de Produção do tipo Padrão e de Beneficiamento de Compra não é necessário enviar o campo "**transferenciaEstoqueLiberacaoOPRetrabalho**" preenchido, portanto, para liberar esses tipos de OPs, basta executar a API informando o campo '**docNumOrdemProducao**' e o JSON conforme exemplo abaixo:

.. image:: /_static/BR\ One\ API/OP/062.png
   :scale: 80%

.. code-block:: json
   :caption: Exemplo de estrutura de transferência de estoque para liberação de OP

   {
     "transferenciaEstoqueLiberacaoOPRetrabalho": {}
   }