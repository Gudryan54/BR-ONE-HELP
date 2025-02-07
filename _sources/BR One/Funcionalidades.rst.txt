
Funcionalidades de Suporte
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Funcionalidades**

É possível através do menu Support Desk do SAP (“Ajuda/Support Desk/BR One”), acessar funcionalidades de suporte do BR One: 

- Atualizar licença do BR One.
- Modo de administração.
- Arquivo de log geral.
- Arquivo de log de inicialização.
- Pasta de log.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.003.png

**Atualizar licença BR One**

Caso haja uma liberação de funcionalidade para um determinado cliente, que seja necessário apenas alterar a licença do BR One, esta deve ser colocada na pasta “Ampliações” (detalhes no tópico de instalação e configuração do Add-On).

Com a nova licença nesta pasta, em cada client SAP que for necessário atualização para liberação de funcionalidade, acessar o menu “Atualizar licença BR One". Ao selecionar essa operação será exibida em tela, uma mensagem confirmando a operação.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.004.png

BR One :: A licença atual será substituída pela licença da pasta ampliações. 
O BR One será reiniciado. Continuar?

Se a operação for confirmada e a licença (“AuthBROne.dll”) para a atualização estiver na raiz da pasta de "Ampliações" ou na subpasta “AuthBROne\_x64” (caso seja um client SAP 64bit) e com uma versão mais atual do que da versão instalada, a atualização será executada com sucesso. 

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.005.png

Licença local Atualizada.

Necessário reiniciar o BR One ou client SAP para aplicar esta atualização.

Caso a versão da licença colocada na pasta "Ampliações" seja inferior a versão que está na pasta do BR One, será atualizada a licença da pasta ampliações com a licença que está na pasta do BR One e a seguinte mensagem será exibida:

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.006.png

Licença remota atualizada.

Necessário reiniciar o BR One ou client SAP para aplicar esta atualização.

Após a atualização da licença, uma janela aparecerá em tela e pedirá que o BR One seja reiniciado.

Logo em seguida, outra janela do SAP será exibida e nela haverá três opções: "Reiniciar add-on", "Efetuar logoff da empresa atual" e "Continuar a trabalhar sem este add-on". Para que o add-on funcione corretamente, a primeira opção deve ser escolhida.

A opção "Continuar a trabalhar sem este add-on" não estará disponível caso a opção selecionada em grupo padrão seja definido como "Obrigatório" (1.3  Grupo padrão), é recomendado que o add-on seja definido com essa opção.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.007.png

**Modo de administração**

O modo de administração do BR One contém operações que possuem a finalidade de configurar, preparar e corrigir o ambiente do SAP e do banco de dados para que o BR One seja corretamente executado.

O acesso a esta opção é disponibilizado automaticamente na execução do BR One em ambientes não configurados para executar o add-on. Quando o ambiente não estiver configurado a seguinte mensagem será apresentada:

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.008.png

BR One :: Banco de dados BR One não configurado para essa empresa.

Será em seguida questionado se deseja entrar em modo de administração.

Caso ainda se tenha a necessidade de forçar a execução do modo de administração para algum fim específico, pode se acessar esta opção através do menu "Ajuda/Support Desk/BR One/Modo de administração".

Em ambos os casos, uma mensagem será exibida, para se confirmar se realmente deseja entrar em modo de administração.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.009.png

Entrar em modo de administração? 

OBS: Caso não seja carregado automaticamente, verificar carregamento na barra de tarefas.

Caso o add-on não esteja iniciado, ou não seja possível inicia-lo por alguma configuração ou falha no ambiente, pode-se entrar em modo de administração de maneira alternativa.

Para isto, sem que nenhum cliente do SAP Business One esteja aberto, dê um duplo clique no executável do BR One (BROne.exe), geralmente disponível em:

Client SAP 32bit: "C:\Arquivos de programas(x86)\SAP\SAP Business One\AddOns\UPP\BROne".

Client SAP 64bit: "C:\Arquivos de programas\SAP\SAP Business One\AddOns\UPP\BROne".

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.010.png

Ao clicar no executável do BR One, a mensagem abaixo será exibida, indicando que não há SAP Business One ativo. Caso esta mensagem não seja exibida, é devido ao cliente do SAP Business One estar aberto e, portanto deverá ser fechado para executar este processo.


.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.011.png

BR One:: 	Não foi possível conectar ao SAP Business One. Erro:
Connection – Could not find SBO that match the conection string 

