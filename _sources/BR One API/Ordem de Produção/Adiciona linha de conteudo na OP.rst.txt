Adiciona uma linha no GRID da Ordem de Produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint permite adicionar uma linha no GRID da Ordem de Produção. É possível adicionar uma Operação, um recurso ou um componente, para realizar a adição a OP deve possuir status “**Planejado**”, para isso deve ser informado os campos e o JSON abaixo:

.. image:: /_static/BR\ One\ API/OP/077.png
   :scale: 90%

.. image:: /_static/BR\ One\ API/OP/078.png
   :scale: 90%

.. code-block:: json
   :caption: Adição de linha

   {
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
             "codigoRecurso": ""
           }
         ]
       }
     ]
   }


Segue abaixo exemplos de adição de linha para uma OP: 

- **Adição de Operação:**

.. image:: /_static/BR\ One\ API/OP/080.png
   :scale: 90%

.. code-block:: json
   :caption: Modelo de Analise
   
   {
     "modeloAnalise": "00000002",
   }
   
**Obs.: Para adição de operação não é necessário enviar nenhum valor no JSON, para isso basta informar { }.**

.. image:: /_static/BR\ One\ API/OP/082.png
   :scale: 80%

- **Adição de Recurso:**

.. image:: /_static/BR\ One\ API/OP/083.png
   :scale: 90%

.. code-block:: json
   :caption: Adição Recurso

   {
     "linhasOperacao": [
       {
         "tipoRecurso": "MQ",
         "codigoRecurso": "GRM",
         "quantidadeBase": 1,
         "tempoFixo": 5,
         "tempoVariavel": 3,
         "recursos": [
           {
             "codigoRecurso": "R-LASER-001"
           }
         ]
       }
     ]
   }


.. image:: /_static/BR\ One\ API/OP/085.png
   :scale: 80%

- **Adição de Componente:**

.. image:: /_static/BR\ One\ API/OP/086.png
   :scale: 90%

.. code-block:: json
   :caption: Adição de Componente

   {
     "linhasOperacao": [
       {
         "tipoRecurso": "CP",
         "codigoRecurso": "item_nenhum_02",
         "quantidadeBase": 1,
         "quantidadeFixa": 5,
         "depositoComponente": "01",
         "metodoBaixa": "M"
       }
     ]
   }


.. image:: /_static/BR\ One\ API/OP/088.png
   :scale: 80%
