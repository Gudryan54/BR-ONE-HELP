Busca de apontamentos conforme parâmetros especificados
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint, possibilita realizar a busca dos apontamentos utilizando parâmetros como filtros, no caso os campos '**docEntryOrdemProducao**' e '**sequenciaOperacao**' são obrigatórios.

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/017.png
   :scale: 60%
   :align: center

| \

Exemplo de retorno da API ao realizar a busca:

.. code-block:: json

   [
     {
       "sequenciaOperacao": 10,
       "operacao": {
         "tipoOperacao": 0,
         "operacaoExterna": false,
         "operacaoFicticia": false,
         "desconsiderarNoLeadTime": false,
         "codigo": "3",
         "nome": ""
       },
       "operacaoConcluida": false,
       "docEntryOrdemProducao": 977,
       "docNumOrdemProducao": 0,
       "periodo": "43",
       "series": "-1",
       "linhas": [
         {
           "recurso": {
             "descricao": "Maquina01",
             "tipo": 0,
             "codigo": "1",
             "nome": "Maquina01"
           },
           "quantidadeRecurso": 1,
           "idColaborador": 1,
           "dataInicial": "2024-07-23T00:00:00",
           "dataFinal": "2024-07-23T00:00:00",
           "tempoTotal": {
             "ticks": 36000000000,
             "days": 0,
             "hours": 1,
             "milliseconds": 0,
             "minutes": 0,
             "seconds": 0,
             "totalDays": 0.041666666666666664,
             "totalHours": 1,
             "totalMilliseconds": 3600000,
             "totalMinutes": 60,
             "totalSeconds": 3600
           },
           "quantidadeProduzida": 1,
           "statusRecurso": "1",
           "classificacaoRefugo": "-1",
           "quantidadeRefugo": 1,
           "observacao": "PUT API",
           "linhaDocumentoBase": 1,
           "horaInicial": 723,
           "horaFinal": 823,
           "idIntegracao": "",
           "docEntry": 112,
           "lineId": 1,
           "id": "00000000-0000-0000-0000-000000000000",
           "validationResult": {
             "isValid": true,
             "invalid": false,
             "errors": []
           },
           "valido": true,
           "invalido": false
         },
         {
           "recurso": {
             "descricao": "Maquina01",
             "tipo": 0,
             "codigo": "1",
             "nome": "Maquina01"
           },
           "quantidadeRecurso": 1,
           "idColaborador": 1,
           "dataInicial": "2024-07-23T00:00:00",
           "dataFinal": "2024-07-23T00:00:00",
           "tempoTotal": {
             "ticks": 36000000000,
             "days": 0,
             "hours": 1,
             "milliseconds": 0,
             "minutes": 0,
             "seconds": 0,
             "totalDays": 0.041666666666666664,
             "totalHours": 1,
             "totalMilliseconds": 3600000,
             "totalMinutes": 60,
             "totalSeconds": 3600
           },
           "quantidadeProduzida": 1,
           "statusRecurso": "1",
           "classificacaoRefugo": "-1",
           "quantidadeRefugo": 1,
           "observacao": "PUT API",
           "linhaDocumentoBase": 2,
           "horaInicial": 623,
           "horaFinal": 723,
           "idIntegracao": "",
           "docEntry": 112,
           "lineId": 2,
           "id": "00000000-0000-0000-0000-000000000000",
           "validationResult": {
             "isValid": true,
             "invalid": false,
             "errors": []
           },
           "valido": true,
           "invalido": false
         }
       ],
       "docEntry": 112,
       "docNum": 112,
       "dataCriacao": "2024-07-23T13:58:28.1262949-03:00",
       "dataAtualizacao": "2024-07-23T13:58:28.1262967-03:00",
       "id": "00000000-0000-0000-0000-000000000000",
       "validationResult": {
         "isValid": true,
         "invalid": false,
         "errors": []
       },
       "valido": true,
       "invalido": false
     }
   ]
