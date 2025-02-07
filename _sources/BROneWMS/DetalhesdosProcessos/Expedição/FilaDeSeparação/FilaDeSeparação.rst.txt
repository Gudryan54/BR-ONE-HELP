Fila de separação
^^^^^^^^^^^^^^^^^^^

.. |image-link| image:: WMS-MenuFilaSeparação.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-MenuFilaSeparação.gif" style="width: 300px;" />
   </div>

| \

Ao acessar o menu Fila de separação, todos os documentos criados no SAP serão listados. Os documentos que serão listados: Pedido de venda, Pedido de devolução de mercadorias e Esboço de Nota Fiscal de Saída.

| \

.. |image-link2| image:: WMS-AcessandoDocFilaSeparação.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AcessandoDocFilaSeparação.gif" style="width: 300px;" />
   </div>

| \

Você pode acessar os documentos listados selecionando manualmente, realizando a leitura via código de barras do número do documento ou utilizando no canto superior direito os filtros de busca.

| \

.. |image-link3| image:: WMS-SeleçãodeitemFilaSeparação.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SeleçãodeitemFilaSeparação.gif" style="width: 300px;" />
   </div>

| \

Após acessar o documento, os itens serão listados. Selecione o item manualmente ou bipando o código do item/código de barras.

| \

.. |image-link4| image:: WMS-SeleçãoloteserieFilaSeparação.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SeleçãoloteserieFilaSeparação.gif" style="width: 300px;" />
   </div>

| \

Na lista de disponibilidade das quantidades do item, selecione o lote/série desejado manualmente, digitando o código do lote/série na barra de pesquisa ou realizando a leitura do código de barras do lote/série. Nos detalhes do item, preencha a quantidade necessária para a separação e registre.

Para itens controlados por lote/série, se escolhido algum lote/série que não siga a ordem de saída definida nas Configurações WMS, será exibida uma mensagem notificando o usuário desse fato.

.. important::

   A ordem de saída dos lotes/séries pode ser definida como FIFO (First in, first out) ou FEFO (First expire, first out), através do parâmetro localizado na aba Expedição das Configurações WMS. Saiba mais sobre este e outros parâmetros que podem ser utilizados nesse processo clicando **aqui**.

| \

.. |image-link5| image:: WMS-DivergênciaFilaSeparação.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-DivergênciaFilaSeparação.gif" style="width: 300px;" />
   </div>

| \

.. |image-link6| image:: WMS-ConclusãoFilaSeparação.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-ConclusãoFilaSeparação.png" style="width: 300px;" />
   </div>

| \

No momento de concluir a separação, possuindo alguma divergência o usuário será alertado. Concluindo a conferência do documento, será gerado no SAP o documento de destino de acordo com o documento de origem:

- Pedido de venda → Entrega ou Nota Fiscal de Saída

- Pedido de devolução de mercadorias → Devolução de mercadorias (Caso o Pedido de devolução de mercadorias possua vínculo com uma Nota Fiscal de Entrada, será gerado Dev.Nota Fiscal de Entrada)

- Esboço de Nota Fiscal de Saída → Nota Fiscal de Saída

.. note::

   Configurações do WMS quando ativas, podem adicionar comportamentos no menu Fila de separação, clique **aqui** e saiba mais sobre as configurações.