Após esta mensagem, será exibida a mensagem do “Modo de Administração”:


.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.012.png

BR One :: Entrar em modo de administração?

Em todos os cenários, ao confirmar, uma janela será exibida solicitando que o cliente informe os dados de conexão ao banco de dados.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.013.png

OBS: Algumas vezes, a janela não é exibida diretamente em tela, pois as janelas abertas do SAP possuem prioridade no modo de exibição. Nestes casos a janela pode ter sido carregada na barra de tarefas do Windows, bastando selecioná-la para dar continuidade ao processo.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.014.png

Após a conexão, o painel de controle do modo de administração será exibido, com as opções disponíveis.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.015.png

**Configurar base de dados BR One**

Esta opção realiza a pré-configuração do banco de dados para que o BR One seja executado.

Ao selecionar esta opção, outra janela será exibida, contendo as bases SAP Business One disponíveis no servidor informado. Nesta janela devem ser selecionadas em quais bases o BR One deve ser configurado. 

Não deve ser selecionado bases do SAP que não utilizem o add-on.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.016.png

Ao clicar no botão "Executar" o procedimento de configuração é iniciado e pode demorar vários minutos, dependendo do nº de bases selecionada.

Ao executar este procedimento, os campos e tabelas de usuário que estiverem disponíveis em todas as bases selecionadas, serão disponibilizados nas Views do BR One (VSBO) para que possa ser utilizado em relatórios e no add-on. Se o campo estiver disponível em apenas algumas das bases, mas não tiver em todas, ele não será disponibilizado nas Views do BR One.

Após a execução e conclusão da operação um alerta com a mensagem de que a estrutura foi criada será apresentada e a janela para seleção de empresas será exibida novamente e deverá ser encerrada caso não se deseje outra configuração.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.017.png

Caso seja a primeira instalação do add-on em uma base selecionada ou tenha sido atualizada a estrutura do BD com novos campos e tabelas, o add-on deverá ser executado em todas as bases para criação da estrutura para que posteriormente seja executado o modo de administração. 

Para este caso, pode ser necessário executar duas vezes o processo. A primeira para habilitar determinada base e a segunda para fazer com que os campos criados sejam corretamente configurados.

**IMPORTANTE:** Neste processo, caso as bases SAP estejam corrompidas ou com a criação de campos ou estruturas de BD externos ao SAP (procedimento não recomendado e não suportado pela SAP), esta validação poderá apresentar mensagem de erros, exibindo eventuais campos e tabelas com problemas. Esta estrutura deverá ser regularizada para que seja possível utilizar o add-on.

**Revalidar estrutura BR One**

Esta validação irá verificar se as tabelas, campos e objetos foram criados devidamente para utilização do BR One. Por padrão esta verificação já é realizada uma vez por dia, quando o primeiro client é logado ou caso haja alguma atualização de versão do add-on.

Quando selecionado esta opção, a validação e criação dos campos que não foram criados será efetuado assim que o BR One for executado novamente conforme é exibida na mensagem:

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.018.png

Processo será realizado na próxima inicialização do BR One.

**Atualizar configuração DI API**

Esta opção realiza a preparação e correção de alguns ambientes para que o BR One seja executado. 

Esta opção só deve ser utilizada para fins específicos em ambiente que apresentam este problema ou quando for solicitado pelo Suporte Uppertools.

**Encerrar BR One**

**IMPORTANTE:** Esta opção só deve ser utilizada para fins específicos em ambientes ou situações em que for explicitamente solicitado ou quando for solicitado pelo Suporte Uppertools.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.019.png

O add-on BR One será finalizado de maneira forçada. Este processo não é recomendado a menos que seja solicitado para situações específicas.

Após finalização o SAP irá solicitar para reiniciá-lo ou será necessário iniciá-lo manualmente. Continuar?

**Encerrar BR One Administração**

Ao clicar nessa opção, o usuário requer que o modo administração se encerre.

**Abrir log geral**

Essa opção irá abrir um arquivo de texto contendo as mensagens geradas no decorrer dos processos do BR One.

Algumas vezes, a janela não é exibida diretamente em tela, pois as janelas abertas do SAP possuem prioridade no modo de exibição, sendo assim, minimizada na barra de tarefas.

**Abrir log de inicialização**

Essa opção irá abrir um arquivo de texto contendo as mensagens geradas no decorrer dos processos de inicialização do BR One.

Este log é útil para verificar problemas ou situações ocorridas na inicialização do add-on.

