Pacotes
^^^^^^^^

.. |image-link| image:: WMS-AcessandoMenuPacotes.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AcessandoMenuPacotes.gif" style="width: 300px;" />
   </div>

| \

Acessando o menu Pacotes, serão listados todos os pacotes criados. Selecione o pacote manualmente via tela ou via leitura de código de barras do código do pacote.

| \

.. |image-link2| image:: WMS-PacotesAbrirIndisp.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-PacotesAbrirIndisp.gif" style="width: 300px;" />
   </div>

| \

Selecionando um pacote, serão exibidas duas opções, **Abrir** e **Indisponibilizar**. Escolhendo abrir, serão exibidos os itens do pacote para que sejam realizadas edições. Indisponibilizando, o pacote será fechado e não poderá mais ser utilizado, liberando as quantidades para a criação de um novo pacote.

| \

.. |image-link3| image:: WMS-OpçõesPacotes.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-OpçõesPacotes.gif" style="width: 300px;" />
   </div>

| \

Para criar um novo pacote, é possível através do botão **"+"** localizado no canto inferior direito, selecionar entre **Pacote avulso**, **Pacotes iguais** ou **Pacotes diferentes**

| \

Pacote avulso
--------------

.. |image-link4| image:: WMS-CriandoPacAvulso.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-CriandoPacAvulso.gif" style="width: 300px;" />
   </div>

| \

Na opção Pacote avulso, após concluir a montagem do pacote, será criado apenas um pacote. Na tela inicial, será demonstrada a tela vazia, pois não há itens adicionados até o momento. Clique em **"+"** no canto inferior e selecione o item através da leitura via código de barras ou selecionando manualmente.

Após selecionar o item, serão listados os depósitos/posições para contagem. Selecione o depósito/posição através da leitura via código de barras ou selecionando manualmente.

Nos detalhes do item, informe a quantidade e registe o apontamento. Neste momento, é possível no inferior da tela, definir um item como "Embalagem".

.. hint::

   O item definido como Embalagem, será considerado na sugestão de destino, quando o item possuir no Cadastro do item, o campo Grupo de armazenamento preenchido. Saiba mais sobre sugestão de destino clicando **aqui**.

| \

Pacote iguais
--------------

.. |image-link5| image:: WMS-CriandoPacIguais.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-CriandoPacIguais.gif" style="width: 300px;" />
   </div>

| \

Na opção Pacotes iguais, antes de iniciar a montagem dos pacotes, será necessário informar a quantidade de pacotes a serem criados.

Após informar a quantidade de pacotes a serem criados, o pacote pode ser montado selecionando os itens e definindo as quantidades. No momento de concluir, ocorrerá uma validação, para verificar se existem quantidades disponíveis para a montagem de todos os pacotes.

Neste exemplo, serão criados dois pacotes com os mesmos itens e quantidades.

| \

Pacote diferentes
------------------

.. |image-link6| image:: WMS-CriandoPacDiferentes.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-CriandoPacDiferentes.gif" style="width: 300px;" />
   </div>

| \

Na opção Pacotes diferentes, antes de iniciar a montagem dos pacotes, será necessário informar a quantidade de pacotes a serem criados.

Após informar a quantidade de pacotes a serem criados, o pacote pode ser montado selecionando os itens e definindo as quantidades. Montando o primeiro pacote, após clicar em "Próximo pacote", serão copiados os itens e quantidades para o próximo pacote, permitindo que possam ser realizadas edições.

Neste exemplo, serão criados dois pacotes com os mesmos itens, porém com quantidades diferentes para o item COMP.0004.

| \

Utilizando os pacotes
----------------------

Existem menus do WMS que você pode utilizar os pacotes criados, sendo eles: **Transferir para produção, Fila de separação, Pedir transferência de estoque, Transferir estoque e Contagem de inventário.**

| \

.. |image-link7| image:: WMS-UtilizandoPacote.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-UtilizandoPacote.gif" style="width: 300px;" />
   </div>

| \

No exemplo a cima, é possível visualizar a utilização do pacote nos menus Transferir estoque e Fila de Separação. Ao invés de adicionar o item via leitura de código de barras do código do item, foi realizada a leitura do código do pacote. Quando realizado essa ação, será aberta uma mensagem informando que o código lido é relacionado a um pacote e se deseja inserir.

Para o caso de transferência de estoque, após inserir o pacote, foi definido o depósito/posição de destino. Como se trata de um pacote, após preencher o depósito/posição da primeira linha, as demais linhas já serão preenchidas automaticamente.

No caso da separação, foi realizada apenas a inserção do pacote. Após concluir a separação utilizando o pacote, o pacote será limpado, permitindo que o mesmo código possa ser reutilizado para a montagem de um novo pacote.