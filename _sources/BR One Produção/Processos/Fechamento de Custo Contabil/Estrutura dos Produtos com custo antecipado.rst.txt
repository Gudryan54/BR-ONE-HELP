==================================================
Estrutura dos Produtos com custo antecipado
==================================================

.. note::

   Para uma melhor visualização das imagens, abra-as em outra guia.
   
- **‘PA_ARB_Nivel-01_001’** consome **‘SA_ARB_Nivel-02_001’** que consome **‘item nenhum’** e custo de hora máquina (antecipado).

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/06.png
   :scale: 60%
   :align: center

| \ 

- **‘PA_ARB_Nivel-01_002’** consome **‘SA_ARB_Nivel-02_001’** que consome **‘item nenhum’** e custo de hora máquina (antecipado).

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/07.png
   :scale: 60%
   :align: center

| \ 

- **‘PA_ARB_Nivel-01_003’** consome **‘SA_ARB_Nivel-02_001’** que consome **‘item nenhum’** e custo de hora máquina (antecipado).
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/08.png
   :scale: 60%
   :align: center

| \ 

Agora, vamos analisar as movimentações apenas do item **‘SA_ARB_Nivel-02_001’**, para isso devemos entrar no cadastro do item e abrir o **‘Relatório de verificação do estoque’**:

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/09.png
   :scale: 60%
   :align: center

| \ 

Portanto, ao analisar as movimentações dentro do mês de maio/24, observamos que houve uma produção do item de 500 peças, devido às entradas de mercadorias vinculadas nas OPs (‘EM 1196’, ‘EM 1198’) e uma entrada proveniente de um estorno de produção (‘EM 1200’).

Observa-se também que o custo do item foi reavaliado em “-200,00” (‘MR 583’) e que houve consumo do item através das saídas de mercadorias (‘SO 1333’, ‘SO 1334’, ‘SO 1335’) a ‘SO 1339’ não é considerada não possui vinculo com uma OP ela é referente ao estorno da entrada ‘EM 1200’. 

Ainda dentro do mês houve duas vendas totalizando 30 peças (‘NS 124’ e ‘NS 125’) e duas transferências de estoque (‘TF 1161’ e ‘TF 1162’).

Com as informações dispostas da tela relatório acima, é possível realizar manualmente a memória de cálculo para o item e por assim, validar se os valores considerados no fechamento estão corretos. 

Segue abaixo exemplo de memória de cálculo para o item **‘SA_ARB_Nivel-02_001’**:

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/10.png
   :scale: 60%
   :align: center

| \ 

Logo para o item **‘SA_ARB_Nivel-02_001’** o fechamento de custo irá observar:

- As movimentações que incluem produções, reavaliações, vendas e transferências.
- O custo final por unidade, que reflete a produção, custos adicionais e ajustes de reavaliação.

Para o nosso exemplo foi cadastrado um GGF com rateio de ‘Horas máquina’ e um valor de 5.000,00:

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/11.png
   :scale: 70%
   :align: center

| \

Portanto, ao simular o fechamento do mês, temos o seguinte retorno:

Aba ‘Resultado”:
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/12.png
   :scale: 60%
   :align: center

| \ 

Aba ‘LCM e reavaliações’:
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/13.png
   :scale: 60%
   :align: center

| \ 

Ao analisar a simulação do fechamento de custo, vemos na aba ‘Resultado’ que foi rateado um valor de 4.999,00 para o item **‘SA_ARB_Nivel-02_001’** na OP 756:

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/14.png
   :scale: 70%
   :align: center

| \ 

Portanto ao verificarmos os lançamentos da aba ‘LCM e Reavaliações’, temos na primeira linha que é o lançamento do antecipado, onde é realizado um débito na conta de ‘GGF antecipado’ que é configurada na aba ‘Custos’ da tela ‘Configurações de produção’:

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/15.png
   :scale: 60%
   :align: center

| \ 

O valor do lançamento do antecipado (cuja 'Observação' é ‘Total antecipado’) é a soma de todos os LCMs de antecipado no mês do fechamento referente as OPs que estão na aba ‘Resultado’, em nosso exemplo,  os LCMs do antecipado são todos da OP 756:
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/16.png
   :scale: 70%
   :align: center

| \ 

Na segunda linha temos o lançamento da temporária, que pega o valor do cadastro do GGF e faz um débito na ‘Conta de alocação temporária de custos’ (alocação), que é configurada na aba ‘Custos’ da tela ‘Configurações de produção’:
  
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/17.png
   :scale: 60%
   :align: center

| \ 

Na terceira linha do fechamento é realizado um débito na conta de WIP do depósito 01, este lançamento ocorre, pois, houve consumo do item **‘SA_ARB_Nivel-02_001’** no depósito 01 dentro do mês do fechamento (‘SO 1333’, ‘SO 1334’, ‘SO 1335’):

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/18.png
   :scale: 60%
   :align: center

| \ 

Obs.: A conta WIP (Work in Progress) trata-se de uma conta utilizada para registrar os custos associados a produtos que estão em processo de fabricação, mas que ainda não foram concluídos, a memória de cálculo se inicia no nível mais baixo do item e seus valores são agregados de nível à nível até o primeiro nível.

Comparando com a memória de cálculo realizada, podemos ver que são os mesmos valores, logo, o valor rateado no fechamento de custo está correto: 
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/19.png
   :scale: 60%
   :align: center

| \ 

Obs.: Os valores na memória de cálculo ficam negativos, pois no relatório de verificação de estoque, ele indica a saída desse montante do depósito (conta: 4.01.01.05.11).

Na quarta e quinta linha do fechamento temos dois lançamentos um para o depósito 01 e outro para o depósito 02, onde é feito um débito para a conta de CPV, esse lançamento é referente a venda realizada do **‘SA_ARB_Nivel-02_001’** dentro do período de fechamento (NS 124 e NS 125):
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/20.png
   :scale: 60%
   :align: center

| \ 

Se compararmos os valores levados no fechamento de custo para o item com a memória de cálculo acima, podemos verificar que, os valores levados para a CPV nos dois depósitos são iguais ao rateados no fechamento, logo o rateio no fechamento também está correto. 
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/21.png
   :scale: 60%
   :align: center

| \ 

Obs.: Os valores na memória de cálculo ficam negativos, pois no relatório de verificação de estoque, ele indica a saída desse montante do depósito (conta: 4.01.01.05.11).

Para a sexta e sétima linha, foram realizadas duas reavaliações referentes às quantidades disponíveis em estoque no último dia do mês do item **‘SA_ARB_Nivel-02_001’** para os depósitos 01 e 02:

.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/22.png
   :scale: 60%
   :align: center

| \ 

Realizando o cálculo da diferença entre o custo adicional e a soma dos LCMs, temos os valores das reavaliações de estoque realizados pelo fechamento de custo, respectivamente, para os depósitos 01 e 02:
 
.. image:: /_static/BR\ One\ Produção/Processo/Fechamento\ de\ Custo\ Contabil/Memoria\ Calculo/23.png
   :scale: 90%
   :align: center

| \ 