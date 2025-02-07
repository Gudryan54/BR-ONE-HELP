=======================
Combinações MRP
=======================

É possível realizar diversas combinações entre todas as configurações e parâmetros existentes no MRP, segue abaixo alguns exemplos práticos dessas combinações.

---------------------------------------
Combinações de quantidade
---------------------------------------

Segue abaixo exemplos de combinações que alteram as quantidades das recomendações realizadas pelo MRP.

- **Solicitar múltiplos + Lote Máximo**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Solicitar múltiplos'** e **'Lote máximo'**.

O item de produção **'PA01_MRP'** possui uma configuração de múltiplo de 8 peças, assim como uma configuração de lote máximo de 80 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/01.png
   :scale: 90%
   :align: center

| \

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/02.png
   :scale: 90%
   :align: center

| \

Em seu roteiro há também o item de compra **'Comp01_MRP'**, que possui um múltiplo de 2 peças,  um lote máximo configurado de 80 peças e uma configuração de quantidade mínima do pedido de 22 peças:

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/03.png
   :scale: 90%
   :align: center

| \

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/04.png
   :scale: 100%
   :align: center

| \

Ao executar o MRP, o add-on trará as seguintes recomendações: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/05.png
   :scale: 80%
   :align: center

| \

Ao analisar as recomendações do MRP: 

**Para o item de produção PA01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/06.png
   :scale: 100%
   :align: center

| \

O MRP recomendou a criação de 2 Ordens de Produção, que respeitam a configuração de lote máximo (80 peças) e de múltiplo (8 peças) onde as linhas 6 e 7 são referentes a demanda de previsão de venda (100 peças), que devido as combinações de configuração, totalizam 104 peças. 

**Para o item de compra Comp01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/07.png
   :scale: 100%
   :align: center

| \

O MRP recomendou 2 solicitações de compra, que respeitam a configuração de lote máximo (80 peças), e de múltiplo (2 peças), onde as linhas 2 e 3 são recomendações referentes a demanda de 100 peças do **'PA01_MRP'**, devido as combinações de configuração, a quantidade recomendada de compra é de 104 peças. 

- **Solicitar múltiplos + Lote Máximo + Quantidade mínima do pedido**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Solicitar múltiplos'**, **'Lote máximo'** e **'Quantidade mínima do pedido'**.

O item de produção **'PA01_MRP'** possui uma configuração de múltiplo de 8 peças, assim como uma configuração de lote máximo de 80 peças e uma configuração de quantidade mínima do pedido de 24 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/08.png
   :scale: 90%
   :align: center

| \
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/09.png
   :scale: 90%
   :align: center

| \

Em seu roteiro há também o item de compra **'Comp01_MRP'**, que possui um múltiplo de 2 peças,  um lote máximo configurado de 80 peças e uma configuração de quantidade mínima do pedido de 28 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/10.png
   :scale: 90%
   :align: center

| \

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/11.png
   :scale: 100%
   :align: center

| \

Ao executar o MRP, o add-on trará as seguintes recomendações: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/12.png
   :scale: 80%
   :align: center

| \

Ao analisar as recomendações do MRP: 

**Para o item de produção PA01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/13.png
   :scale: 100%
   :align: center

| \

O MRP recomendou a criação de 2 Ordens de Produção, que respeitam a configuração de lote máximo (80 peças), de múltiplo (8 peças) e quantidade mínima do pedido (24 peças), onde as linhas 6 e 7 são referentes a demanda de previsão de venda (100 peças), que devido as combinações de configuração, totalizam 104 peças. 

**Para o item de compra Comp01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/14.png
   :scale: 100%
   :align: center

| \

O MRP recomendou 2 solicitações de compra, que respeitam a configuração de lote máximo (80 peças), de múltiplo (2 peças) e a quantidade mínima do pedido (28 peças), onde as linhas 2 e 3 são recomendações referentes a demanda de 100 peças do **'PA01_MRP'**, devido as combinações de configuração, a quantidade recomendada de compra é de 108 peças, onde as 4 peças a mais para o componente em relação ao PA é referente a configuração de quantidade mínima de pedido do mesmo, que é superior ao do PA.

