=======================
Etapa 2
=======================

Na **Etapa 2** são configurados o horizonte de planejamento e as preferências de exibição da execução do MRP.

------------------
Data inicial
------------------

A **'Data inicial'** representa o ponto inicial a partir do qual o sistema começa a calcular as necessidades de materiais. Todas as fontes de demanda e fornecimento que possuírem as datas de entrega para antes dessa data são consideradas históricas e não são incluídas nos cálculos do MRP.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/01.png
   :scale: 80%
   :align: center

| \

A **'Data inicial'** deve ser menor ou igual a data atual, caso seja informado uma data maior do que a data atual, o add-on irá retornar a seguinte validação: 

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/02.png
   :scale: 120%
   :align: center

**BR One :: Data inicial deve ser menor ou igual a data atual.**

Ao definir a **'Data inicial'** com a data de 27/12/2023 e selecionar uma fonte de demanda, ao executar o MRP, será retornado apenas as demandas que estejam com a data de entrega dentro período escolhido. Em nosso exemplo, temos o pedido de venda 98, que teve sua demanda calculada e recomendada pelo MRP.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/03.png
   :scale: 80%
   :align: center

| \

Caso a data do pedido de venda 98, fosse anterior a data informada no campo **'Data inicial'**, essa demanda não seria recomendada no MRP, pois o mesmo está fora do horizonte de planejamento selecionado.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/04.png
   :scale: 80%
   :align: center

| \

--------------
Data final
--------------

A **‘Data final’** define a última data considerada no cálculo do MRP. Todas as fontes de demanda e fornecimento que possuírem as datas superiores à essa data não são incluídas nos cálculos do MRP.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/05.png
   :scale: 80%
   :align: center

| \

A **‘Data final’** não pode ser superior a 36 meses da data de execução, caso seja informado uma data superior, o add-on irá validar e exibirá a mensagem:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/06.png
   :scale: 120%
   :align: center

**BR One :: A diferença máxima entre data de execução e data final permitida é de 36 meses.**

Ao definir a **‘Data final’** com a data de 30/01/2024, selecionar as fontes de demanda e fornecimento, e executar o MRP, será retornado apenas as demandas que estejam com a data de entrega dentro período escolhido. Em nosso exemplo, temos o pedido de venda 98, que teve sua demanda calculada e recomendada pelo MRP.
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/07.png
   :scale: 80%
   :align: center

| \ 

Caso a data do pedido de venda 98, seja maior que a **‘Data final’**, essa demanda não será recomendada no MRP, pois a mesma está fora do horizonte de planejamento selecionado. 

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/08.png
   :scale: 80%
   :align: center

| \

---------------------------------
Visualizar dados em período de:
---------------------------------

Este parâmetro permite escolher a forma de visualizar os dados, é possível escolher entre três opções:

- Dias
- Semanas
- Meses

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/09.png
   :scale: 100%
   :align: center

| \

A escolha das parametrizações acima, altera a forma como os dados calculados pelo MRP serão demonstrados na aba **‘Resultado’** da tela do **‘Assistente de MRP’**, segue abaixo exemplo de cada uma das exibições: 

Visualizar dados em período de: **DIAS**

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/10.png
   :scale: 60%
   :align: center

| \

Visualizar dados em período de: **SEMANAS**

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/11.png
   :scale: 60%
   :align: center

| \
 
Visualizar dados em período de: **MESES**

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/12.png
   :scale: 60%
   :align: center

| \

---------------------------
Comprimento do Horizonte:
---------------------------

Este campo demonstra o comprimento do horizonte conforme o tipo de visualização escolhida no parâmetro **‘Visualizar dados em período de’**, onde o mesmo pode ser definido como:

- Dias
- Semanas
- Meses

Segue abaixo exemplo de cada uma das exibições, conforme configuração escolhida:

Comprimento do horizonte: **DIAS**

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/13.png
   :scale: 80%
   :align: center

| \

Comprimento do horizonte: **SEMANAS**

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/14.png
   :scale: 80%
   :align: center

| \
 
Comprimento do horizonte: **MESES**

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/15.png
   :scale: 80%
   :align: center

| \
 
--------------------------------
Exibir itens sem necessidade:
--------------------------------

A flag **‘Exibir itens sem necessidade’** tem como objetivo exibir os itens que não possuem necessidade de fornecimento, isto é, itens em estoque que atendem à demanda. Caso selecionado, esses itens aparecerão na aba **'Resultado'** somente.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/16.png
   :scale: 70%
   :align: center

| \

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/17.png
   :scale: 70%
   :align: center

| \

-------------------------
Filtrar recomendações:
-------------------------

No parâmetro ‘Filtrar recomendações’, o add-on permite realizar os filtros de três formas:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/18.png
   :scale: 100%
   :align: center

| \
 
- **Exibir todas**

Tanto as recomendações de **‘Solicitação de compra’** como a **‘Ordem de produção’** aparecerão;

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/19.png
   :scale: 80%
   :align: center

| \

- **Documentos de compra:**

