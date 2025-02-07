Ordem de Produção - Beneficiamento de compra
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Detalhamento dos campos e cálculos utilizados na aba custo da Ordem de Beneficiamento de Compra.

Para exemplificar o processo de produção, vamos utilizar uma Ordem de Produção (OP) beneficiamento de compra com uma quantidade planejada de 10 unidades. 

Seu roteiro é composto por 2 componentes, sendo que a quantidade base de cada um deles é de 1 unidade e quantidade fixa é 0. E também composto por um item de serviço, sendo que a quantidade base é 01.

Para encontrar **quantidade planejada** de cada item:

**Quantidade planejada** = Quantidade base \* quantidade planejada do cabeçalho da OP + quantidade fixo

Para encontrar o **tempo planejado** de cada recurso:

**Tempo planejado** = Tempo variável \* quantidade planejada do cabeçalho da OP + tempo fixo  

**Custos dos componentes utilizados:**

- Item I009  - R$ 2,50

- Item I010 – R$ 3,00	

- Item-Serviço – R$ 12,00


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img01.png
   :scale: 100%

Iremos passar pelos campos da aba Custo

**1. Custo não alocado**

São listados os valores de custo alocado no fechamento de custo, caso a OP não tenha entrada de PA no mês do apontamento de horas.

**2. Custo componentes**

Na tela **"BR One :: Detalhe custo de componentes" [...]**, são listados todos os documentos gerados como:

- Saída de insumos;
- Saída de insumos com flag refugo marcada; 
- Apontamento de refugo com retorno do componente.

O sistema recupera o custo unitário de cada item que será realizado o documento e multiplica pela quantidade, gerando assim o custo total.

Na Saída de insumos realizada para o **item I009** de 08 unidades com o custo unitário de R$ 2,50, resultando em um custo total de **R$ 20,00**. Já o **item** **I010** de 08 unidades com o custo unitário de R$ 3,00, totalizando um custo de **R$ 24,00**. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img02.png
   :scale: 100%

Nesse cenário também houve saída de insumo com a flag refugo marcada na quantidade de 1 PA. O **item I009** de 01 unidades com o custo unitário de R$ 2,50, resultando em um custo total de **R$ 2,50**. Já o **item** **I010** de 01 unidades com o custo unitário de R$ 3,00, totalizando um custo de **R$ 3,00**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img03.png
   :scale: 100%

Dessa forma, o custo dos componentes é a soma da coluna de custo total dos detalhes, sendo **R$ 49,50**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img04.png
   :scale: 100%


**3. Custo atual do PA**

Na tela **"BR One :: Detalhe custo atual do PA"**, são listados todos os documentos gerados como:

- Entrada de PA
- Reavaliação do estoque

Na entrada de PA é recuperado o custo dos insumos para produção de 1 PA. E é realizado uma reavaliação do estoque com o valor do Rateio de custos de terceiros.

O custo dos componentes nesse cenário é de R$ 5,50, o total do PA será de R$ 5,50.

O sistema recupera o custo unitário do PA que será realizado o documento e multiplica pela quantidade, gerando assim o custo total.

Realizada entrada do PA de 08 unidades com o custo unitário de R$ 5,50, resultando em um custo total de **R$ 44,00.**

O valor da reavaliação do estoque foi de R$ **75,30**, que será acrescentado ao custo do PA. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img05.png
   :scale: 100%

Dessa forma, o custo atual do PA é a soma da coluna de custo total dos detalhes, sendo **R$ 119,30**.


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img06.png
   :scale: 100%

**4. Rateios de custo de terceiros**

Exibe os documentos que deram origem ao valor do rateio de custos de terceiros.

**Valor total da linha (Rateio de custos de terceiros)** = Valor total da nota – valor total do imposto

**Valor total da linha (Rateio de custos de terceiros)** = R$ 120,00 – R$ 44,70

**Valor total da linha (Rateio de custos de terceiros)** = R$ 75,30

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img07.png
   :scale: 100%

**Valor unitário** = Valor total da linha (Rateio de custos de terceiros) / Quantidade na Nota Fiscal de Entrada

**Valor unitário** = R$ 75,30 / 10

**Valor unitário** = R$ 7,53

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img08.png
   :scale: 100%
   
**5. Custo atual do SUB**

Na tela **"BR One :: Detalhe custo atual do subproduto"**, são listados todos os documentos gerados como:

- Entrada de Subproduto
- Estorno Entrada Subproduto

**6. Custo por produto**

Para encontrar o custo por produto é realizado o cálculo:

*(Custo componentes + Rateio de custos de terceiros) / Quantidade entrada de PA.*

- Custo componentes: R$ 49,50

- Rateio de custos de terceiros: R$ 75,30

- Quantidade entrada de PA: 8

**Custo por produto** = (R$ 49,50 + R$ 75,30) / 8

**Custo por produto** =  R$ 15,60


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img09.png
   :scale: 100%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img10.png
   :scale: 100%


**7. Desvio total**

Para encontrar o desvio total é realizado o cálculo:

