Entrada de produção
^^^^^^^^^^^^^^^^^^^

.. |image-link| image:: WMS-AcessandoMenuEntradaPA.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AcessandoMenuEntradaPA.gif" style="width: 300px;" />
   </div>

| \

Acessando o menu Entrada de produção, todos os documentos de Ordem de produção gerados no SAP, que tenham o status **Liberada**, serão exibidos no aplicativo.

| \

.. |image-link2| image:: WMS-AberturadeDocumento.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AberturadeDocumento.gif" style="width: 300px;" />
   </div>

| \

Abra o documento escolhendo manualmente, digitando o código do documento ou realizando a leitura via código de barras.

| \

.. |image-link3| image:: WMS-PreenchimentoEntradadePA.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-PreenchimentoEntradadePA.gif" style="width: 300px;" />
   </div>

| \

Para concluir com a Entrada de produto acabado, preencha o lote/série e a quantidade do item. Opcionalmente, a data de vencimento pode ser preenchida.

| \

.. important::

   Possuindo licença BR One Produção, no momento de realizar o preenchimento do lote/série, o campo no aplicativo pode estar bloqueado. Isso ocorre porque o comportamento de permitir ou não a alteração do lote/série no momento de realizar a Entrada de produto acabado, segue as **Configurações de Produção - Aba Lote/Série**.

| \

.. |image-link4| image:: WMS-ConclusãoEntradadePA.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-ConclusãoEntradadePA.png" style="width: 300px;" />
   </div>

| \

.. important::

   Para Ordens de produção de itens que geram Subprodutos, durante a entrada de Produto Acabado, também pode ser feita a entrada de Subproduto. 

| \


.. image:: WMS-DocumentoEntradadeMercadorias.png
   :align: center

| \

Uma vez concluída a Entrada de produto acabado, o documento Entrada de mercadorias, será gerado no SAP. Existindo configurações para geração de ficha de análise, aprovação da ficha através de skip lote e/ou beneficiamento de compras, os documentos relacionados a estes processos serão gerados também neste momento.

.. tip::

   Saiba mais sobre a configuração de ficha de análise e processo de aprovação por skip lote, clicando **aqui**. Para conhecer o processo de beneficiamento de compras, clique **aqui**

| \

.. image:: WMS-DocumentoEntradadeMercadorias2.png
   :align: center

| \

Se a base de dados não tiver licença de BR One Produção, o documento gerado após a conclusão da entrada de PA no aplicativo, será o documento Entrada de produto acabado nativo do SAP Business One.