Traz apenas os itens que são sugeridos nas solicitações de compra. Se a flag **‘Exibir itens sem necessidade’** estiver marcada, traz também os itens sem necessidade cujo método de planejamento seja **‘Comprar’**.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/20.png
   :scale: 80%
   :align: center

| \

- **Ordem de produção:**

Traz apenas os itens que são sugeridos nas ordens de produção. Se a flag **‘Exibir itens sem necessidade’** estiver marcada, traz também os itens sem necessidade cujo método de planejamento seja **‘Produzir’**.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/21.png
   :scale: 80%
   :align: center

| \

------------------
Grupo de itens:
------------------

O parâmetro **‘Grupo de itens’**, permite realizar o filtro de acordo com o grupo de itens selecionado. Com isso o MRP irá considerar em suas recomendações apenas os itens que fazer parte do **‘Grupo de itens’** selecionado.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/22.png
   :scale: 80%
   :align: center

| \

---------------
Fabricantes:
---------------

O parâmetro **‘Fabricante’**, permite realizar o filtro de acordo com o fabricante selecionado. Ao clicar no botão **‘[…]’**, a tela **‘Fabricante’** será aberta e nela poderão ser selecionados os fabricantes para filtrar os resultados para os itens de compra e produção.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/23.png
   :scale: 75%
   :align: center

| \ 

Considerando o exemplo acima, existem dois fabricantes cadastrados que podem ser selecionados, levando em conta o pedido de venda número 100, há dois itens que possuem fabricantes diferentes, conforme demonstra imagem abaixo:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/24.png
   :scale: 50%
   :align: center

| \ 
 
Ao rodar o MRP sem filtrar nenhum fabricante, o MRP irá considerar em seus cálculos todos os itens que possuam demanda, conforme imagem abaixo: 

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/25.png
   :scale: 75%
   :align: center

| \ 
 
Entretanto, caso seja filtrado um fabricante, o MRP irá recomendar apenas os itens que possuam esse fabricante cadastrado:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/26.png
   :scale: 75%
   :align: center

| \

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/27.png
   :scale: 75%
   :align: center

| \ 
 
---------------
Fornecedores:
---------------

O parâmetro **‘Fornecedores’**, permite realizar o filtro de acordo com os fornecedores selecionados. Ao clicar no botão **‘[…]’**, a tela **‘Fornecedores’** será aberta e nela poderão ser selecionados fornecedores para filtrar os resultados para os itens de compra.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/28.png
   :scale: 80%
   :align: center

| \ 
 
 
Ao filtrar os fornecedores desejados, o MRP irá calcular e recomendar apenas os itens que possuam o campo **‘Fornecedor preferencial’** ou da tela **‘Fornecedores preferidos’** da tela de **‘Cadastro do item’** igual ao selecionado na etapa 2 do Assistente de MRP. 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/29.png
   :scale: 50%
   :align: center

| \ 
 

O item **‘Comp01_MRP’**, não possui nenhum fornecedor preferencial ou preferido cadastrado.
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/30.png
   :scale: 80%
   :align: center

| \ 
 

Ao executar o Assistente de MRP determinando alguns fornecedores no filtro de **‘Fornecedores’**, o resultado do MRP não irá trazer nenhuma recomendação de compra para o item **‘Comp01_MRP’**, mesmo ele fazendo parte do roteiro dos itens a serem produzidos.
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/31.png
   :scale: 80%
   :align: center

| \

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/32.png
   :scale: 80%
   :align: center

| \ 
 
-----------------------
Data de vencimento:
-----------------------

No parâmetro **‘Data de vencimento’**, quando marcado, pode ser escolhido um período de datas para filtrar por data de vencimento dos documentos.


.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/33.png
   :scale: 120%
   :align: center

| \ 
 
-------------------------
Data de liberação:
-------------------------

No parâmetro **‘Data de liberação’**, quando marcado, pode ser escolhido um período de datas para filtrar por data de liberação dos documentos.

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/34.png
   :scale: 120%
   :align: center

| \

-------------------------
Ordenar recomendações:
-------------------------

O parâmetro **‘Ordenar recomendações’** tem a função de ordenar os itens da aba **‘Recomendações’**, após a execução do MRP. As recomendações podem ser ordenadas conforme abaixo, onde todas as ordenações são agrupadas pelo **‘Tipo de pedido’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/35.png
   :scale: 100%
   :align: center

| \
 
Exemplo de ordenação por **‘Nº do item’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/36.png
   :scale: 80%
   :align: center

| \

Exemplo de ordenação por **‘Data de vencimento’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/37.png
   :scale: 80%
   :align: center

| \ 

Exemplo de ordenação por **‘Data de liberação’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/38.png
   :scale: 80%
   :align: center

| \ 

Exemplo de ordenação por **‘Nº do item pai’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/39.png
   :scale: 80%
   :align: center

| \ 

Exemplo de ordenação por **‘LeadTime’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/40.png
   :scale: 80%
   :align: center

| \ 

Exemplo de ordenação por **‘Exceção’**:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Etapa\ 2/41.png
   :scale: 80%
   :align: center

| \


 
