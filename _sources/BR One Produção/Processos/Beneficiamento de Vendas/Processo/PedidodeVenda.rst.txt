Pedidos de Venda
~~~~~~~~~~~~~~~~~~

O cliente a ser utilizado no pedido de venda é o cliente solicitante do beneficiamento, onde todas as configurações de tipo de documento e depósitos já estão previamente configuradas. 

O item a ser utilizado será o item beneficiado, que contém a estrutura de produção, e que também será utilizado como item pai na ordem de produção.

Todas as linhas devem possuir a mesma utilização **Venda industrialização encomenda** ou **Venda industrialização triangular**, caso alguma linha seja definida com uma utilização do beneficiamento, as demais linhas precisam ter a mesma utilização, caso contrário o pedido não será adicionado.

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Vendas/1.png

Quando a utilização do beneficiamento é selecionada em um pedido de venda, o depósito da linha precisa ser o depósito de **Benef. Vendas** vinculado ao cadastro do cliente. Caso o deposito seja diferente, ao tentar adicionar o pedido o sistema automaticamente trocará para o depósito de **Benef. Vendas** conforme a simulação a seguir.

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Vendas/GIF01.gif

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Vendas/2.png