*Custo atual do PA – (Custo componentes + Rateio de custos de terceiros + GGF antecipado)*


- Custo atual do PA: R$ 119,30

- Custo componentes: R$ 49,50

- Rateio de custos de terceiros: R$ 75,30

- GGF antecipado: R$ 0,00

**Desvio total** = R$ 119,30 – (R$ 49,50 + R$ 75,30 + R$ 0,00)

**Desvio total** = R$ -5,50

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img11.png
   :scale: 100%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img12.png
   :scale: 100%


**8. Desvio por produto**

Para encontrar o desvio por produto é realizado o cálculo:

*Desvio total / Quantidade entrada de PA*

- Desvio total: R$ - 5,50

- Quantidade entrada de PA: 8

**Desvio por produto** = R$ - 5,50 / 8

**Desvio por produto** =  R$ - 0,687

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img13.png
   :scale: 100%

**9. Variação %**

Para encontrar a variação é realizado o cálculo:

*Desvio por produto / Custo por produto \* 100*

- Desvio por produto: R$ - 0,687

- Custo por produto: R$ 15,60

**Variação %** = R$ -0,687 / R$ 15,60 \* 100

**Variação %** =  - 4,41

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img14.png
   :scale: 100%

**10. Ignorar no fechamento de custos**

As OPs que estiverem com essa opção marcada, não serão consideradas no cálculo do fechamento de custo mensal, para realização do rateio dos gastos gerais de fabricação cadastrados.

**11. Quantidade concluída**

Soma das quantidades que foram realizados os apontamentos na Entrada de PA.


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img15.png
   :scale: 100%

**12. Quantidade refugo**

Quantidade refugada em uma Entrada de PA ou Saída de insumos. Os componentes que tiverem o depósito **Item de terceiros em minha propriedade serão desconsiderados.**

**13. % refugo**

Para encontrar o % refugo é realizado o cálculo:

*(Quantidade de refugo / (Quantidade de refugo + Quantidade PA)) \* 100*

- Quantidade de refugo: 1

- Quantidade PA: 8

**% refugo** = (1 / (1 + 8)) \* 100

**% refugo** = 11,11

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img16.png
   :scale: 100%

**14. Data fechamento**

É informado a data que a OP foi fechada.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img17.png
   :scale: 100%

**15. Atraso (dias)**

É informado a quantidade de dias de atraso da OP **(Data fechamento – Data vencimento)**


**16. Observações do diário**

Nas observações do diário são listados todos os lançamentos de ajustes realizados no fechamento da Ordem de Produção.
De acordo com o valor do desvio é realizado a validação das movimentações do item e os ajustes são inseridos.

**Exemplos:**

**1. Desvio positivo**

- **1.1 Quantidade em estoque maior ou igual à Quantidade de Entradas de PA**

Quantidade em estoque for maior ou igual à quantidade de Entradas de PA, significa que tudo o que foi produzido ainda está no estoque. 
É realizada somente a reavaliação de estoque do tipo débito/crédito para o item da OP.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img18.png
   :scale: 100%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Valor** = Desvio total \* (-1)

**Valor** = 5,50 \* (-1)

**Valor** = -5,50

- **1.2 Quantidade em estoque menor que a quantidade de Entradas de PA**


Quando a quantidade em estoque for menor que a quantidade de Entradas de PA significa que parte do que foi produzido está no estoque e outra parte foi vendido.

Nesse caso será gerado uma reavaliação de estoque e um lançamento contábil manual.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img19.png
   :scale: 100%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Quantidade estoque** = 5

**Valor** = ((Desvio total / Quantidade de PA) \* Quantidade em estoque) \* (-1)

**Valor** = ((5,50 / 11) \* 5) \*(-1) 

**Valor** = (0,5 \* 5) \*(-1) 

**Valor** = 2,5 \* (-1)

**Valor** = - 2,50




- **LCM**

**Crédito:** Conta de custo de produtos vendidos (CPV) 

**Débito:** Conta de material em processo (WIP)

**Valor** = (Desvio total / Entrada PA) \* (Entrada PA - Quantidade em estoque) 

**Valor** = (5,50 / 11) \* (11 - 5) 

**Valor** = (0,5) \* (6) 

**Valor** = 3





- **1.3 Sem estoque, mas com Entrada de PA**

Se não tiver estoque, mas tiver sido feita a entrada de produto acabado, então significa que tudo o que foi produzido já foi vendido. Como não existe estoque para reavaliar, o desvio de custo deverá ser incorporado num LCM, na Conta de custo de produtos vendidos. É realizado apenas um LCM.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img20.png
   :scale: 100%

- **LCM**

**Crédito:** Conta de custo de produtos vendidos (CPV) 

**Débito:** Conta de material em processo (WIP)

**Valor** = Desvio total 

**Valor** =  5,50 


- **1.4 Quantidade em estoque e valor acumulado menor que desvio calculado**

Quando possuir quantidade em estoque igual ou menor que entrada de PA, porém, o valor acumulado do depósito é menor que o desvio calculado para o item. 

Nesse cenário podemos ter:

