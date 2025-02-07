Invoice
~~~~~~~~~~~~~~~~

Para criar uma Invoice basta clicar em **Invoice** na aba de **processos** e sua tela será aberta, devendo ser inserido o número da Invoice , a data de vencimento, de lançamento e do documento. No momento de gerar a Invoice, caso haja, serão descontados os adiantamentos para fornecedor já criados. A Invoice seguirá a mesma moeda do processo de importação e a taxa de câmbio será a taxa do dia da geração do documento. Com isso será gerado um LCM na moeda estrangeira.

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.001.png
   :scale: 80%

Por padrão, os campos **Data de lançamento** e **Data do documento** estarão preenchidos com a data atual ao abrir a tela. 
Porém, essas datas podem ser alteradas. Informe o número da Invoice , a data de vencimento, de lançamento e do documento e clique em **Gerar**. 
A seguinte mensagem de sucesso será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.002.png
   :scale: 80%

*BR One :: Invoice inserida com sucesso.*

- **Possíveis ocorrências durante o processo**

Antes de criar a Invoice, é necessário inserir os itens do pedido de compra. Caso os itens não tenham sido inseridos e o usuário clique no botão **Invoice**, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.003.png
   :scale: 80%

*BR One :: Antes de gerar a Invoice é necessário inserir os itens.*

Para gerar a Invoice, é necessário que todos os adiantamentos estejam pagos. Caso não estejam pagos, será exibida a seguinte mensagem:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.004.jpeg
   :scale: 80%

*BR One :: Existem adiantamentos não pagos n°(s) ( x), antes de gerar a Invoice realizar o pagamento ou o cancelamento dos adiantamentos.*

Também é necessário observar as Despesas de Invoice para esse processo, pois caso exista alguma despesa lançada, é obrigatória a execução do **Rateio de Invoice** antes de criar a Invoice. Caso aconteça de existirem despesas de Invoice e o rateio não estiver feito, ao tentar adicionar a Invoice, será exibida a mensagem de erro:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.005.jpeg
   :scale: 80%

*BR One :: Realize o processo de **Rateio de Invoice** antes de realizar este processo.*

A Invoice só pode ser criada uma única vez, caso ela já tenha sido inserida e ao tentar criar uma outra Invoice, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.006.jpeg
   :scale: 80%

*BR One :: É possível realizar o processo de Invoice uma única vez.*

Não é possível cancelar uma Invoice quando houver documentos posteriores criados (NF Nacionalização, NF Transporte etc.). Se o usuário tentar cancelar uma Invoice vinculada a documentos posteriores já criados, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.007.jpeg
   :scale: 80%

*BR One :: Não é possível cancelar a Invoice, documentos posteriores já foram criados.*

Ao clicar no botão **Gerar**, caso a data de lançamento seja superior a data atual, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.008.png
   :scale: 80%

*BR One :: A data de lançamento não pode ser maior que a data atual.*

Caso a data do documento seja superior a data atual, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.009.png
   :scale: 80%

*BR One :: A data do documento não pode ser maior que a data atual.*

Caso alguns desses campos não tenha sido informado, a mensagem respectiva será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.010.png
   :scale: 80%

*BR One :: A data de vencimento não foi informada.*

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.011.png
   :scale: 80%

*BR One :: A data de lançamento não foi informada.*

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.012.png
   :scale: 80%

*BR One :: A data do documento não foi informada.*

- **Lançamento Contábil gerado**

O Lançamento Contábil será criado. No campo **Observações** será sinalizado o número do processo de importação no qual a Invoice pertence.

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/1.png
   :scale: 80%

As contas a serem utilizadas pelo processo são as contas do cadastro do PN do fornecedor informado no processo de importação. No débito será a Conta de Importações em Andamento e no crédito será o Fornecedor.

O botão [...] da Invoice abrirá a tela de detalhes com a Invoice inserida, mostrando o nº do documento, status, valor do documento, adiantamento pago e valor pago.

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.014.png
   :scale: 80%

Ao selecionar uma invoice e clicar no botão ****Cancelar Invoice***, o LCM será estornado e a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.015.png
   :scale: 80%

*BR One :: Invoice nº **XXX** cancelada com sucesso.*

Há os status:

- **Aberto**: Quando a Invoice ainda não foi paga.
- **Cancelado**: Quando a Invoice for cancelada.
- **Pago Parcial**: Quando a Invoice tiver o valor pago parcialmente.
- **Pago Total**: Quando a Invoice tiver o valor pago total.

Esses são os status da Invoice visualizado nos detalhes.

- **Possíveis ocorrências após inserida a Invoice**

O botão **Cancelar Invoice** cancela o LCM que estiver selecionado. Caso seja clicado no botão e não haja nenhuma linha selecionada, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Invoice/Aspose.Words.f3770a86-7fe7-4a13-8f24-5b20679ce69e.016.png
   :scale: 80%

*BR One :: Selecione ao menos uma linha para realizar o cancelamento dos esboços.*


