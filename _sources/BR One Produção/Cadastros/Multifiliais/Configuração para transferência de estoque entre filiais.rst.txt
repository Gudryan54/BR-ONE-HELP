Configuração para transferência de estoque entre filiais
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A tela Configuração de depósitos para referência é utilizada para configuração do processo de Transferêrencia de estoque entre filias.

Portanto, ela está disponível apenas para bases multi-filiais.

Para acessar a tela é necessário ir no menu:

**Administração > Definição > Estoque > Configurações de transferência entre filiais**.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.011.png


Nessa tela, devem ser preenchidos os campos:

- **Utilização:**

Essa utilização será utilizada nos documentos de **"NF de Saída"** e **"NF de Entrada"**. Serão carregadas apenas as que em seu cadastro possuírem a flag **"Só imposto"** marcada e as flags **"Transf. Estoque"** e **“Gratuito”** desmarcadas. 

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.012.png


**Observação:** Caso a versão do SAP seja 9.1 ou superior, em vez de marcar o campo **“Só Imposto”** selecione o campo **“Gratuito”**.

- **Utilizar depósito padrão do item:**

Quando parâmetro está marcado, indica que será utilizado o deposito padrão configurado no cadastro do item.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.013.png


- **Realizar conferência do recebimento:**

Quando parâmetro está marcado, indica que será utilizado o depósito **“Em trânsito”** cadastrado na tela de filias.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.014.png


Caso a marcação não estiver realizada, processo deverá ser o mesmo já existente, ou seja, deve preencher o campo depósito de acordo com a configuração **“Utilizar depósito padrão”** e a **“Configuração de depósito de referência”**.

- **Responsável pela conferência:**

Indica qual usuário receberá o alerta das quantidades a mais ou a menos na conferência final. Lembrando que:

- Apenas colaboradores existentes podem ser selecionados;

- Apenas colaboradores ativos podem ser selecionados;

- Apenas colaboradores com o usuário preenchidos podem ser selecionados;

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.015.png


- **Abrir esboço NF de Entrada gerado automaticamente:**

Indica se o esboço de **"NF de Entrada"** gerada pelo processo será carregado para visualização.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.016.png


- **Adicionar NF de entrada automaticamente:**

Quando o parâmetro está marcado, indica que a NF de entrada será gerada automaticamente.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.017.png


Com o parâmetro **"Adicionar NF de entrada automaticamente"** marcado é possível escolher entre duas opções **"Sem chave de acesso vinculada"** e **"Com chave de acesso vinculada"**.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.018.png


Não será possível selecionar a opção **"Com chave de acesso vinculada"**, caso o campo **"Solução Fiscal"** que se encontra na tela **‘Configurações de documento’** na aba **‘BR One’** esteja definido como **"Nenhum"**.

Caso o usuário tente selecionar, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.019.png


*Para buscar a chave de acesso primeiro informe a solução fiscal em Configurações do Documento > aba BR One*

Não é possível marcar os campos **"Abrir esboço NF de Entrada gerado automaticamente"** e **"Adicionar NF de Entrada automaticamente"** ao mesmo tempo.

Caso o parâmetro **"Abrir esboço NF de Entrada gerado automaticamente"** esteja marcado e o usuário tente selecionar a opção **"Adicionar NF de Entrada automaticamente",** a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.020.png


*Parâmetro disponível apenas se a opção "Abrir esboço NF de Entrada gerado automaticamente" estiver desmarcada.*

Caso o parâmetro **"Adicionar NF de Entrada automaticamente"** esteja marcado e o usuário tente selecionar a opção **"Abrir esboço NF de Entrada gerado automaticamente",** a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.021.png


*Parâmetro disponível apenas se a opção "Adicionar NF de Entrada automaticamente" estiver desmarcada.*

- **Abrir esboço de NF de faturamento gerada automaticamente:**

Indica se o esboço de **NF de faturamento** gerada pelo processo será carregado para visualização.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ para\ transferência\ de\ estoque\ entre\ filiais/Aspose.Words.74079a32-c677-4bfd-851d-b9e8685101c9.022.png