- **1.4.1 Quantidade de estoque maior ou igual da entrada de PA e valor acumulado menor que desvio calculado.**

Será gerado uma reavaliação do estoque e um LCM de desvio de custo.

Verificação da quantidade e valor acumulado do estoque:

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img21.png
   :scale: 100%


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img22.png
   :scale: 100%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Valor** = Valor acumulado do estoque \* (-1)

**Valor** = 2,50 \* (-1)

**Valor** = -2,50

- **LCM (Desvio de custo)**

**Crédito:** Conta de desvio do estoque de material em processo

**Débito:** Conta de material em processo (WIP)

**Valor** = Desvio total - Valor acumulado do estoque

**Valor** = 5,50 – 2,50

**Valor** = 3



- **1.4.2 Quantidade em estoque menor da entrada de PA e valor acumulado menor que desvio calculado**

Será gerado uma reavaliação do estoque e um LCM de desvio de custo e um LCM de custo de produtos vendidos.

Verificação da quantidade e valor acumulado do estoque:

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img23.png
   :scale: 100%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img24.png
   :scale: 100%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Valor** = Valor acumulado do estoque \* (-1)

**Valor** = 2,50 \* (-1)

**Valor** = - 2,50

- **LCM (Desvio de custo)**

**Crédito:** Conta de desvio do estoque de material em processo

**Débito:** Conta de material em processo (WIP)

**Quantidade em estoque** = 8

**Valor** = ((Desvio total / Quantidade de PA) \* Quantidade em estoque) – valor acumulado do estoque

**Valor** = ((5,50 / 11) \* 8) – 2,50

**Valor** =  (0,5 \* 8) – 2,50

**Valor** = 4,00 – 2,50

**Valor** = 1,50

- **LCM (Custo de produtos vendidos)**

**Crédito:** Conta de custo de produtos vendidos (CPV) 

**Débito:** Conta de material em processo (WIP)

**Valor** = (Desvio total / Entrada PA) \* (Entrada PA - Quantidade Estoque) 

**Valor** = (5,50 / 11) \* (11 - 8) 

**Valor** = (0,5) \* (3) 

**Valor** = 1,50



**2. Desvio negativo**

- **2.1 Quantidade em estoque maior ou igual à quantidade de Entradas de PA**

Quantidade em estoque for maior ou igual à quantidade de Entradas de PA, significa que tudo o que foi produzido ainda está no estoque. 
É realizada somente a reavaliação de estoque do tipo débito/crédito para o item da OP.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img25.png
   :scale: 100%

- **Reavaliação de estoque**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de estoque

**Valor** = Desvio total \* (-1)

**Valor** = - 5,50 \* (-1)

**Valor** = 5,50

- **2.2 Quantidade em estoque menor que a quantidade de Entradas de PA**

No LCM para desvio negativo, a conta crédito é equivalente à conta de material em processo (WIP), a conta débito é equivalente à conta de custo de produtos vendidos (CPV) do estoque padrão e o valor é (valor desvio /quantidade entrada de PA) \* (Quantidade entrada de PA - Quantidade estoque).

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img26.png
   :scale: 100%


- **Reavaliação de estoque**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de estoque

**Quantidade em estoque** = 5

**Valor** = ((Desvio total / Quantidade entrada de PA) \* Quantidade em estoque) \* (-1)

**Valor** = ((R$ - 5,50 / 8) \* 5) \*(-1) 

**Valor** = (- 0,687 \* 5) \* (-1)

**Valor** = - 3,435 \* (-1)

**Valor** = 3,44



- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de custo de produtos vendidos (CPV)

**Valor** = (Desvio total / Entrada PA) \* (Entrada PA - Quantidade Estoque) 

**Valor** =(R$ - 5,50 / 8) \* (8 - 5) \*(-1)

**Valor** = (- 0,687 \* 3) \* (-1)

**Valor** = - 2,06 \*(-1)

**Valor** = 2,06


- **2.3 Sem estoque, mas com Entrada de PA**


Se não tiver estoque, mas tiver sido feita a entrada de produto acabado, então significa que tudo o que foi produzido já foi vendido. Como não existe estoque para reavaliar, o desvio de custo deverá ser incorporado num LCM, na Conta de custo de produtos vendidos. É realizado apenas um LCM.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img27.png
   :scale: 100%

- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de custo de produtos vendidos (CPV)

**Valor** = Desvio total \* (-1)

**Valor** = - 5,50 \* (-1)

**Valor** = 5,50


- **2.4 Sem Entrada de PA e com ou sem estoque**

Quando não existir entrada de PA, independente se há ou não estoque para o item, se houver um desvio, **sempre** será um **desvio negativo**. Para OPs. de Beneficiamento de compra o valor de rateios de custo de terceiros não é levado para lançamento contábil manual.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ beneficiamento\ de\ compra/img28.png
   :scale: 100%



- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de desvio do estoque de material em processo

**Valor** = (Desvio total – Rateios de custo de terceiros) \* (-1)

**Valor** = 13,03 – 7,53 \* (-1)

**Valor** = 5,50