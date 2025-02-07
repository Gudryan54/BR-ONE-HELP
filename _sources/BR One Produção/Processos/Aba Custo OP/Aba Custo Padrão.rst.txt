Ordem de Produção - Padrão
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Detalhamento dos campos e cálculos utilizados na aba custo da Ordem de Produção Padrão.

Para exemplificar o processo de produção, vamos utilizar uma Ordem de Produção (OP) com uma quantidade planejada de 10 unidades. 

Seu roteiro é composto por 2 componentes, sendo que a quantidade base de cada um deles é de 1 unidade e quantidade fixa é 0. 
E também composto por um recurso de mão de obra, sendo o tempo variável 5 minutos e tempo fixo 2 minutos.

Para encontrar **quantidade planejada** de cada item:

**Quantidade planejada** = Quantidade base \* quantidade planejada do cabeçalho da OP + quantidade fixo.

Para encontrar o **tempo planejado** de cada recurso:

**Tempo planejado** = Tempo variável \* quantidade planejada do cabeçalho da OP + tempo fixo.

**Custos dos componentes utilizados:**

- Item I009 – R$ 2,50

- Item I010 – R$ 3,00	

Nesse cenário também iremos utilizar o custo do recurso através do GGF antecipado.

**Custo hora dos recursos:**

- MAO01 - R$15,00

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img01.png
   :scale: 80%

Iremos passar pelos campos da aba Custo

**1. Custo não alocado**

São listados os valores de custo alocado no fechamento de custo, caso a OP não tenha entrada de PA no mês do apontamento de horas.

**2. Custo componentes**

Na tela **"BR One :: Detalhe custo de componentes" [...]**, são listados todos os documentos gerados como:

- Saída de insumos;
- Saída de insumos com flag refugo marcada; 
- Apontamento de refugo com retorno do componente.

O sistema recupera o custo unitário de cada item que será realizado o documento e multiplica pela quantidade, gerando assim o custo total.

Na Saída de insumos realizada para o **item I009** de 10 unidades com o custo unitário de R$ 2,50, resultando em um custo total de **R$ 25,00**. Já o **item** **I010** de 10 unidades com o custo unitário de R$ 3,00, totalizando um custo de **R$ 30,00**. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img02.png
   :scale: 80%

Nesse cenário também houve **Apontamento de refugo** na quantidade de 2 PA, aonde os itens retornaram para seu estoque gerando um lançamento de **Estorno por refugo** (entrada de mercadoria) para os insumos. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img03.png
   :scale: 80%

O sistema recupera o custo unitário de cada item que será realizado o documento e multiplica pela quantidade, gerando assim o custo total nesse caso com o total negativo, pois está retornando ao estoque.

No Apontamento de refugo para o **item I009** de 2 unidades com o custo unitário de R$ 2,50, resultando em um custo total de **R$ 5,00**. Já o **item** **I010** de 2 unidades com o custo unitário de R$ 3,00, totalizando um custo de **R$ 6,00**. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img04.png
   :scale: 80%

Dessa forma, o custo dos componentes é a soma da coluna de custo total dos detalhes, sendo **R$ 44,00**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img05.png
   :scale: 80%

**3. Custo atual do PA**

Na tela **"BR One :: Detalhe custo atual do PA"**, são listados todos os documentos gerados como:

- Entrada de PA
- GGF antecipado
- Apontamento de Refugo
- Estorno Entrada de PA

O sistema recupera o custo unitário do PA através dos insumos, GGF antecipado.

Na entrada de PA é recuperado o custo dos insumos para produção de 1 PA + o cálculo do GGF antecipado por PA.

O custo dos componentes nesse cenário é de R$ 5,50, o custo do GGF antecipado por PA R$1,30. O custo unitário do PA será de 6,80.

**Para encontrar o custo do Recurso por PA:**

*(Custo do recurso encontrado \* tempo planejado em horas / quantidade planejada do produto acabado)*

