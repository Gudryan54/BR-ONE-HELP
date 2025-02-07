Saída de insumos
^^^^^^^^^^^^^^^^^^^

.. |image-link| image:: WMS-AcessandoMenuSaídaInsumos.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AcessandoMenuSaídaInsumos.gif" style="width: 300px;" />
   </div>

| \

No menu Saída de insumos, serão listadas todas as OPs que tenham seu status definido como **Liberada**. Acesse a OP escolhendo manualmente, digitando o código do documento ou realizando a leitura via código de barras.

| \

.. |image-link2| image:: WMS-ComponenteManualListado.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-ComponenteManualListado.png" style="width: 300px;" />
   </div>

| \

.. |image-link3| image:: WMS-InserindoComponenteBaixaExplosão.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-InserindoComponenteBaixaExplosão.gif" style="width: 300px;" />
   </div>

| \

Acessando a OP desejada, serão listados todos os componentes que tenham o método de baixa definido como Manual. Sendo necessário realizar a saída de insumos de componentes definidos com o método Baixa por explosão, através do botão **"+"** é possível adicioná-los.

| \

.. warning::

   Caso a base de dados não possua licença BR One Produção, será possível realizar a saída de insumos apenas para itens de baixa Manual.

| \

.. |image-link4| image:: WMS-SelecionandoComponenteLista.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SelecionandoComponenteLista.gif" style="width: 300px;" />
   </div>

| \

Selecione o componente manualmente, digitando o código do item ou realizando a leitura via código de barras do código do item. Na sequência, serão listados todos os lotes/séries e quantidades disponíveis nos depósitos/posições.

| \

.. |image-link5| image:: WMS-SeleçãodeLoteSaídaInsumos.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SeleçãodeLoteSaídaInsumos.gif" style="width: 300px;" />
   </div>

| \

.. |image-link6| image:: WMS-SeleçãodeLoteSaídaInsumos2.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SeleçãodeLoteSaídaInsumos2.gif" style="width: 300px;" />
   </div>

| \

Na lista de disponibilidade das quantidades do item, selecione o lote/série desejado manualmente, digitando o código do lote/série na barra de pesquisa ou realizando a leitura do código de barras do lote/série. Se o lote/série selecionado tiver quantidade disponível em diferentes depósitos/posições, será aberto um modal para que seja informada a localização desejada.

| \

.. |image-link7| image:: WMS-QtqSegueMétododeSaídaInsumos.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-QtqSegueMétododeSaídaInsumos.gif" style="width: 300px;" />
   </div>

| \

.. |image-link8| image:: WMS-QtqNãoSegueMétododeSaídaInsumos.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-QtqNãoSegueMétododeSaídaInsumos.gif" style="width: 300px;" />
   </div>

| \

.. |image-link11| image:: WMS-FlagdeRefugo.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-FlagdeRefugo.gif" style="width: 300px;" />
   </div>

| \

Preencha a quantidade para realizar a saída de insumos e clique em registrar. Para itens controlados por lote/série, se escolhido algum lote/série que não siga a ordem de saída definida nas Configurações WMS, será exibida uma mensagem notificando o usuário desse fato.

Neste momento, o usuário pode marcar a flag de refugo para que o apontamento seja definido como refugo na Saída de insumos.

.. important::

   A ordem de saída dos lotes/séries pode ser definida como FIFO (First in, first out) ou FEFO (First expire, first out), através do parâmetro localizado na aba Expedição das Configurações WMS. Saiba mais sobre este e outros parâmetros que podem ser utilizados nesse processo clicando **aqui**.

| \

.. |image-link9| image:: WMS-SaídadeinsumosPreenchida.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SaídadeinsumosPreenchida.png" style="width: 300px;" />
   </div>

| \

.. |image-link10| image:: WMS-SaídadeinsumosConcluída.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-SaídadeinsumosConcluída.png" style="width: 300px;" />
   </div>

| \

.. image:: WMS-SaídadeMercadoriasGerada.png
   :align: center

| \

.. image:: WMS-SaídaMercadoriasRefugo.png
   :align: center

| \

Finalizando a Saída de insumos, será gerado no SAP o documento Saída de mercadorias, contendo apenas as linhas preenchidas no aplicativo. Todos os apontamentos marcados como refugo no aplicativo, no documento gerado terão a coluna "Refugo" definida como Sim.

| \

.. warning::

   Parâmetros do BR One Produção, localizados na aba Saída de insumos das Configurações de produção, quando ativos, podem realizar validações adicionais no momento da conclusão. Confira o comportamento dos parâmetros clicando **aqui**.

| \

.. image:: WMS-SaídadeInsumos.png
   :align: center

| \

Se a base de dados não tiver licença de BR One Produção, o documento gerado após a conclusão da saída de insumos no aplicativo, será o documento Saída de insumos nativo do SAP Business One.