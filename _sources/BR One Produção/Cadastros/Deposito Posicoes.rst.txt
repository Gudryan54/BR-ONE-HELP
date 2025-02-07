Depósitos - Ativar posições
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para utilizarmos as posições de depósito é necessário que a configuração **Ativar posições no depósito** para o depósito desejado esteja ativa.

.. image:: /_static/BR\ One\ Produção/Cadastros/Deposito\ Posicoes/Aspose.Words.e9aa17dc-4d36-4969-96c7-3b70e2bbfbfe.002.png
   :scale: 80%

**Utilizando Posições no Depósito**

Com a opção **Ativar Posições no Depósito** ativa, será apresentado a aba **Posições no depósito** na tela.

.. image:: /_static/BR\ One\ Produção/Cadastros/Deposito\ Posicoes/Aspose.Words.e9aa17dc-4d36-4969-96c7-3b70e2bbfbfe.003.png
   :scale: 80%

Nesta tela será apresentada as posições de depósito configuradas no sistema. 

Conforme o padrão SAP temos a posição 01-SYSTEM-BIN-LOCATION criada automaticamente pela SAP quando ativamos a configuração de posição por depósito.

.. image:: /_static/BR\ One\ Produção/Cadastros/Deposito\ Posicoes/Aspose.Words.e9aa17dc-4d36-4969-96c7-3b70e2bbfbfe.004.png
   :scale: 80%
 
Porém, quando utilizamos o addon BROne e posições do depósito ativa, temos a opção **Considerar posição padrão no depósito (BR One).**
 
Com a opção ativa é necessário configurarmos uma posição para o depósito BR One diferente da configurada para o Padrão SAP.
 
.. image:: /_static/BR\ One\ Produção/Cadastros/Deposito\ Posicoes/Aspose.Words.e9aa17dc-4d36-4969-96c7-3b70e2bbfbfe.005.png
   :scale: 80%

Após configurarmos esta posição para BR One, as operações serão realizadas verificando primeiramente a posição configurada no addon e posteriormente a posição configurada no SAP.

Todo documento que gera uma transação de estoque e envolve um depósito de posição, requer alocação de itens para receber ou dar saída de posições nos depósitos específicos.

Os documentos de Entrada de Mercadoria, Saída de Mercadoria, Recebimento de Mercadoria, Transferência de Estoque, Picking e Entrega solicitarão uma alocação no depósito. 
