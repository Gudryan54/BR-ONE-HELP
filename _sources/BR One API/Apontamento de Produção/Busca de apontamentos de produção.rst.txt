
Busca de apontamentos de produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Ao utilizar a URL abaixo e informar os dados conforme solicitado.

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/007.png
   :scale: 75%
   :align: center

| \

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/008.png
   :scale: 75%
   :align: center

| \

O endpoint **GET** acima irá buscar todos os apontamentos existentes na base, ao informar o campo **'pagina'** definimos quantas páginas serão retornadas na API após a busca, já o campo **'quantidade'** indica quantos apontamentos serão exibidos por página.

.. code-block:: json
   :caption: Exemplo retorno da API

   [
     {
       "sequenciaOperacao": 10,
       "operacao": {
         "tipoOperacao": 0,
         "operacaoExterna": false,
         "operacaoFicticia": false,
         "desconsiderarNoLeadTime": false,
         "codigo": "2",
         "nome": ""
       },
       "operacaoConcluida": false,
       "docEntryOrdemProducao": 3,
       "docNumOrdemProducao": 0,
       "periodo": "8",
       "series": "-1",
       "linhas": [
         {
           "recurso": {
             "tipo": 0,
             "codigo": "1"
           },
           "quantidadeRecurso": 1,
           "idColaborador": 1,
           "dataInicial": "2021-08-17T00:00:00",
           "dataFinal": "2021-08-17T00:00:00",
           "tempoTotal": {
             "ticks": 90000000000,
             "days": 0,
             "hours": 2,
             "milliseconds": 0,
             "minutes": 30,
             "seconds": 0,
             "totalDays": 0.10416666666666667,
             "totalHours": 2.5,
             "totalMilliseconds": 9000000,
             "totalMinutes": 150,
             "totalSeconds": 9000
           },
           "quantidadeProduzida": 100,
           "statusRecurso": "1",
           "classificacaoRefugo": "-1",
           "quantidadeRefugo": 0,
           "linhaDocumentoBase": 1,
           "horaInicial": 700,
           "horaFinal": 930,
           "docEntry": 1,
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
             "tipo": 0,
             "codigo": "2"
           },
           "quantidadeRecurso": 1,
           "idColaborador": 1,
           "dataInicial": "2021-08-17T00:00:00",
           "dataFinal": "2021-08-17T00:00:00",
           "tempoTotal": {
             "ticks": 126000000000,
             "days": 0,
             "hours": 3,
             "milliseconds": 0,
             "minutes": 30,
             "seconds": 0,
             "totalDays": 0.14583333333333334,
             "totalHours": 3.5,
             "totalMilliseconds": 12600000,
             "totalMinutes": 210,
             "totalSeconds": 12600
           },
           "quantidadeProduzida": 100,
           "statusRecurso": "1",
           "classificacaoRefugo": "-1",
           "quantidadeRefugo": 0,
           "linhaDocumentoBase": 2,
           "horaInicial": 600,
           "horaFinal": 930,
           "docEntry": 1,
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
       "docEntry": 1,
       "docNum": 1,
       "dataCriacao": "2024-07-23T10:38:38.5452985-03:00",
       "dataAtualizacao": "2024-07-23T10:38:38.5453939-03:00",
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
