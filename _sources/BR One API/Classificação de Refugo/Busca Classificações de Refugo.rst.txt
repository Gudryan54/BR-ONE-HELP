
Busca Classificações de Refugo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

É possível utilizar a API para realizar uma busca das classificações de refugo cadastrados na base. Para realizar a busca, deve-se utilizar o endpoint abaixo e executar o mesmo.

.. image:: /_static/BR\ One\ API/Classificação\ de\ Refugo/092.png
   :scale: 90%
   :align: center

| \

Exemplo de retorno da API, após a execução do endpoint:

.. code-block:: json
   :caption: Retorno da API

   [
     {
       "codigo": "Classificação01",
       "nome": "Classificação01"
     },
     {
       "codigo": "Classificação02",
       "nome": "Classificação02"
     },
     {
       "codigo": "-1",
       "nome": "Sem classificação"
     }
   ]
