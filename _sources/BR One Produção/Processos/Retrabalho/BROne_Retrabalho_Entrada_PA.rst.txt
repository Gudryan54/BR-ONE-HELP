Entrada de PA
~~~~~~~~~~~~~~~~~~~~~

Ao realizar a entrada de Produto acabado (PA), algumas validações serão realizadas:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img01.png
   :scale: 100% 
   :align: center
 
| \

O campo **“Custo unitário”** não pode ser igual a zero. Caso seja, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img02.png
   :scale: 100% 
   :align: center
 
| \

**BR One :: O custo unitário dever maior que zero.**

A quantidade da entrada de PA deve ser menor ou igual a quantidade planejada da Ordem de produção (PA), caso contrário, exibirá a seguinte mensagem:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img03.png
   :scale: 100% 
   :align: center 

| \

**BR One :: Não é permitido apontar uma quantidade de produto acabado maior que a quantidade planejada na OP de retrabalho.**

Caso a quantidade informada na tela de entrada de produto acabado (PA) seja menor que a quantidade planejada da Ordem de produção (OP) mas já existir entradas anteriores, o sistema validará sobre a quantidade restante:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img04.png
   :scale: 100% 
   :align: center 

| \

**BR One ::Não é possível adicionar a Entrada de PA, pois ultrapassa a Quantidade planejada da OP. Quantidade faltante: 1.**

Caso a Ordem de produção (OP) não possua nenhum componente com baixa por explosão e o PA administrado por lote, exibirá a seguinte mensagem:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img05.png
   :scale: 100% 
   :align: center 

| \

**BR One :: Não é possível realizar uma Entrada de PA sem antes realizar uma Saída de Insumos ou um Apontamento de Produção para a OP.**

Caso a Ordem de produção (OP) não possua nenhum componente com baixa por explosão e o PA não é administrado por lote, exibirá a seguinte mensagem:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img06.png
   :scale: 100% 
   :align: center 

| \

**BR One :: É necessário realizar pelo menos uma saída de insumos para essa OP antes de executar a reavaliação de estoque.**

- **Entrada de PA para Item administrado por lote ou série** 

Ao clicar em **Adicionar** e com o parâmetro **Obriga trocar os lotes/séries do produto retrabalhado** desmarcada, e considerando que o Produto Acabado (PA) que está sendo trabalhado naquele momento é administrado por lote/série, será aberta a seguinte tela:

- **Lote**

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img07.png
   :scale: 100% 
   :align: center 
   
- **Série**

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/a-img03.png
   :scale: 100% 
   :align: center 


| \

Antes de abrir a tela de **Entrada de mercadoria**,  as seguintes condições devem ser atendidas: A entrada de Produto acabado (PA) não seja do tipo refugo, o parâmetro **Obriga trocar os lotes/séries do produto retrabalhado** está marcado ou a resposta na tela anterior é **Sim**, o item é administrado por lote/série, e a soma das quantidades alocadas nas Ordens de produção (OPs) vinculadas é maior ou igual a quantidade na entrada de produto acabado (PA), e a quantidade da entrada de PA é menor que a soma dos lotes/séries disponíveis.


- **Lote**

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img08.png
   :scale: 80% 
   :align: center 
   
   
- **Série**

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/a-img04.png
   :scale: 80% 
   :align: center    

| \

Na tela **BR One :: Seleção do nº de lote/série**, deve ser escolhido o lote/série que será utilizado na saída de mercadorias que será criada ao inserir a **Entrada de mercadoria**. Esse lote/série escolhido será o lote/série entrado na entrada de PA da OP vinculada à OP de retrabalho.

Após selecionar o lote ou série, basta clicar em **Adicionar** na tela **BR One :: Entrada de PA**, que a tela **Entrada de mercadoria** será aberta:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img09.png
   :scale: 100% 
   :align: center 

| \

Essa tela não poderá ser fechada ou cancelada antes de adicionar a entrada. Caso o usuário tente fechar ou cancelar, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img10.png
   :scale: 100% 
   :align: center 

| \

**BR One :: Não é possível fechar a tela sem inserir a entrada de mercadoria.**

Ao clicar em **Adicionar**, a tela de definição de lotes/séries será aberta:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img11.png
   :scale: 90% 
   :align: center 

| \

Nessa tela, será criado o lote/série que será utilizado na entrada de mercadoria. Caso a configuração de gerar lote/série automaticamente esteja ativa, basta clicar no botão **Carregar lote** para o lote/série ser carregado.

Após criar o lote/série, clique em **OK** e insira a **Entrada de mercadoria**.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img12.png
   :scale: 80% 
   :align: center 

| \

Será criada uma **Entrada de mercadoria** com o item da Entrada de PA e, com esse mesmo item, será criada também uma **Saída de mercadorias** para os componentes com baixa por explosão e uma saída para o item pai da OP.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img13.png
   :scale: 80% 
   :align: center 