*(15 \* 0,866667 /10) =* **1,30** 

O custo do recurso é de **R$ 15,00/hora**, o tempo planejado transformado em horas é de **0,866667** (ou seja, 52 minutos), a quantidade planejada do produto acabado é 10.

O sistema recupera o custo unitário do PA que será realizado o documento e multiplica pela quantidade, gerando assim o custo total.

Realizada entrada do PA de 10 unidades com o custo unitário de R$ 6,80, resultando em um custo total de **R$ 68,00.**

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img06.png
   :scale: 80%

Para criação do LCM de GGF antecipado é recuperado o GGF antecipado por PA e multiplicado pela quantidade apontada. No caso 1,30 \* 10 = **R$13,00**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img07.png
   :scale: 80%

Nesse cenário também houve **Apontamento de refugo** na quantidade de 2 PA, aonde foram dado baixa do item no estoque gerando um lançamento de **Estorno por refugo** (saída de mercadoria) para o PA. 

O sistema recupera o custo unitário do PA e multiplica pela quantidade, gerando assim o custo total nesse caso com o total negativo, pois está retirando do estoque.

No Apontamento de refugo para o PA de 2 unidades com o custo unitário de R$ 6,66, resultando em um custo total de **R$ 13,32**. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img08.png
   :scale: 80%

Dessa forma, o custo atual do PA é a soma da coluna de custo total dos detalhes, sendo **R$ 54,68**.


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img09.png
   :scale: 80%

**4. Rateios de custo de terceiros**

Exibe os documentos que deram origem ao valor do rateio de custos de terceiros.


**5. Custo atual do SUB**

Na tela **"BR One :: Detalhe custo atual do subproduto"**, são listados todos os documentos gerados como:

- Entrada de Subproduto
- Estorno Entrada Subproduto

O sistema recupera o custo unitário do Subproduto através da Entrada de PA e conforme configuração para cálculo.

**6. Custo por produto**

Para encontrar o custo por produto é realizado o cálculo:

*(Custo componentes + GGF antecipado) / Quantidade entrada de PA.*

- Custo componentes: R$ 44,00

- GGF antecipado: R$ 13,00

- Quantidade entrada de PA: 8

**Custo por produto** = (R$ 44,00 + R$ 13,00) / 8 

**Custo por produto** = R$ 7,13


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img10.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img11.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img12.png
   :scale: 80%

**7. Desvio total**

Para encontrar o desvio total é realizado o cálculo:

*Custo atual do PA – (Custo componentes + Rateio de custos de terceiros + GGF antecipado)*

- Custo atual do PA: R$ 54,68

- Custo componentes: R$ 44,00

- Rateio de custos de terceiros: R$0,00

- GGF antecipado: R$ 13,00

**Desvio total** = R$ 54,68 – (R$ 44,00 + R$0,00 + R$ 13,00) 

**Desvio total** = R$ -2,32

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img13.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img14.png
   :scale: 80%


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img15.png
   :scale: 80%


**8. Desvio por produto**

Para encontrar o desvio por produto é realizado o cálculo:

*Desvio total / Quantidade entrada de PA*

- Desvio total: R$ -2,32

- Quantidade entrada de PA: 8

**Desvio por produto** = R$ -2,32 / 8

**Desvio por produto** = R$ -0,29

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img16.png
   :scale: 80%

**9. Variação %**

Para encontrar a variação é realizado o cálculo:

*Desvio por produto / Custo por produto \* 100*

- Desvio por produto: R$ - 0,29

- Custo por produto: R$ 7,13

**Variação %** = R$ -0,29 / R$ 7,13 \* 100

**Variação %** = -4,07

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img17.png
   :scale: 80%

**10. Ignorar no fechamento de custos**

As OPs que estiverem com essa opção marcada, não serão consideradas no cálculo do fechamento de custo mensal, para realização do rateio dos gastos gerais de fabricação cadastrados.

**11. Quantidade concluída**

