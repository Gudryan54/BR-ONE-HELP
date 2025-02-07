Adiantamento Despachante
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Assim como no adiantamento fornecedor, o adiantamento despachante não é um processo obrigatório e serve para obter o controle de contas a pagar do despachante. 

Ao clicar no botão **Adiantamento despachante,** a tela de adiantamento será aberta, devendo ser inserido o valor do adiantamento, a data de vencimento, de lançamento e do documento. Só poderá ser gerada uma parcela por vez. O adiantamento para o despachante (LCM) será gerado em moeda corrente. Não há limites de adiantamento para o mesmo processo.

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.001.png
   :scale: 80%

Por padrão, os campos **Data de lançamento** e **Data do documento** estarão preenchidos com a data atual ao abrir a tela. Porém, essas datas podem ser alteradas. Informe o valor do adiantamento, data de vencimento, data de lançamento e data do documento e clique em **Gerar**. A seguinte mensagem de sucesso será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.002.jpeg
   :scale: 80%

*BR One :: Adiantamento despachante inserido com sucesso.*

- **Possíveis ocorrências durante o processo**

Caso os itens não tenham sido inseridos e o usuário clique no botão **Adiantamento despachante*, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.003.png
   :scale: 80%

*BR One :: Antes de gerar o adiantamento para despachante é necessário inserir os itens.*

Ao clicar no botão **Gerar*, caso a data de lançamento seja superior a data atual, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.004.png
   :scale: 80%

*BR One :: A data de lançamento não pode ser maior que a data atual.*

Caso a data do documento seja superior a data atual, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.005.png
   :scale: 80%

*BR One :: A data do documento não pode ser maior que a data atual.*

Caso alguns desses campos não tenha sido informado, a mensagem respectiva será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.006.png
   :scale: 80%

*BR One :: O valor para o adiantamento não pode ser menor ou igual a 0.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.007.png
   :scale: 80%

*BR One :: A data de vencimento não foi informada.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.008.png
   :scale: 80%

*BR One :: A data de lançamento não foi informada.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.009.png
   :scale: 80%

*BR One :: A data do documento não foi informada.*

- **Lançamento Contábil gerado**

O Lançamento Contábil será criado com o adiantamento para o despachante. No campo **Observações** será sinalizado que o adiantamento para despachante pertence ao processo de importação. As contas a serem utilizadas pelo processo são as contas do cadastro do PN do despachante informado no processo de importação.

No débito será a Conta Adiantamentos de Fornecedores e no crédito será o despachante. O botão [...] do adiantamento para despachante abrirá a tela de detalhes, com o adiantamento inserido, mostrando o nº do documento, status, valor do documento e valor pago.

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.010.png
   :scale: 80%

Após inserir o adiantamento, é necessário realizar o seu pagamento. Vá até a tela **Contas a pagar,** selecione o mesmo despachante do adiantamento. Na coluna **Pagamento total** pode ser digitado o valor a pagar, se for um pagamento parcial. O valor pago será com a moeda corrente. Adicione o **Contas a pagar.** Clique no botão [...] do adiantamento para verificar o status.

Também é possível cancelar adiantamentos que não estejam pagos. Basta selecionar o adiantamento e clicar no botão “*Cancelar Adian.”.** Após cancelar, será gerado um LCM de estorno do adiantamento. 

Há 3 tipos de Status:

- **Aberto:** Quando o adiantamento é inserido.
- **Pago total:** Quando for pago o total do adiantamento.
- **Cancelado:** Quando o adiantamento for cancelado através do botão **Cancelar Adian.*

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.011.png
   :scale: 80%

- **Possíveis ocorrências após inserido adiantamento**

Caso o usuário tente cancelar um adiantamento que já tenha sido pago, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Processo/Adiantamento\ despachante/Aspose.Words.b45c30d8-9215-4ba5-8faf-2555728a4a3c.012.jpeg
   :scale: 80%
   
*BR One :: Só é possível cancelar adiantamentos que estejam abertos.*


