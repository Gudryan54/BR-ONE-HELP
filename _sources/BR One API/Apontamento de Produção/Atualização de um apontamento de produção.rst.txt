Atualização de um apontamento de produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint, possibilita realizar a atualização de um apontamento de produção, onde é informado o campo '**docEntryApontamento**' na URL e o JSON com os campos que deseja alterar.

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/019.png
   :scale: 60%
   :align: center

| \

.. code-block:: json
   :caption: Exemplo de código JSON

   {
     "operacaoConcluida": false,
     "linhas": [
       {
         "lineId": 0,
         "dataInicial": "2024-07-23",
         "dataFinal": "2024-07-23",
         "horaInicial": "10:23",
         "horaFinal": "10:23",
         "codigoRecurso": "",
         "permiteMultiplasOrdemsProducao": false,
         "quantidadeRecurso": 0,
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

Na atualização do apontamento de produção é possível atualizar as informações de uma linha existente, ou então, adicionar uma nova linha no apontamente. 

A atualização ou adição de uma linha, é determinada pelo campo **"lineId"**, sempre que ela for igual a **'0'** a API irá adicionar uma linha nova e para alterar uma linha existente, deve ser informado o valor numérico correspondente a linha desejada.

Exemplo de apontamento de produção antes de ser atualizado: 

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/021.png
   :scale: 60%
   :align: center

| \

Exemplo de JSON preenchido e enviado na API para atualização de uma linha:

.. code-block:: json

   {
     "operacaoConcluida": false,
     "linhas": [
       {
         "lineId": 0,
         "dataInicial": "2023-04-19",
         "dataFinal": "2023-04-19",
         "horaInicial": "06:30",
         "horaFinal": "07:30",
         "codigoRecurso": "13",
         "permiteMultiplasOrdemsProducao": false,
         "quantidadeRecurso": 5,
         "statusRecurso": 1,
         "quantidadeProduzida": 10,
         "quantidadeRefugo": 1,
         "codigoOperador": 1,
         "classificacaoRefugo": "-1",
         "observacao": "Atualização API",
         "idIntegracao": "",
         "motivoParada": ""
       }
     ]
   }

Apontamento de produção após ser atualizado pela API: 

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/023.png
   :scale: 60%
   :align: center

| \

