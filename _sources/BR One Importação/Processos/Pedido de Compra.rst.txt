Pedido de Compra
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O processo de importação se inicia no Pedido de compra. Para empresa habilitada em Multi-filiais, é necessário definir para qual filial o pedido de compra será criado. Após ser criado o documento, o SAP não permite a troca da filial.

.. image:: /_static/BR\ One\ Importação/Processo/Pedido\ de\ Compra/Aspose.Words.537a9195-f192-42fa-b44f-2788973d3b6c.001.jpeg
   :scale: 80%


Todos os pedidos devem ser criados em Moeda Estrangeira tanto para as linhas quanto para o total do documento. Para isso, as taxas de câmbio têm que estar atualizadas.

.. image:: /_static/BR\ One\ Importação/Processo/Pedido\ de\ Compra/Aspose.Words.537a9195-f192-42fa-b44f-2788973d3b6c.002.png
   :scale: 80%


Havendo taxa informada, ao selecionar a moeda, o SAP irá carregar a taxa informada para o pedido de compra.

.. image:: /_static/BR\ One\ Importação/Processo/Pedido\ de\ Compra/Aspose.Words.537a9195-f192-42fa-b44f-2788973d3b6c.003.png
   :scale: 80%


Não será possível adicionar um pedido de compra em que a moeda do cabeçalho seja diferente das moedas das linhas, somente será possível quando o parceiro de negócio for nacional. Caso o parceiro de negócio não seja nacional, ao tentar atualizar ou adicionar o pedido de compra, a seguinte mensagem será exibida.

.. image:: /_static/BR\ One\ Importação/Processo/Pedido\ de\ Compra/Aspose.Words.537a9195-f192-42fa-b44f-2788973d3b6c.004.png
   :scale: 80%


*(-5) BR One :: Não é possível inserir/atualizar pedidos que contenham a moeda do cabeçalho diferente da moeda da linha.*

Após os pedidos de compras serem criados, eles podem ser importados na tela de *Processo de Importação*. Não será possível alterar o código da UM de itens que estejam vinculados em um processo de importação em aberto. Caso isso aconteça, ao tentar atualizar a UM de um item, a seguinte mensagem será exibida.

.. image:: /_static/BR\ One\ Importação/Processo/Pedido\ de\ Compra/Aspose.Words.537a9195-f192-42fa-b44f-2788973d3b6c.005.png
   :scale: 80%


*(-15) BR One :: Não é possível modificar a UM do item quando ele se encontra aberto em um processo de importação. – 2.0.1588*



