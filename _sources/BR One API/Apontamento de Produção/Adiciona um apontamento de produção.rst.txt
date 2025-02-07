Adiciona um apontamento de produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para realizar a adição de um apontamento de produção, o usuário deve utilizar método POST e enviar o JSON abaixo.

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/009.png
   :scale: 100%
   :align: center

| \

.. code-block:: json
   :caption: Exemplo de JSON para Adição de Apontamento de Produção

   {
     "docEntryOrdemProducao": 0,
     "docNumOrdemProducao": 0,
     "sequenciaOperacao": 0,
     "operacaoConcluida": false,
     "linhas": [
       {
         "dataInicial": "2024-07-23",
         "dataFinal": "2024-07-23",
         "horaInicial": "10:23",
         "horaFinal": "10:23",
         "codigoRecurso": "",
         "quantidadeRecurso": 0,
         "tipoRecurso": "",
         "statusRecurso": 0,
         "quantidadeProduzida": 0,
         "quantidadeRefugo": 0,
         "codigoOperador": 0,
         "classificacaoRefugo": "",
         "observacao": "",
         "idIntegracao": "",
         "motivoParada": ""
       }
     ]
   }

Com isso, a API irá adicionar um apontamento conforme os dados preenchidos no JSON enviado.

Segue abaixo exemplo de JSON preenchido e enviado na API:

.. code-block:: json

   {
     "docEntryOrdemProducao": 761,
     "sequenciaOperacao": 10,
     "operacaoConcluida": false,
     "linhas": [
       {
         "dataInicial": "2023-04-19",
         "dataFinal": "2023-04-19",
         "horaInicial": "06:00",
         "horaFinal": "07:00",
         "codigoRecurso": "13",
         "quantidadeRecurso": 1,
         "statusRecurso": 1,
         "quantidadeProduzida": 10,
         "quantidadeRefugo": 1,
         "codigoOperador": 1,
         "classificacaoRefugo": "1",
         "observacao": "Criado na API",
         "idIntegracao": "",
         "motivoParada": ""
       }
     ]
   }


Resultado no BR One:

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/012.png
   :scale: 60%
   :align: center

| \

**Campos obrigatórios:**

- docEntryOrdemProducao
- sequenciaOperacao
- dataInicial
- dataFinal
- horaInicial
- horaFinal
- codigoRecurso
- quantidadeRecurso
- statusRecurso
- quantidadeProduzida
- quantidadeRefugo
- codigoOperador
- classificacaoRefugo