| \

- **Entrada de PA para item não administrado por lote/série**

Para item que não é administrado por lote/série, pode ser consultado o seu processo de entrada de PA diretamente no tópico de **Transferência de estoque**.

Se o usuário tentar fazer uma entrada de PA com quantidade maior que a planejada na OP, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img03.png
   :scale: 100% 
   :align: center 

| \

**BR One :: Não é permitido apontar uma quantidade de produto acabado maior que a quantidade planejada na OP de retrabalho.**

Caso o usuário tente inserir uma entrada de PA sem realizar uma saída de insumos para a OP, a seguinte mensagem será exibida: 

*BR One :: É necessário realizar pelo menos uma saída de insumos para essa OP antes de executar a reavaliação de estoque*.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img06.png
   :scale: 100% 
   :align: center 

| \

- **Entrada de PA na OP de Retrabalho com quantidade sobressalente**

Para realizar uma entrada de PA com uma quantidade sobressalente para uma OP de Retrabalho, o parâmetro **% desvio da quantidade planejada da OP de retrabalho** deve estar marcado e com um desvio configurado.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img14.png
   :scale: 100% 
   :align: center 

| \

Com o parâmetro devidamente configurado, ao realizar a entrada de PA com as quantidades sobressalentes (desvio), o add-on irá realizar uma entrada de mercadoria para todas as quantidades que não foram planejadas na OP. 

**Exemplo:**

Em uma OP, onde a quantidade planejada são **10 peças**, e o parâmetro está configurado como **50%**, é possível realizar uma entrada de **15 peças**, onde **10 são planejadas**, portanto, seguem o fluxo normal do BR One, e **5 peças** são sobressalentes, onde o add-on irá gerar uma entrada de mercadoria para essa quantidade.

No exemplo da OP abaixo, foi feita uma entrada de PA de **15 peças**, e o add-on teve justamente o comportamento indicado acima.

- 10 peças planejadas, geraram uma reavaliação de estoque (pois não houve troca de lote).
- 05 peças sobressalentes, geraram uma entrada de mercadoria.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img15.png
   :scale: 70% 
   :align: center 

| \

**Obs.:** Não houve alteração no processo de saída de insumos, se a OP possui componentes com baixa por explosão, as entradas de quantidades sobressalentes irão abater a quantidade conforme configurado na OP, se os componentes são de baixa manual, a saída deve ocorrer manualmente.

Independentemente de quantas entradas sejam realizadas, o add-on irá identificar o que é quantidade sobressalente e irá realizar uma entrada de mercadoria para essa quantidade.

A fim de facilitar a identificação das entradas de PA de quantidade sobressalentes, todas as entradas de mercadoria, que forem provenientes do desvio configurado, terão uma mensagem específica no campo **Observações**, **Observação do diário** e estarão preenchidas como **Não** no campo **Qtde. Planejada OP Retrabalho**.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img16.png
   :scale: 100% 
   :align: center 

| \

- **Entrada de PA na OP de Retrabalho sem componentes**

Para realizar uma entrada de PA sem componentes para uma OP de Retrabalho, é necessário que o parâmetro **Utilizar GGF arbitrado** esteja ativo, e que os recursos tenham um tempo planejado na OP e um custo hora em seu cadastro.

Caso usuário tente adicionar uma OP de Retrabalho sem componentes e o recurso não possua cadastrado nenhum custo hora, o add-on irá retornar a seguinte mensagem:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img17.png
   :scale: 100% 
   :align: center 

| \

**BR One :: Insira um custo hora no recurso ou no grupo do recurso para continuar.**

Caso usuário tente adicionar uma OP de Retrabalho sem componentes e o recurso não tenha tempo planejado, o add-on irá retornar a seguinte mensagem:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img18.png
   :scale: 100%
   :align: center 

| \

**BR One :: A coluna 'Tempo planejado' da linha com custo hora deve ser maior que zero.**

Caso usuário tente realizar a entrada de PA para OPs de retrabalho que não possuem componentes no grid, utilizando o add-on, e essa OP não possui tempo planejado, deve ser retornado a seguinte mensagem em vermelho no rodapé:

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img19.png
   :scale: 100%
   :align: center 

| \

**BR One :: Não é possível realizar a Entrada de PA na OP de Retrabalho, pois o GGF arbitrado não está ativo ou não há tempo planejado nos recursos da OP.'**

Com todas as configurações corretas, a entrada de PA na OP de Retrabalho sem componentes, deve ser realizada normalmente,

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img20.png
   :scale: 80%
   :align: center 

| \

Observa-se que o custo unitário do PA, será referente ao custo do **GGF** gerado na entrada. 

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Entrada\ de\ PA\ Retrabalho/img21.png
   :scale: 60%
   :align: center 

| \