- **Solicitar múltiplos + Lote Máximo + Quantidade mínima do pedido + Estoque mínimo**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Solicitar múltiplos'**, **'Lote máximo'** e **'Quantidade mínima do pedido'**.

O item de produção **'PA01_MRP'** possui uma configuração de múltiplo de 8 peças, assim como uma configuração de lote máximo de 80 peças e uma configuração de quantidade mínima do pedido de 24 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/15.png
   :scale: 90%
   :align: center

| \

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/16.png
   :scale: 90%
   :align: center

| \

Além de também possuir cadastrado um estoque mínimo de 16 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/17.png
   :scale: 90%
   :align: center

| \

Em seu roteiro há também o item de compra **'Comp01_MRP'**, que possui um múltiplo de 2 peças,  um lote máximo configurado de 80 peças e uma configuração de quantidade mínima do pedido de 22 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/18.png
   :scale: 90%
   :align: center

| \

E também possui cadastrado um estoque mínimo de 28 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/19.png
   :scale: 90%
   :align: center

| \

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/20.png
   :scale: 100%
   :align: center

| \

Ao executar o MRP, o add-on trará as seguintes recomendações: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/21.png
   :scale: 80%
   :align: center

| \ 

Ao analisar as recomendações do MRP: 

**Para o item de produção PA01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/22.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou a criação de 3 Ordens de Produção, que respeitam a configuração de lote máximo (80 peças), de múltiplo (8 peças) e quantidade mínima do pedido (24 peças), das três linhas recomendadas, nota-se que as linhas 14 e 15 são referentes a demanda de previsão de venda (100 peças), onde devido as combinações de configuração, totalizam 104 peças. 

A terceira recomendação, a linha 12, é referente a quantidade configurada de estoque mínimo (16 peças), entretanto o MRP recomenda 24 peças devido a configuração de quantidade mínima do pedido (24 peças).

**Para o item de compra Comp01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/23.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou 4 solicitações de compra, que respeitam a configuração de lote máximo (80 peças), de múltiplo (2 peças) e a quantidade mínima do pedido (22 peças), as linhas 6 e 7 são recomendações referentes a demanda de 100 peças do **'PA01_MRP'**, devido as combinações de configuração, a quantidade total é 104 peças. 

A a linha 2, é referente a quantidade configurada de estoque mínimo do PA, ou seja, o MRP recomendou a produção do estoque mínimo do PA e recomendou a compra dos componentes deste PA.

A linha 4 é referente a quantidade configurada de estoque mínimo do próprio componente.

- **Solicitar múltiplos + Lote Máximo + Quantidade mínima do pedido + Estoque máximo**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Solicitar múltiplos'**, **'Lote máximo'**, **'Quantidade mínima do pedido'** e **'Estoque máximo'**.

O item de produção **'PA01_MRP'** possui uma configuração de múltiplo de 8 peças, assim como uma configuração de lote máximo de 80 peças e uma configuração de quantidade mínima do pedido de 24 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/24.png
   :scale: 90%
   :align: center

| \ 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/25.png
   :scale: 90%
   :align: center

| \ 

Além de também possuir cadastrado um estoque máximo de 50 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/26.png
   :scale: 90%
   :align: center

| \ 

Em seu roteiro há também o item de compra **'Comp01_MRP'**, que possui um múltiplo de 2 peças,  um lote máximo configurado de 80 peças e uma configuração de quantidade mínima do pedido de 22 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/27.png
   :scale: 90%
   :align: center

| \ 

E também possui cadastrado um estoque máximo de 40 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/28.png
   :scale: 90%
   :align: center

| \ 

O **'PA01_MRP'** possui uma previsão de vendas de 150 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/29.png
   :scale: 100%
   :align: center

| \ 

Ao executar o MRP, o add-on trará as seguintes recomendações: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/30.png
   :scale: 80%
   :align: center

| \ 

Ao analisar as recomendações do MRP: 

**Para o item de produção PA01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/31.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou a criação de 3 Ordens de Produção, que respeitam a configuração de lote máximo (80 peças), de múltiplo (8 peças) e quantidade mínima do pedido (24 peças), das três linhas recomendadas, nota-se que as linhas 98 e 99 são referentes a demanda de previsão de venda (150 peças), onde devido as combinações de configuração, totalizam 152 peças. 

