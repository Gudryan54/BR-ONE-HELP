Configurar Endpoints
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este documento explica os passos necessários para realizar a
configuração dos endpoints da API com a base que será utiliza na API.

**1. Extração dos Endpoints da API**

Antes de iniciar a configuração, é necessário baixar e extrair os
endpoints compatíveis com o tipo de banco de dados utilizado pela sua
empresa.

**2. Importação dos Endpoints no Extension Manager**

Após a extração dos arquivos, é necessário importar os endpoints no SAP
Business One utilizando o Extension Manager.

**Passos:**

1. Dentro do Extension Manager, acesse a aba **Extensions**:

.. image:: /_static/BR\ One\ API/Endpoints/image1.png
   :scale: 60%
   :align: center

|

2. Utilize o botão **Importar**, e na sequência o botão **Browse** para
   buscar o endpoint desejado:

.. image:: /_static/BR\ One\ API/Endpoints/image2.png
   :scale: 60%
   :align: center

|

3. Selecione o arquivo de endpoint desejado e clique em **Upload**:

.. image:: /_static/BR\ One\ API/Endpoints/image3.png
   :scale: 70%
   :align: center

|

4. O upload do endpoint será realizado, nesse momento, basta clicar em
   **Next** e **Finish:**

.. image:: /_static/BR\ One\ API/Endpoints/image4.png
   :scale: 80%
   :align: center

|

.. image:: /_static/BR\ One\ API/Endpoints/image5.png
   :scale: 80%
   :align: center

|

.. image:: /_static/BR\ One\ API/Endpoints/image6.png
   :scale: 80%
   :align: center

|

5. Confirme a importação do endpoint na aba e verifique se o foi
   adicionado com sucesso na lista de extensões.

.. image:: /_static/BR\ One\ API/Endpoints/image7.png
   :scale: 70%
   :align: center

|

**3. Vínculo dos Endpoints da API**

Para que os endpoints funcionem corretamente, é necessário vinculá-los
às bases de dados desejadas.

**Passos:**

1. No Extension Manager do SAP, acesse a aba **Company Assignment:**

.. image:: /_static/BR\ One\ API/Endpoints/image8.png
   :scale: 60%
   :align: center

|

2. Selecione a base que deseja utilizar no vínculo do endpoint e clique
   em **Assign:**

.. image:: /_static/BR\ One\ API/Endpoints/image9.png
   :scale: 60%
   :align: center

|

3. Escolha o endpoint que deseja vincular a base selecionada e clique em
   **Next:**

.. image:: /_static/BR\ One\ API/Endpoints/image10.png
   :scale: 70%
   :align: center

|

4. Avance as telas utilizando o botão **Next** e para finalizar clique
   em **Finish:**

.. image:: /_static/BR\ One\ API/Endpoints/image11.png
   :scale: 70%
   :align: center

|

.. image:: /_static/BR\ One\ API/Endpoints/image12.png
   :scale: 70%
   :align: center

|

.. image:: /_static/BR\ One\ API/Endpoints/image13.png
   :scale: 70%
   :align: center

|

5. Após finalizar o vínculo, o mesmo será exibido na grade de extensões
   vinculadas na base:

.. image:: /_static/BR\ One\ API/Endpoints/image14.png
   :scale: 65%
   :align: center

|

6. Teste o endpoint vinculado para garantir para garantir o correto
   funcionamento.

**Remoção de endpoint da base ou do Extension Manager**

É possível desvincular o endpoint de uma base, para isso, deve-se
acessar a aba **Company Assignment**, selecionar a base desejada e na
lista das extensões vinculadas, selecionar o endpoint desejado e clicar
em **Unassign**.

.. image:: /_static/BR\ One\ API/Endpoints/image15.png
   :scale: 60%
   :align: center

|

É possível remover o endpoint do **Extension Manager**, para isso,
deve-se acessar a aba **Extensions**, selecionar o endpoint desejado e
clicar em **Remove**.

.. image:: /_static/BR\ One\ API/Endpoints/image16.png
   :scale: 70%
   :align: center

|
