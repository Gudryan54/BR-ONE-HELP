Transferência entre filiais - Manual
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O processo de Transferência entre filiais podem ser gerados manualmente através da tela Transferência de estoque.

Para acessar a tela é necessário ir  no menu:

**Estoque -> Transações de estoque -> Transferência de estoque**

Na transferência de estoque devem ser informados:

- **Parceiro de negócio**

Deve ser informado o Parceiro de negócio do tipo **Cliente** informado na filial de destino.

**Lembrete:** Para o funcionamento correto do processo, nas configurações de **Filiais - Definição** é preciso estar parametrizados os PN’s a serem utilizados no processo.

- **Filial**

Ao informar o depósito **“Do depósito”**, manualmente, ele preenchera a filial automaticamente padrão de acordo com o depósito informado.

- **Depósitos**

No processo manual é preciso informar os depósitos manualmente:

**Do Depósito:** Tem que ser informado um depósito da Filial Origem.

**Para Depósito:** Tem que ser informado o **Depósito em trânsito** , configurado na tela **Filiais – Definição** referente a filial de origem.

- **Item**

Nas linhas do documento deve ser informado os itens que serão transferidos.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.020.png


A Transferência de estoque gera o **Lançamento Contábil Manual**:

- **Crédito:** Conta de estoque 

- **Débito:** Conta de estoque


Após adicionar a **transferência de estoque**, o add-on gera um esboço de **Nota Fiscal de Saída** 

**Nota fiscal de saída**

É aberto o esboço na tela, com as informações preenchidas de acordo com as configurações e transferencia de estoque:

- **Parceiro de negócio:** O Cliente informado é o que está definido nas configurações da tela **Filiais – Definição** , na coluna **Cliente da filial** da filial que será destino.

- **Filial**: A filial informada é a origem.

- **Item**: Carregado os itens da **transferência de estoque**

- **Depósito**: O deposito preenchido é das configurações **Filiais – Definição** de **Envio direto** da filial origem.

- **Utilização**: É informado a utilização configurada na tela **Configurações de transferência entre filiais**.

- **Quantidade**: A quantidade é a mesma informada na **transferência de estoque**.

- **Observações:** É preenchido pelo add-on uma observação informando que o documento é referente ao processo de transferência entre filiais, e o Nº transferência de estoque**.**

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.021.png


A NF de saída gera o **lançamento contábil manual**:

- **Crédito:** Conta de Receita
- **Débito:** Na conta para saída gratuita


Após adicionar a **Nota Fiscal de Saída**, o add-on gera um esboço de **NF de entrada**.

**NF de entrada**

Para adição da NF de Entrada diversos parametros são levados em consideração:

**1.** Caso o parâmetro **“Abrir esboço NF de Entrada gerado automaticamente”** esteja marcada.

Nesse processo o add-on valida o parâmetro “Abrir esboço NF de entrada gerado automaticamente”, se está marcado na tela **BR One :: Configurações de transferência entre filiais**.

- **Abre o NF de entrada - Esboço**

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.022.png


A NF de entrada gera um **lançamento contábil manual**:

- **Crédito:** Conta de entrada gratuita
- **Débito:** Conta de despesas

Ao adicionar a NF de entrada, o sistema automaticamente gera uma **saída de mercadoria** e uma **entrada de mercadoria** por DI. 

**2.** Caso o parâmetro **“Abrir esboço NF de Entrada gerado automaticamente”** esteja desmarcada.

Caso o parâmetro esteja desmarcado na tela **BR One :: Configurações entre filiais** , ao adicionar a **Nota Fiscal de Saída - Esboço** será necessário buscar o esboço da NF de entrada na tela **Transf. Filiais – Relatório de NF de Entrada pendentes**.

Ao adicionar  **Nota Fiscal de entrada – Esboço** , o sistema automaticamente gera uma **saída de mercadoria** e uma **entrada de mercadoria** por DI.

**3.** Processo com “Adicionar NF de entrada automaticamente – sem chave de acesso vinculada”, marcada.

Com esse parâmetro marcado na tela **“BR One :: Configuração transferência entre filiais”** , ao adicionar **Nota Fiscal de Saída – Esboço**  o add-on irá gerar Nota Fiscal de Entrada por DI com os campos preenchidos automaticamente: 

- Nº NF

- Serial

- Serie

- Subsérie

- Modelo 

E irá gerar a  **saída de mercadoria** e **entrada de mercadoria** por DI.

É possível buscar a Nota Fiscal de Entrada, através:

**Compras – C/P -> Nota Fiscal de Entrada**

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.023.png


**4.** Processo com “Adicionar NF de entrada automaticamente – com chave de acesso vinculada”, marcada

Com esse parâmetro marcado na tela **“BR One :: Configuração transferência entre filiais”**, ao adicionar **Nota Fiscal de Saída – Esboço** , o add-on não gerar NF de Entrada. 

Para adição dessa Nota Fiscal de Entrada é necessário que a Nota Fiscal de Saída esteja com a chave de acesso preenchida de acordo com o Add-on fiscal.

Com a chave de acesso preenchido é necessário na Nota Fiscal de Saída ir na opção **Operações adicionais -> Gerar NF de Entrada**

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.024.png


Ao selecionar a opção o add-on irá gerar NF de Entrada por DI com os campos preenchidos automaticamente: 
- Nº NF

- Serial

- Serie

- Subsérie

- Modelo 

- Chave de acesso 

E irá gerar a  **saída de mercadoria** e **entrada de mercadoria** por DI.

É possível buscar a Nota Fiscal de Entrada, através:

**Compras – C/P -> Nota Fiscal de Entrada**


**Saída de mercadoria**

A Saída de mercadoria é inserida na filial de origem com o deposito em transito utilizado na transferência de estoque.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.025.png



A saída de mercadoria gera **lançamento contábil manual**:

- **Crédito:** Conta de estoque

- **Débito:** "Conta de saída" definida no depósito em trânsito da filial origem


**Entrada de mercadoria**

A entrada de mercadoria é inserida na filial de destino, o depósito é preenchido de acordo com a definição do parâmetro **Utilizar depósito padrão do item**.

Entrada de mercadoria com o parâmetro **marcado**:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.026.png


O depósito da entrada de mercadoria será recuperado no cadastro do item na aba estoque definido como depósito padrão, caso o depósito padrão do item não seja correspondente a filial destino, o Add-on irá recuperar o depósito conforme **configuração de depósito para referência**. 

Se não existir um deposito padrão no cadastro do item é recuperado o deposito padrão da filial definido no cadastro das Filiais.

Entrada com o parâmetro **desmarcado**:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Transferência\ entre\ filiais/Aspose.Words.0843b7bd-0047-4dce-8b53-352fa2e84686.027.png


O deposito da entrada de mercadoria será recuperado na tela de **configuração de depósito para referência**, com base no depósito utilizado na **transferência de estoque** do campo **“DO depósito”**. 

Se não existir o cadastro do depósito na tela é recuperado o deposito padrão da filial definido no cadastro das Filiais.

A Entrada de mercadoria gera um lançamento contábil manual:

- **Crédito:** "Conta de entrada" definida no depósito em informado na demanda. 

- **Débito:** Conta de estoque