A terceira recomendação, a linha 102, é referente a quantidade configurada de estoque máximo (50 peças), entretanto o MRP recomenda apenas 48 peças devido a configuração de múltiplos (8 peças), porém, na linha 99 que é uma recomendação referente a previsão, “sobraram” 2 peças devido as configurações do item, com isso somando a “sobra” da linha 99 mais a recomendação da linha 102, temos as 50 peças referentes ao estoque máximo.

**Para o item de compra Comp01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/32.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou 4 solicitações de compra, que respeitam a configuração de lote máximo (80 peças), de múltiplo (2 peças) e a quantidade mínima do pedido (22 peças), as linhas 31 e 32 são recomendações referentes a demanda de 150 peças do **'PA01_MRP'**, devido as combinações de configuração, a quantidade total é 152 peças. 

A linha 34, é referente a quantidade configurada de estoque máximo do PA, ou seja, o MRP recomendou a produção do estoque máximo do PA e recomendou a compra dos componentes deste PA, pegando esta linha de recomendação e a “sobra” da linha 32, totalizam 50 peças. 

A linha 37 é referente a quantidade configurada de estoque máximo do próprio componente.

- **Solicitar múltiplos + Lote Máximo + % refugo**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Solicitar múltiplos'**, **'Lote máximo'**, e **'% refugo'**.

O item de produção **'PA01_MRP'** possui uma configuração de múltiplo de 8 peças, um lote máximo de 96 peças e **'% refugo'** de 10% :
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/33.png
   :scale: 90%
   :align: center

| \ 

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/34.png
   :scale: 100%
   :align: center

| \ 


Em seu roteiro há também o item de compra **'Comp01_MRP'**, que possui um múltiplo de 2 peças,  um lote máximo configurado de 80 peças.
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/35.png
   :scale: 90%
   :align: center

| \ 

Obs.: Não há configuração de porcentagem de refugo para itens de compra.

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/36.png
   :scale: 90%
   :align: center

| \ 

Ao executar o MRP, o add-on trará as seguintes recomendações: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/37.png
   :scale: 80%
   :align: center

| \ 

Ao analisar as recomendações do MRP: 

**Para o item de produção PA01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/38.png
   :scale: 100%
   :align: center

| \ 


O MRP recomendou a criação de 2 Ordens de Produção, que respeitam a configuração de lote máximo (96 peças), de múltiplo (8 peças) e a **'% de refugo'** (10%), na linha 65 está sendo considerado essa configuração que realiza um acréscimo na quantidade recomendada pelo MRP, totalizando assim 112 peças. As duas peças que “passaram” da quantidade de **'% refugo'** ocorreu devido ao múltiplo de 8 peças. 

**Para o item de compra Comp01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/39.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou 2 solicitações de compra para atender a demanda do PA,  onde foi respeitado as configurações de lote máximo (80 peças), de múltiplo (2 peças) e a quantidade mínima do pedido (22 peças), além de considerar a % de refugo (10%) existente no roteiro do PA, totalizando assim 112 peças.

- **Solicitar múltiplos + Lote Máximo + Quantidade mínima do pedido + % refugo**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Solicitar múltiplos'**, **'Lote máximo'**, **'Quantidade mínima do pedido'** e **'% refugo'**.

O item de produção **'PA01_MRP'** possui uma configuração de múltiplo de 8 peças, assim como uma configuração de quantidade mínima do pedido de 24 peças, um lote máximo de 80 peças e **'% refugo'** de 10% :
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/40.png
   :scale: 90%
   :align: center

| \ 

.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/41.png
   :scale: 90%
   :align: center

| \ 

Em seu roteiro há também o item de compra **'Comp01_MRP'**, que possui um múltiplo de 2 peças,  um lote máximo configurado de 80 peças e uma configuração de quantidade mínima do pedido de 22 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/42.png
   :scale: 90%
   :align: center

| \ 

Obs.: Não há configuração de porcentagem de refugo para itens de compra.

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/43.png
   :scale: 90%
   :align: center

| \ 

