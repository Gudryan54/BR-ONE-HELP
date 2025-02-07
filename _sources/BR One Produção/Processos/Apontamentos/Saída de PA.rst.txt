Saída de Produto Acabado
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta tela é possível realizar a saída de produtos acabados.

Para acessar essa tela pode utilizar as opções:


- Através do menu **Produção -> Saída de produto acabado**;


- Através do Terminal de Apontamentos;


- Através do botão direito na Ordem de Produção de Desmontagem liberada.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.002.png


Para realizar a saída de produto acabado, basta informar os campos **"Nº da ordem de produção"**, o **"Depósito"** e a **"Quantidade"**. 

O CFL (Choose From List) do campo **“Nº ordem produção”** será carregado da seguinte forma:

- Quando o campo estiver vazio, apenas aparecerão as 100 primeiras OPs para seleção.

- Quando o campo estiver com \*, aparecerão todas as OPs disponíveis para saída de PA.

- Quando houver algum filtro, aparecerão todas as OPs de acordo com o filtro informado.

**OBS.:** Somente serão carregadas no CFL, OPs do tipo **Desmontagem**, que possuam o status **"Liberada"**.

Caso o usuário tente adicionar uma saída sem informar o número da OP, a seguinte mensagem será exibida ao usuário:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.003.png


*BR One :: Informe uma ordem de produção.*

Para o campo **"Depósito"**, caso a base seja multifilias, só poderão ser selecionados depósitos que pertençam à mesma filial do depósito informado na ordem de produção. 

Caso o parâmetro **"Bloquear alteração do campo depósito"** esteja desmarcado, e o usuário tente adicionar uma saída sem informar o depósito, a seguinte mensagem será exibida ao usuário:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.004.png


*BR One :: Informe um depósito.*



Caso o usuário tente adicionar uma saída sem informar uma quantidade, a seguinte mensagem será exibida ao usuário:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.005.png


*BR One :: Informe uma quantidade maior que zero.*


Ao realizar uma saída de produto acabado, é feita uma saída de mercadoria para o PA da Ordem de produção de Desmontagem e é realizado uma entrada de mercadoria para os componentes da OP que possuem **"Método baixa"** configurado como baixa por explosão.

Segue abaixo exemplo de **"Saída de produto acabado"** para a ordem de produção de desmontagem: 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.006.png



Saída de mercadoria e Entrada mercadoria gerados no processo de saída de PA:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.007.png


Lançamento contábil manual gerado no processo:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Saída\ de\ PA/Aspose.Words.ff716fd9-9385-40ca-9115-1d28cdd740c4.008.png

