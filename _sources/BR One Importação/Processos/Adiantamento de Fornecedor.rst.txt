Adiantamento de Fornecedor
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O adiantamento para fornecedor não é um processo obrigatório, e irá servir para gerar um Lançamento Contábil, realizando o controle do pagamento do fornecedor.

Antes de criar o adiantamento, é necessário inserir os itens do pedido de compra. 

Todo adiantamento realizado e pago será abatido automaticamente do valor da Invoice. 

O adiantamento terá a mesma moeda do processo de importação.

A taxa de câmbio considerada no adiantamento para o fornecedor não será a mesma utilizada no pedido de compra; mas taxa corrente cadastrada na tela **Taxa de câmbio e índice**.

Ao clicar no botão **Adiantamento fornecedor**, será aberta a tela **Adiantamento para fornecedor** para preenchimento de:

- Nº do Adiantamento
- Data de vencimento
- Data de lançamento
- Data do documento
- Taxa de câmbio
- Valor do adiantamento
- Observações

Estes campos serão utilizados para gerar o Lançamento Contábil. 

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.001.png
   :scale: 80%

Por padrão, os campos **Data de vencimento**, **Data de lançamento** e **Data do documento** estarão preenchidos com a data atual ao abrir a tela.

Porém, essa data pode ser alterada. Informe o número do adiantamento, data de vencimento, data de lançamento, data do documento e  valor do adiantamento e clique em **Gerar**.

A seguinte mensagem de sucesso será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.002.png
   :scale: 80%

*BR One :: Adiantamento do fornecedor inserido com sucesso*

**Possíveis ocorrências durante o processo**

Caso os itens não tenham sido inseridos e o usuário clique no botão *Adiantamento fornecedor*, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.003.png
   :scale: 80%

*BR One :: Antes de gerar o adiantamento para fornecedor, é necessário inserir os itens.*

Caso o usuário tente adicionar um adiantamento sem informar uma taxa de câmbio, a seguinte mensagem será apresentada:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.004.png
   :scale: 80%

*BR One :: Para gerar o adiantamento para fornecedor é preciso atualizar a taxa de câmbio.*

Ao clicar no botão *Gerar*, caso a data de lançamento seja superior a data atual, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.005.png
   :scale: 80%

*BR One :: A data de lançamento não pode ser maior que a data atual.*

Caso a data do documento seja superior a data atual, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.006.png
   :scale: 80%

*BR One :: A data do documento não pode ser maior que a data atual.*

Caso alguns desses campos não tenha sido informado, a mensagem respectiva será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.007.png
   :scale: 80%

*BR One :: O valor para o adiantamento não pode ser menor ou igual a 0.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.008.png
   :scale: 80%

*BR One :: A data de vencimento não foi informada.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.009.png
   :scale: 80%

*BR One :: A data de lançamento não foi informada.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.010.png
   :scale: 80%

*BR One :: A data do documento não foi informada.*

- **Lançamento Contábil gerado**

Após adicionar o adiantamento para o fornecedor, será criado  um Lançamento Contábil para este fornecedor. No campo **Observações** será sinalizado que o adiantamento para fornecedor pertence ao processo de importação. 

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.011.png
   :scale: 80%

As contas a serem utilizadas pelo processo são as contas do cadastro do PN do Fornecedor informado no processo de importação. No débito será a Conta de Conciliação Financeira informada na tela de Configurações de Importação e no crédito será o Fornecedor.

Após gerar o Lançamento Contábil, ao clicar no botão [...] ao lado do botão **Adiantamento fornecedor,** na aba Processos, será aberta a tela de detalhes, com o adiantamento inserido, mostrando o nº do documento, status, valor do documento e valor pago.

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.012.png
   :scale: 80%

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.013.png
   :scale: 80%

Após inserir o adiantamento, é necessário realizar o seu pagamento. Vá até a tela *Contas a pagar,* selecione o mesmo fornecedor do adiantamento. Na coluna **Pagamento total** pode ser digitado o valor a pagar, se for um pagamento parcial. O valor pago será com a moeda corrente, após os pagamentos é possível obter detalhes dos status ao clicar no botão [...] do adiantamento.

Há 3 tipos de Status:

- **Aberto**: Quando o adiantamento é inserido.
- **Pago total**: Quando for pago o total do adiantamento.
- **Cancelado**: Quando o adiantamento for cancelado através do botão **Cancelar Adian.**

Nas colunas **Valor documento** e **Valor pago** é possível visualizar o valor do documento e o valor que já foi pago. Não será possível inserir um adiantamento para fornecedor caso a Invoice já tenha sido inserida. 

**Possíveis ocorrências após inserido adiantamento**

Caso o usuário tente inserir um adiantamento após a Invoice, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.014.jpeg
   :scale: 80%

*BR One :: Não é permitido gerar adiantamentos após a Invoice ser inserida.*

Não será possível inserir um adiantamento com valor superior ao valor em aberto. Se o usuário tentar inserir um valor maior, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.015.jpeg
   :scale: 80%

*BR One :: Valor do documento é maior que o valor em aberto para o documento de importação. Valor em aberto:x*

Caso seja clicado no botão *Adiantamento Fornecedor* com o total do documento já pago, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.016.jpeg
   :scale: 80%

*BR One :: O valor total do documento de importação já foi atingido.*

Caso o adiantamento criado já tenha sido pago parcialmente ou com valor total, ele não poderá mais ser cancelado. Caso o usuário tente cancelar um adiantamento já pago, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.017.jpeg
   :scale: 80%

*BR One :: Não é possível cancelar o adiantamento n°: x pois ele já foi pago.*

Para cancelar um esboço, basta selecionar a linha do esboço e clicar em *Cancelar esboço*. Caso não seja selecionada nenhuma linha, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.018.png
   :scale: 80%

*BR One :: Selecione ao menos uma linha para ser cancelada.*

Para cancelar adiantamentos que não estejam pagos, basta selecionar o adiantamento e clicar no botão **Cancelar Adian.**.

Após cancelar, será gerado um LCM de estorno do adiantamento. 

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.019.png
   :scale: 80%

Caso o usuário tente cancelar um adiantamento que já tenha sido pago, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ de\ Fornecedor/Aspose.Words.30de9d45-b3dc-4318-9743-a55b6870897d.020.jpeg
   :scale: 80%

*BR One :: Só é possível cancelar adiantamentos que estejam abertos.*