Soma das quantidades que foram realizados os apontamentos na Entrada de PA.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img18.png
   :scale: 80%

**12. Quantidade refugo**

Quantidade de refugo registrada através da tela de **BR One :: Apontamento de refugo**. Os componentes que tiverem o depósito **Item de terceiros em minha propriedade serão desconsiderados.**

**13. % refugo**

Para encontrar o % refugo é realizado o cálculo:

*(Quantidade de refugo / (Quantidade de refugo + Quantidade PA)) \* 100*

- Quantidade de refugo: 2

- Quantidade PA: 8

**% refugo** = (2 / (2 + 8)) \* 100

**% refugo** = 20

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img19.png
   :scale: 80%

**14. Data fechamento**

É informado a data que a OP foi fechada

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img20.png
   :scale: 80%

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

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img21.png
   :scale: 80%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Valor** = Desvio total \* (-1)

**Valor** = 14,18 \* (-1)

**Valor** = -14,18


- **1.2 Quantidade em estoque menor que a Quantidade de Entradas de PA**

Quando a quantidade em estoque for menor que a quantidade de Entradas de PA significa que parte do que foi produzido está no estoque e outra parte foi vendido.

Nesse caso será gerado uma reavaliação de estoque e um lançamento contábil manual.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img22.png
   :scale: 80%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Quantidade estoque** = 4

**Valor** = ((Desvio total / Quantidade de PA) \* Quantidade em estoque) \* (-1)

**Valor** = ((14,18 / 8) \* 4) *(-1)

**Valor** = (1,7725 \* 4) *(-1)

**Valor** = 7,09 \* (-1)

**Valor** = - 7,09


- **LCM**

**Crédito:** Conta de custo de produtos vendidos (CPV) 

**Débito:** Conta de material em processo (WIP)

**Valor** = (Desvio total / Entrada PA) \* (Entrada PA - Quantidade em estoque) 

**Valor** = (14,18 / 8) \* (8 - 4) 

**Valor** = (1,7725) \* (4) 

**Valor** = 7,09


- **1.3 Sem estoque, mas com Entrada de PA**

Se não tiver estoque, mas tiver sido feita a entrada de produto acabado, então significa que tudo o que foi produzido já foi vendido. Como não existe estoque para reavaliar, o desvio de custo deverá ser incorporado num LCM, na Conta de custo de produtos vendidos. É realizado apenas um LCM.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img23.png
   :scale: 80%

- **LCM**

**Crédito:** Conta de custo de produtos vendidos (CPV) 

**Débito:** Conta de material em processo (WIP)

**Valor** = Desvio total 

**Valor** = 14,18 


- **1.4 Quantidade em estoque e valor acumulado menor que desvio calculado**

Quando possuir quantidade em estoque igual ou menor que entrada de PA, porém, o valor acumulado do depósito é menor que o desvio calculado para o item. 

Nesse cenário podemos ter:

- **1.4.1 Quantidade de estoque maior ou igual da entrada de PA e valor acumulado menor que desvio calculado.**

Será gerado uma reavaliação do estoque e um LCM de desvio de custo.

Verificação da quantidade e valor acumulado do estoque:

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img24.png
   :scale: 80%


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img25.png
   :scale: 80%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Valor** = Valor acumulado do estoque \* (-1)

**Valor** = 3,28 \* (-1)

**Valor** = - 3,28


- **LCM (Desvio de custo)**

**Crédito:** Conta de desvio do estoque de material em processo

**Débito:** Conta de material em processo (WIP)

**Valor** = Desvio total - Valor acumulado do estoque

**Valor** = 14,18 - 3,28

**Valor** = 10,90



- **1.4.2 Quantidade em estoque menor da entrada de PA e valor acumulado menor que desvio calculado**

Será gerado uma reavaliação do estoque e um LCM de desvio de custo e um LCM de custo de produtos vendidos.

Verificação da quantidade e valor acumulado do estoque:

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img26.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img27.png
   :scale: 80%

