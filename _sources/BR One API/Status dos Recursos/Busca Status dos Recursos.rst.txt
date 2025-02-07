
Busca Status dos Recursos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

É possível utilizar a API para realizar uma busca dos status dos recursos cadastrados na base. Para realizar a busca, deve-se utilizar o endpoint abaixo e executar o mesmo.

.. image:: /_static/BR\ One\ API/Status\ dos\ Recursos/090.png
   :scale: 90%
   :align: center

| \

Exemplo de retorno da API, após a execução do endpoint:

.. code-block:: json
   :caption: Retorno da API

   [
     {
       "codigo": "1",
       "nome": "PRD - Produção"
     },
     {
       "codigo": "2",
       "nome": "FDT - Fora de turno"
     },
     {
       "codigo": "3",
       "nome": "AOP - Aguardando OP"
     },
     {
       "codigo": "4",
       "nome": "SET - Setup"
     },
     {
       "codigo": "5",
       "nome": "STR01 - STR01"
     }
   ]










