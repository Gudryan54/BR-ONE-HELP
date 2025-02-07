Configurações
~~~~~~~~~~~~~

.. image:: /_static/BR\ One\ Produção/Processo/Desmontagem/desmon01.png
   :scale: 80%

- **Conta contábil de desmontagem:**

Para adicionar uma Ordem de Produção de Desmontagem é necessário configurar uma conta contábil de desmontagem, para que sejam realizados os lançamentos de desvios e fechamento de custos, esta configuração está na tela **"Configurações de produção"**, na aba **"O.P"**.


Não é permitido inserir uma conta contábil do tipo **"Título"**.

.. image:: /_static/BR\ One\ Produção/Processo/Desmontagem/desmon02.png
   :scale: 80%
   
- **Lista de Preço para Desmontagem:**

Esta funcionalidade exibirá todas as listas de preço disponíveis no SAP, permitindo que o usuário selecione qual lista utilizar para o cálculo do custo dos componentes durante a desmontagem de um item. Vale ressaltar que a lista de preço selecionada será considerada somente se, 
na Ordem de Produção, a origem do custo estiver definida como **"Lista de Preço"**.

- Algumas configurações de produção não são consideradas para o processo da **OP de Desmontagem**.

Entre elas temos, a aba **"Lote/Série"**, onde nenhuma configuração é considerada.

.. image:: /_static/BR\ One\ Produção/Processo/Desmontagem/desmon03.png
   :scale: 80%

Já os parâmetros **"Não fechar OP sem apontamento de materiais"** e **"Não fechar OP sem apontamento de PA"** da aba **"O.P"**, mesmo quando marcadas, são desconsiderados para OPs de Desmontagem.

.. image:: /_static/BR\ One\ Produção/Processo/Desmontagem/desmon04.png
   :scale: 80%