- **Reavaliação de estoque**

**Crédito:** Conta de estoque

**Débito:** Conta de material em processo (WIP)

**Valor** = Valor acumulado do estoque \* (-1)

**Valor** = 3,28 \* (-1)

**Valor** = - 3,28

- **LCM (Desvio de custo)**

**Crédito:** Conta de desvio do estoque de material em processo

**Débito:** Conta de material em processo (WIP)

**Quantidade em estoque** = 4

**Valor** = ((Desvio total / Quantidade de PA) \* Quantidade em estoque) – valor acumulado do estoque

**Valor** = ((14,18 / 8) \* 4) – 3,28

**Valor** = (1,7725 \* 4) - 3,28

**Valor** = 7,09 - 3,28

**Valor** = 3,81

- **LCM (Custo de produtos vendidos)**

**Crédito:** Conta de custo de produtos vendidos (CPV) 

**Débito:** Conta de material em processo (WIP)

**Valor** = (Desvio total / Entrada PA) \* (Entrada PA - Quantidade Estoque) 

**Valor** = (14,18 / 8) \* (8 - 4) 

**Valor** = (1,7725) \* (4) 

**Valor** = 7,09


**2. Desvio negativo**

- **2.1 Quantidade em estoque maior ou igual à Quantidade de Entradas de PA**

Quantidade em estoque for maior ou igual à quantidade de Entradas de PA, significa que tudo o que foi produzido ainda está no estoque. 
É realizada somente a reavaliação de estoque do tipo débito/crédito para o item da OP.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img28.png
   :scale: 80%

- **Reavaliação de estoque**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de estoque

**Valor** = Desvio total \* (-1)

**Valor** = -2,32 \* (-1)

**Valor** = 2,32

- **2.2 Quantidade em estoque menor que a quantidade de Entradas de PA**

No LCM para desvio negativo, a conta crédito é equivalente à conta de material em processo (WIP), a conta débito é equivalente à conta de custo de produtos vendidos (CPV) do estoque padrão e o valor é (valor desvio /quantidade entrada de PA) \* (Quantidade entrada de PA - Quantidade estoque).

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img29.png
   :scale: 80%


- **Reavaliação de estoque**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de estoque

**Quantidade em estoque** = 2

**Valor** = ((Desvio total / Quantidade entrada de PA) \* Quantidade em estoque) \* (-1)

**Valor** = ((R$ -2,32 / 8) \* 2) \*(-1) 

**Valor** = (- 0,29 \* 2) \* (-1)

**Valor** = -0,58 \* (-1)

**Valor** = 0,58



- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de custo de produtos vendidos (CPV)

**Valor** = (Desvio total / Entrada PA) \* (Entrada PA - Quantidade Estoque) 

**Valor** = (R$ -2,32 / 8) \* (8 -2) \* (-1)

**Valor** = (- 0,29 \* 6) \* (-1)

**Valor** = - 1,74 \* (-1)

**Valor** = 1,74


- **2.3 Sem estoque, mas com Entrada de PA**

Se não tiver estoque, mas tiver sido feita a entrada de produto acabado, então significa que tudo o que foi produzido já foi vendido. 
Como não existe estoque para reavaliar, o desvio de custo deverá ser incorporado num LCM, na Conta de custo de produtos vendidos. É realizado apenas um LCM.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img30.png
   :scale: 80%

- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de custo de produtos vendidos (CPV)

**Valor** = Desvio total \* (-1)

**Valor** = -2,32 \* (-1)

**Valor** = 2,32


- **2.4 Sem Entrada de PA e com ou sem estoque**

Quando não existir entrada de PA, independente se há ou não estoque para o item, se houver um desvio, **sempre** será um **desvio negativo**. É realizado apenas um LCM.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Padrao/img31.png
   :scale: 80%


- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:** Conta de desvio do estoque de material em processo

**Valor** = Desvio total \* (-1)

**Valor** = -2,32 \* (-1)

**Valor** = 2,32