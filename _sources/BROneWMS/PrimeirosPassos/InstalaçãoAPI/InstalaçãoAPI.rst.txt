Instalação API WMS
^^^^^^^^^^^^^^^^^^^^

| \

.. tip::

   Saiba como atualizar a versão da API WMS clicando :doc:`aqui <../../Versões/Atualização/Atualização>`.

| \

Pré requisitos
---------------------------

Para realizar a instalação da API WMS, serão necessários os pré-requisitos:

- **Servidor Windows com IIS (Internet Information Services) habilitado;**

| \

.. image:: WMS-IIS.png
   :align: center

| \

- **ASP.NET Core Runtime 3.1.32 Hosting Bundle instalada** (`link web <https://dotnet.microsoft.com/en-us/download/dotnet/3.1>`_);

| \

.. image:: WMS-ASPNET.png
   :align: center

| \

- **Caso o ambiente possua o SAP na versão 9.3, será necessário verificar se os drivers HANA estão instalados.**

.. note::

   Este pré-requisito se aplica apenas para ambientes SAP 9.3, para SAP 10 não será necessária a instalação dos drivers HANA.

| \

.. image:: WMS-PesquisODBC.png
   :align: center

| \

Na barra de pesquisa do Windows, pesquisando por ODBC, selecione o tipo do sistema (64 ou 32 bits).

| \

.. image:: WMS-ODBCDrivers.png
   :align: center

| \

Na aba Drivers, verifique a existência do driver **HDBODBC** instalado. Na existência do driver instalado, nenhuma ação será necessária. Caso o contrário baixe e instale os drivers abaixo:

.. |SAP_HANA_CLIENT_1.0_X64.rar| replace::
   :download:`SAP_HANA_CLIENT_1.0_X64.rar <SAP_HANA_CLIENT_1.0_X64.rar>`

.. |SAP_HANA_CLIENT_1.0_X86.rar| replace::
   :download:`SAP_HANA_CLIENT_1.0_X86.rar <SAP_HANA_CLIENT_1.0_X86.rar>`

- |SAP_HANA_CLIENT_1.0_X64.rar|

| \

- |SAP_HANA_CLIENT_1.0_X86.rar|

| \

.. image:: WMS-HDBSETUP.png
   :align: center

| \

Extraia os arquivos, acesse a pasta e execute o **hdbsetup.exe**. No wizard de instalação, basta prosseguir (next) em todas as etapas e aguarde a instalação dos drivers.

| \

Deploy da API no diretório
----------------------------

| \

.. image:: WMS-PastaAPI.gif
   :align: center

| \

Em **C:/inetpub**, crie um novo diretório que será usado na instalação da API.

| \

.. image:: WMS-IIS_IUSRS.png
   :align: center

| \

Nas Priopriedades da pasta, na aba Segurança, edite e adicione o usuário **IIS_IUSRS** com permissão de Controle total na pasta.

| \

.. image:: WMS-DeployAPIPasta.gif
   :align: center

| \

Baixe a versão da API WMS, extraia e copie todos os arquivos para o diretório criado em **C:/inetpub**.

| \

.. image:: WMS-appsettings.png
   :align: center

| \

No diretório de instalação da API, abra o arquivo **appsettings.json**, e altere as informações abaixo:

- **ServiceLayerURL**: insira a URL da service layer do SAP B1;
- **DefaultUser** e **DefaultPassword**: insira o usuário/senha do SAP que será utilizado em todas as requisições;
- **Server**: insira o IP/porta do servidor de banco de dados;
- **User** e **Password**: insira o usuário/senha do usuário de banco de dados;
- **Type**: insira o tipo do banco de dados, HANA ou SQL.

| \

Baixe e extraia o arquivo abaixo e substitua no diretório de instalação da API.

| \

.. |webconfig.rar| replace::
   :download:`web.config <webconfig.rar>`

- |webconfig.rar|

| \

Deploy da API no IIS
----------------------------

| \

.. image:: WMS-CriandoPool.gif
   :align: center

| \

No IIS, crie um novo Application Pool, alterando apenas o **.NET CRL version:** para "No Managed Code".

| \

.. image:: WMS-CriandoSite.gif
   :align: center

| \

Crie um novo Site, preenchendo o **Site Name** de acordo com o nome do diretório criado no inetpub. Em **Application Pool** clique em Select e selecione o Pool criado anteriormente. No **Physical Path**, clique em "..." e selecione o diretório da instalação da API. Em **Binding** defina o protocolo entre **http** ou **https** e escolha a **Port**.

| \

.. image:: WMS-Swagger.gif
   :align: center

| \

Realizando todas as etapas anteriores, para validar se houve sucesso na instalação, abra um navegador e digite a URL de acordo com a configuração realizada.

- [http/https]://localhost:[porta configurada]/swagger.

- Nesse exemplo: http://localhost:9000/swagger

Abrindo o swagger e listando os endpoints, a instalação foi realizada com sucesso. Caso exiba alguma mensagem de erro ao abrir a página, reveja as etapas de instalação.

| \

Deploy dos Endpoints Customizados
----------------------------------

| \

.. note::

   O deploy dos endpoints customizados deverá ser realizado apenas para ambientes que utilizarão BR One Produção.

| \

Baixe os endepoints customizados abaixo de acordo com o tipo de banco de dados:

.. |EndpointsCustomizados_SQL.rar| replace::
   :download:`EndpointsCustomizados_SQL.rar <EndpointsCustomizados_SQL.rar>`

.. |EndpointsCustomizados_HANA.rar| replace::
   :download:`EndpointsCustomizados_HANA.rar <EndpointsCustomizados_HANA.rar>`

- |EndpointsCustomizados_SQL.rar|

| \

- |EndpointsCustomizados_HANA.rar|

| \

No servidor onde a API está instalada, acesse o Extension Manager. Normalmente será semelhante a URL abaixo:

- https://[nomeservidor]:40000/ExtensionManager/

| \

.. image:: WMS-AbaExtension.gif
   :align: center

| \

No Extension Manager, na aba Extensions, clique em Import e procure o endpoint customizado e faça o upload. Dê next em todas etapas e refaça o procedimento até importar todos os endpoints.

| \

.. image:: WMS-CompanyAssignment.gif
   :align: center

| \

Na na aba Company Assignment, selecione a base de dados, clique no botão Assign, selecione o endepoint importado e dê next em todas as etapas. Refaça o procedimento até atribuir todos os endpoints.