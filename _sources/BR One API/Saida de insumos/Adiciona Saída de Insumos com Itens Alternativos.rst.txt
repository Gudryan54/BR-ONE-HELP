Adiciona Saída de Insumos com Itens Alternativos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O endpoint de saída de insumos da API também permite a realização da saída de insumos utilizando os itens alternativos, para o correto funcionamento, os itens alternativos devem estar configurados na tela de **'Itens Alternativos'**.

.. image:: /_static/BR\ One\ API/Saida\ de\ Insumos/101.png
   :scale: 90%
   :align: center

| \

Ao configurar o item na tela acima, para realizar a saída de insumos na API, basta preencher normalmente o JSON da saída de insumos, utilizando o código do item alternativo, realizando assim normalmente a saída de insumos. 

Segue abaixo exemplo do processo, na **OP 1056**, há três componentes, onde o componente **'item_nenhum_01'** possui um cadastro de item alternativo para o **'item_nenhum_02'**.

.. image:: /_static/BR\ One\ API/Saida\ de\ Insumos/102.png
   :scale: 80%
   :align: center

| \
   
Na API ao enviar o JSON abaixo, será realizado a saída de insumos para o componente presente na OP, no caso o **‘item_nenhum_01’**.

.. code-block:: json
   :caption: Saída de Insumos para o componente da OP.

   {
     "docNumOrdemProducao": 1056,
     "sequenciaOperacao": 10,
     "codigoProjeto": "",
     "dataDocumento": "2023-09-26",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": false,
     "linhas": [
       {
         "lineId": 3,
         "codigoItem": "item_nenhum_01",
         "codigoDeposito": "01",
         "quantidade": 1,
         "classificacaoRefugo": ""
       }
     ]
   }
   
Para realizar a saída de insumos para os itens alternativos, basta o usuário informar o item cadastrado na tela de ‘Itens alternativos’, neste exemplo, o item alternativo seria o componente **‘item_nenhum_02’**, com isso basta enviar o JSON abaixo na API.

.. code-block:: json
   :caption: Saída de Insumos para o Item Alternativo.

   {
     "docNumOrdemProducao": 1056,
     "sequenciaOperacao": 10,
     "codigoProjeto": "",
     "dataDocumento": "2023-09-26",
     "referencia": "",
     "codigoRegraDistribuicao": "",
     "observacoes": "",
     "refugo": false,
     "linhas": [
       {
         "lineId": 3,
         "codigoItem": "item_nenhum_02",
         "codigoDeposito": "01",
         "quantidade": 1,
         "classificacaoRefugo": ""
       }
     ]
   }

- **Validações do processo**
   
Caso o usuário informe um item alternativo para o componente da OP, mas o mesmo não possua cadastro na tela de **'itens alternativos'**, a API retornará a seguinte mensagem de erro: 

.. image:: /_static/BR\ One\ API/Saida\ de\ Insumos/105.png
   :scale: 70%
   :align: center

| \
   
Caso o usuário informe um item alternativo para o componente da OP, mas esse “item alternativo” não está configurado na tela de ‘itens alternativos’, a API retornará a seguinte mensagem de erro:

.. image:: /_static/BR\ One\ API/Saida\ de\ Insumos/106.png
   :scale: 70%
   :align: center

| \
   
E por fim, caso o usuário tente realizar a saída de insumos utilizando um item alternativo para uma OP que está com o parâmetro **'Permitir edição após liberação'** desmarcado, a API irá retornar a seguinte mensagem de erro:

.. image:: /_static/BR\ One\ API/Saida\ de\ Insumos/107.png
   :scale: 70%
   :align: center

| \