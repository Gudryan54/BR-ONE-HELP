Depósito Fechado
~~~~~~~~~~~~~~~~~~~~

O processo de Faturamento de Depósito Fechado exige a configuração do processo de **Transferencia entre filiais.**

**Faturamento em Depósito Fechado**

Para acessar a tela de Faturamento de Depósito Fechado, basta acessar o menu:

**Vendas C/R** -> **Faturamento em depósito fechado**
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img1.png
   :scale: 80%

Após seleção a tela **BR One :: Faturamento em deposito fechado** será apresentada.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img2.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img3.png
   :scale: 80%

A tela possui os seguintes campos de filtro:
 
**Cliente:** Apresentará todos os Parceiros de Negócios cadastrados como cliente no sistema.

**Ponto de Entrega:** Apresentrá os pontos de entrega do cadastrado do cliente, somente permitirá ser preenchido o campo, caso o campo cliente esteja com filtro.

**Filial:** Apresentará todas as Filiais ativas cadastradas no sistema para seleção.

**Processo:** Apresentará os processos que fazem parte do Faturamento de deposito fechado, sendo eles:

-  **Pedido de Venda**

-  **NF de entrega futura**

-  **Esboço de NF de Saída**

-  **Esboço de NF de Faturamento**

-  **Pedido de Transferência**

**Data de entrega:** Apresentará o calendário para realizar o filtro por Data De/Até.

**Nº Documento:** Apresentará o número dos documentos conforme selecionados no campo Processo para realizar o filtro De/Até.

**N° do item:** Apresentará os itens cadastrados para realizar filto De/Até.

A tela possui os seguintes campos na grid:
 
-  **Selecionado**:  Campo do tipo checkbox utilizado para seleção da linha e processamento.

-  **Nº do documento:** Apresenta o número do documento selecionado previamente no campo processo do cabeçalho.

-  **Código do item**: Apresenta os códigos dos itens no documento selecionado previamente no campo processo do cabeçalho.

-  **Descrição do Item:** Apresenta a descrição dos itens no documento selecionado previamente no campo processo do cabeçalho.

-  **Depósito:** Apresenta o deposito dos itens no documento selecionado previamente no campo processo do cabeçalho.

-  **Quantidade:** Apresenta a quantidade dos itens no documento selecionado previamente no campo processo do cabeçalho. O valor do campo quantidade pode ser alterado.

-  **Cliente:** Apresenta o código do cliente no documento selecionado previamente no campo processo do cabeçalho ou no campo cliente.

-  **Data de Entrega:** Apresenta a data de entrega no documento selecionado previamente no campo processo do cabeçalho.

A tela possui os seguintes botões:
 
-  **Filtrar:** O botão aciona a consulta com base nos parametros escolhidos pelo usuário para apresentação em tela.

-  **Cancelar:** O botão tem ação de finalizar a tela.

-  **Processar:** O botão possui a ação de processar os documentos selecionados na grid.

**Processo do Faturamento em Deposito Fechado**
 
O processo de Faturamento em Deposito Fechado é utilizado para faturar um determinado produto na Filial A, porém este é produzido pela Filial B.
 
Para o início do processo devemos ter Pedidos de Vendas ou NF de Entrega Futuras inseridos no sistema.
 
Para filtrar os Pedido de Vendas ou NF de Entrega Futuras não há necessidade de preenchermos o campo Cliente, apenas se for necessário Pedidos de Vendas ou NF de Entragas Futuras de um cliente especifico.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img4.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img5.png
   :scale: 80%

Utilizando Pedido de Vendas no processo, selecionamos o Pedido de Venda e Item desejado, marcando o checkbox do campo selecionado.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img6.png
   :scale: 80%

Ao clicarmos no botão Processar, será aberto a tela BR One:: Seleção da filial de transferência para seleção da Filial será feita a transferencia.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img7.png
   :scale: 80%

Caso não selecionarmos nenhuma linha, a mensagem de alerta no rodapé será apresentada ‘Erro pois nenhuma linha foi selecionada’.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img8.png
   :scale: 80%

Caso selecionarmos a mesma filial do cabeçalho, neste exemplo SBO\_BROne será apresentada a mensagem ‘A filial da transferência não pode ser nula ou igual a filial dos documentos selecionados’.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img9.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img10.png
   :scale: 80%

Selecionando a filial desejada e clicando em OK, a tela do Pedido de Transferência de Estoque será aberto.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img11.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img12.png
   :scale: 80%

Podemos utilizar o botão Copiar para e assim efetivarmos o Pedido de Transferencia de Estoque para uma Trasnferencia de Estoque.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img13.png
   :scale: 80%

Podemos também utilizar a opção Pedido de Transferencia no cabeçalho da tela de Faturamento de Deposito Fechado.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img14.png
   :scale: 80%

Após selecionarmos as linhas dos pedidos desejados e selecionar o botão processar, os pedidos de transferencia de estoque serão transformados em Transferencia de Estoque e o Esboço de Nota Fiscal de Saída será apresentado em tela.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img15.png
   :scale: 80%

O esboço de Nota Fiscal de Saída pode ser adicionado já quando for aberto na tela ou localizado através do filtro na tela de Faturamento Deposito Fechado.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img16.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img16_1.png
   :scale: 80%

Após adicionarmos o Esboço da Nota Fiscal de Saída o mesmo se tornará uma Nota Fiscal de Saída e será aberto automaticamente em tela o Esboço de Nota Fiscal de Entrada para a filial SBO\_BROne.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img17.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img17_1.png
   :scale: 80%

Ao adicionarmos o Esboço de Nota Fiscal de Entrada o mesmo se tornará uma Nota Fiscal de Entrada e será aberto automaticamente um Esboço de Nota Fiscal de Saída para a filial SBO\_BROne.

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img18.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img18_1.png
   :scale: 80%

Podemos localizar também este documento na tela de Faturamento em Deposito Fechado através do filtro de cabeçalho Esboço de NF de Faturamento.
 
.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img19.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img19_1.png
   :scale: 80%

Ao adicionarmos o Esboço da Nota Fiscal de Saída o mesmo se tronará uma Nota Fiscal de Saída para a filial SBO\_BROne finalizando assim o processo de Faturamento em Deposito Fechado.

.. image:: /_static/BR\ One\ Produção/Processo/DepositoFechado/img20.png
   :scale: 80%