Ao executar o MRP, o add-on trará as seguintes recomendações: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/44.png
   :scale: 80%
   :align: center

| \

Ao analisar as recomendações do MRP: 

**Para o item de produção PA01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/45.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou a criação de 2 Ordens de Produção, que respeitam a configuração de lote máximo (80 peças), de múltiplo (8 peças) e quantidade mínima do pedido (24 peças), além de considerar a % de refugo (10%), na linha 65 está sendo considerado essa configuração que realiza um acréscimo na quantidade recomendada pelo MRP, totalizando assim 112 peças. As duas peças que “passaram” da quantidade de **'% refugo'** ocorreu devido ao múltiplo de 8 peças. 

**Para o item de compra Comp01_MRP:**
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/46.png
   :scale: 100%
   :align: center

| \ 

O MRP recomendou 2 solicitações de compra para atender a demanda do PA,  onde foi respeitado as configurações de lote máximo (80 peças), de múltiplo (2 peças) e a quantidade mínima do pedido (22 peças), além de considerar a % de refugo (10%) existente no roteiro do PA, totalizando assim 112 peças.

----------------------------
Combinações de leadtime
----------------------------

- **Leadtime + dias entre operações + calendário dias úteis**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Leadtime'**, **'Quantidade de dias entre as operações'** e utilizando um calendário de dias úteis.

O leadtime preferencial do PA está configurado como **'Sequencia de operações'**. 

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/47.png
   :scale: 90%
   :align: center

| \ 

O **'PA01_MRP'** possui o roteiro abaixo: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/48.png
   :scale: 80%
   :align: center

| \ 

Destacado estão as quantidades por recurso e o tempo variável por item em minutos, logo para se produzir uma unidade do **'PA01_MRP'**, a operação 10 leva 6 minutos enquanto a operação 20 leva 3,6 minutos.

A configuração de **'Quantidade de dias entre operações'** está configurada conforme print abaixo:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/49.png
   :scale: 100%
   :align: center

| \ 

Portanto, ao rodar o MRP temos o cenário abaixo: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/50.png
   :scale: 80%
   :align: center

| \ 

Onde a operação 10 tem inicio no dia 26/02/2024 e termina no dia 27/02/2024, totalizando um leadtime de 2 dias. 

Esse leadtime é diretamente influenciado pelo calendário utilizado, neste exemplo é utilizado um calendário de apenas dias úteis, com 8 horas diárias de trabalho, dessa forma o MRP realiza o seguinte cálculo para definir o prazo da operação 10: 

**600 min / 60 min = 10 horas**

Como o calendário possui apenas 8 horas de trabalho diário, o MRP calcula as 2 horas restantes para o dia seguinte, totalizando assim 2 dias de leadtime para essa operação.

Como a configuração de **'Quantidade de dias entre operações'** está configurada com o valor 3, portanto ele calcula 3 dias para iniciar a operação 20, iniciando e finalizando a mesma no dia 01/03/2024.

**360 min /60 min = 6 horas**

Conforme cálculo realizado pelo MRP, o prazo para finalizar a operação 20 é de 6 horas, com isso, se enquadra no tempo de trabalho estipulado no calendário, calculando assim um leadtime de 1 dia. 


- **Leadtime fixo + dias entre operações + calendário dias úteis + parâmetro considerar fixo independente do calculado**

Segue abaixo exemplo de recomendação de MRP onde há combinação entre as configurações **'Leadtime'**, **'Quantidade de dias entre as operações'**, **'Considerar Lead Time fixo independente do calculado'** e utilizando um calendário de dias úteis.

O leadtime preferencial do PA está configurado como **'Fixo em dias'**. 

O **'PA01_MRP'** possui uma previsão de vendas de 100 peças:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/51.png
   :scale: 100%
   :align: center

| \ 

O **'PA01_MRP'** possui o roteiro abaixo: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/52.png
   :scale: 80%
   :align: center

| \ 

Destacado estão as quantidades por recurso e o tempo variável por item em minutos, logo para se produzir uma unidade do **'PA01_MRP'**, a operação 10 leva 6 minutos enquanto a operação 20 leva 3,6 minutos.

Existe também configurado as configurações abaixo:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/54.png
   :scale: 90%
   :align: center