Algumas vezes, a janela não é exibida diretamente em tela, pois as janelas abertas do SAP possuem prioridade no modo de exibição, sendo assim, minimizada na barra de tarefas.

**Abrir pasta de log do BR One**

Irá abrir a pasta que contém os logs mencionados acima e outros eventuais logs que possam ser gerados no decorrer dos processos do BR One.

**Opção “Enviar informações”**

Outra funcionalidade é o envio de informações relevantes dos processos do BR One e do ambiente em que está instalado. 

Estas informações tem a finalidade de auxiliar a equipe de Desenvolvimento da Uppertools na resolução de problemas ou situações encontradas no decorrer da execução das tarefas diárias do add-on.

Esta opção fica localizada no menu do BR One na opção "Sobre BR One".

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.020.png

Depois de selecionada, a janela com informações do BR One será exibida em tela, com os componentes que constituem o add-on e sua respectiva versão.

Deverá ser selecionado o botão “Informações” e a opção “Enviar informações”.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.021.png

O usuário deve concordar que deseja enviar suas informações para a Uppertools:

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.022.png

Serão enviadas informações do ambiente par análise da Uppertools. Estas informações poderão conter os logs de atividades do add-on BR One, SAP e sistema operacional e serão criptografadas para envio. Continuar?

Depois que os dados forem enviados, uma mensagem será exibida em tela confirmando o sucesso da operação de envio de informações.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.023.png

Informações enviadas com sucesso!

**Opção “Histórico de versões”**

Na tela "Sobre" do BR One (detalhes no tópico anterior), através do botão "Informações", é possível visualizar histórico de versões de objetos de BD, add-on e pacotes. 

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.024.png

Para que o usuário possa visualizar essas informações é necessário possuir autorização. 

Para atribuir autorização para o usuário, acessar o menu "Administração/Inicialização do sistema/Autorizações/Autorizações gerais".

Na tela de "Autorizações", selecionar um usuário e acessar as opções "Autorização do usuário -> BR One Autorizações -> BR One -> Informações"

Nas opções de "Histórico de versões" clique na coluna "Autorização", altere para "Autorização total" e clique em atualizar.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.025.png

Se o usuário tentar abrir e não possuir permissão a seguinte mensagem será apresentada:

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.026.png

"Sobre - Informações (Usuario não possui permissão)"
BR One :: Usuário sem autorização para realizar esta ação.

**Histórico de versões (objetos de BD)**

Ao abrir a essa opção serão listados todos os scripts da base de dados atual, para melhorar o retorno pode ser feito filtro:

- Por data.
- Pela base atual ou por todas as bases.
- Pelo nome do script.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.027.png

Filtro por data:

Para utilizar esse filtro digite uma data de início no campo "Data de execução (De)" e uma data final no campo "Data de execução (Até)". Clique no botão “Pesquisar” e será retornado todos os dados correspondentes, como ilustrado na imagem a seguir:

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.028.png

Informações - Historico (Objetos de BD) - Filtro Data

Filtro por Nome do BD:

Para utilizar este filtro, selecione uma das opções no campo "Nome do BD" e clique no botão “Pesquisar”. 

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.029.png

Informações - Historico (Objetos de BD) - Filtro Nome do BD

Filtro por Nome do script:

Para utilizar esse filtro selecione uma das opções no campo "Nome do script" e clique no botão “Pesquisar”. Na lista só serão carregados os nomes de scripts já executados no BD.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.030.png

Os filtros também podem ser combinados para refinar ainda mais a busca, no exemplo acima foi selecionado no campo "Nome do script" a opção "Br1\_EstruturaDB" e no campo "Nome do BD" a opção "Todas as bases", se a opção selecionada fosse "Apenas base atual" seria retornado apenas a linha do BD logado.

**Histórico de versões (add-on)**

Ao abrir a essa opção serão listadas todas as versões de add-on que já foram instalados. Para melhorar o retorno pode ser feito filtro:

- Por data.
- Pela base atual ou por todas as bases.

Os detalhes sobre o funcionamento de cada filtro, foram detalhados anteriormente.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.031.png

**Pacotes**

Ao abrir essa opção serão listados todos pacotes que já foram instalados, para melhorar o retorno pode ser feito filtro:

- Por data. 
- Pela base atual ou por todas as bases.

Os detalhes sobre o funcionamento de cada filtro, foram detalhados anteriormente.

.. image:: /_static/Geral/Funcionalidades/Aspose.Words.399f5325-c998-47c1-b343-75e5043b0366.032.png