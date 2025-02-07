
Instalação do add-on BR One Cloud
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Configuração das permissões de usuário**

A instalação do add-on **e a primeira execução** do mesmo realiza diversas configurações tanto na base da Company quanto na base exclusiva do BR One, chamada UPP\_BRONE, que é criada em tempo de execução após a instalação.

Estas configurações demandam algumas permissões diferentes das criadas automaticamente pela solução SAP Cloud Control Center e, portanto, é necessário aplicar estas permissões manualmente.

**Usuário do SAP** 

- O usuário do SAP deverá ser “Super usuário”.

**Usuário do Windows**

- O usuário do Windows deverá pertencer ao grupo de administradores ou equivalente, com permissão na pasta de instalação do SAP Business One. 

**Usuários do banco de dados**

- Usuário criado automaticamente pela solução SAP Cloud Control Center:
  - Banco UPP\_BRONE
- Leitura
- Escrita
- Público
- Demais atribuições
- View any definition
- Usuário vinculado ao grupo de domínio do Windows (Administrador ou equivalente)
- Banco UPP\_BRONE
- Leitura
- Escrita
- DDL\_ADMIN 
- Público
- Demais atribuições
- View any definition

- Usuário vinculado ao grupo do domínio do Windows (perfil restrito, usuário comum)
- Banco UPP\_BRONE
- Leitura
- Escrita
- Público
- Demais atribuições
- View any definition

A atribuição “View any definition” é importante estar liberada ao usuário vinculado tanto para o grupo de domínio administrador quanto ao grupo de domínio do usuário “comum” pois em toda inicialização são realizadas consultas validando se os objetos de banco de dados necessários foram criados (tópico 3 **Validações obrigatórias do add-on***).

**Registro do add-on (extensão), deploy e instalação**

**Processo de registro / deploy**

Caso o add-on ainda não tenha sido instalado, basta realizar o registro do mesmo como uma “extensão” na Service Unit desejada.

Após a conclusão do registro, realizar o **deploy** do add-on às Companies desejadas.

O processo de registro de extensões é descrito em detalhes no guia de utilização/manutenção do SAP CCC Landscape.

**Processo de instalação**

A instalação do Add-on iniciará automaticamente (conforme tela abaixo). Na tela seguinte, clique em *“Avançar”.*

.. image:: /_static/Geral/Cloud/Aspose.Words.970f67b6-56ec-47fd-88c7-381c53332713.002.png

Será mostrado o caminho onde o add-on será instalado. Clique em Instalar. Será exibido a seguinte mensagem:

.. image:: /_static/Geral/Cloud/Aspose.Words.970f67b6-56ec-47fd-88c7-381c53332713.004.png


*Poderá ser solicitado os dados de acesso para conexão com o banco de dados.
Sendo necessário, será solicitado usuário e senha com permissão de super usuário. Verifique o carregamento da tela na barra de tarefas (caso não seja carregado automaticamente).*

.. image:: /_static/Geral/Cloud/Aspose.Words.970f67b6-56ec-47fd-88c7-381c53332713.003.png

Após o processo de instalação ser completado, clique em Concluir para finalizar. 

Caso o usuário não possua as permissões necessárias, ou as configurações devidas não tenham sido realizadas conforme o tópico 1.1 **Configuração das permissões de usuário***, o add-on irá solicitar as credenciais do usuário conforme mensagem anterior.

.. image:: /_static/Geral/Cloud/Aspose.Words.970f67b6-56ec-47fd-88c7-381c53332713.005.png

**Variáveis de ambiente customizáveis**

É possível customizar alguns aspectos do add-on via arquivo de configuração XML, a alteração destas configurações mudará o comportamento do add-on em “tempo de execução” apenas na máquina onde a configuração foi aplicada.

**Caminho dos arquivos de logs**

Por padrão, os logs do BR One são salvos na pasta de instalação de add-on, dentro de uma pasta chamada “Logs”. Caso seja necessário alterar este local, basta editar/criar o arquivo XML **PathConfiguration.xml**.

No elemento **LOG** incluir o caminho a ser salvo.

Após definição deste caminho, todos os logs do BR One serão salvos na pasta indicada. 

.. image:: /_static/Geral/Cloud/Aspose.Words.970f67b6-56ec-47fd-88c7-381c53332713.006.png

**Atualização do add-on BR One**

Para atualizar o add-on no ambiente CLOUD não é necessário realizar as etapas de instalação, sendo necessário apenas extrair os arquivos disponibilizados em cada versão diretamente na pasta de instalação do add-on na Service Unit desejada.

No registro do SAP irá permanecer a versão “base” que foi instalada, porém na janela “Sobre” do BR One, será exibida qual a versão atualizada.

**IMPORTANTE:** A cada atualização do add-on **é obrigatória a atualização da licença** (arquivo “AuthBrOne”) que deve ser solicitada no **Canal do Parceiro/Cliente**.