| \ 

Portanto, ao rodar o MRP temos o cenário abaixo: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/55.png
   :scale: 80%
   :align: center

| \ 

Como a configuração de leadtime preferencial está como **'Fixo em dias'** e o parâmetro **'Considerar Lead Time fixo independente do calculado'** está marcado, o MRP recomenda como leadtime exatamente o que está configurado no campo leadtime do PA.
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/56.png
   :scale: 80%
   :align: center

| \

----------------------------
Combinações de documentos
----------------------------

É possível realizar combinações entre os tipos de documentos, segue abaixo alguns exemplos de combinações: 

- **Demanda + fornecimento**

Combinação de demanda e fornecimento, segue exemplo, onde temos um pedido de venda de quantidade de 1.000 peças, e uma ordem de produção no sistema de 300 peças.

Pedido de venda: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/57.png
   :scale: 80%
   :align: center

| \

Ordem de produção: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/58.png
   :scale: 80%
   :align: center

| \

Na tela do Assistente de MRP vamos selecionar as fontes de demanda **'Pedido de venda'** e **'Ordem de produção'**:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/59.png
   :scale: 80%
   :align: center

| \

Ao executar o MRP, os documentos das fontes de demanda selecionados que estejam dentro do horizonte de planejamento e dos depósitos configurados, serão recomendados, em nosso exemplo o MRP irá recomendar a quantidade faltante referente ao pedido de venda, pois como a demanda **'Ordem de produção'** está marcada, o mesmo está considerando a quantidade da OP 749, segue resultado:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/60.png
   :scale: 80%
   :align: center

| \

- **Demanda + estoque**

Combinação de demanda e estoque, segue exemplo, onde temos uma previsão de venda de quantidade de 100 peças, e 50 peças em estoque.

Previsão de venda:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/61.png
   :scale: 80%
   :align: center

| \

Quantidade em estoque: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/62.png
   :scale: 80%
   :align: center

| \

Na tela do Assistente de MRP vamos selecionar apenas a previsão criada **'Prev-2024'**:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/63.png
   :scale: 80%
   :align: center

| \

Ao executar o MRP, será considerado a previsão selecionada e as quantidades disponíveis em estoque, em nosso exemplo o MRP irá recomendar a quantidade faltante referente a previsão, recomendando assim uma **'Ordem de produção'** para o PA e uma solicitação de compra para o componente, segue resultado:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/64.png
   :scale: 80%
   :align: center

| \

- **Demanda + fornecimento + estoque**

Combinação de demanda, fornecimento e estoque, para este exemplo vamos analisar o componente **'Comp02_MRP'**, onde temos um pedido de venda de 100 peças para o **'PA02_MRP'**, um pedido de compra de 50 peças e um estoque de 20 peças para o **'Comp02_MRP'**. 

Pedido de venda:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/65.png
   :scale: 80%
   :align: center

| \

Pedido de compra:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/66.png
   :scale: 80%
   :align: center

| \

Quantidade em estoque:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/67.png
   :scale: 80%
   :align: center

| \

Segue abaixo o roteiro do **'PA02_MRP'**, onde para cada item produzido, é utilizado 1 unidade do componente **'Comp02_MRP'**: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/68.png
   :scale: 80%
   :align: center

| \

Na tela do Assistente de MRP vamos selecionar as fontes de demanda **'Pedido de compra'** e **'Pedido de venda'**: 
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/69.png
   :scale: 80%
   :align: center

| \

Ao executar o MRP, será considerado os documentos de demanda selecionados, junto a suas quantidades disponíveis em estoque:
 
.. image:: /_static/BR\ One\ Produção/Processo/MRP/Combinações\ MRP/70.png
   :scale: 80%
   :align: center

| \

Ao analisar as recomendações do MRP, vemos que para o **'PA02_MRP'**, foi recomendada a produção de 100 peças (linha 17), para atender ao pedido de venda de número 100. 

Já para o componente **'Comp02_MRP'**, o MRP considera a quantidade disponível em estoque (20 peças) e o pedido de compra de número 146 (50 peças), logo é recomendado a solicitação de compra de apenas 30 peças (linha 8) para atender a demanda do pedido de venda de número 100.



