Ordem de Produção - Desmontagem
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Detalhamento dos campos e cálculos utilizados na aba custo da Ordem de Produção Desmontagem.

Para exemplificar o processo de produção, vamos utilizar uma Ordem de Produção (OP) com uma quantidade planejada de 5 unidades. 

Seu roteiro é composto por 2 componentes, sendo que a quantidade base de cada um deles é de 1 unidade e quantidade fixa é 0. E também composto por um recurso de mão de obra, sendo o tempo variável 5minutos e tempo fixo 2minutos.

Para encontrar **quantidade planejada** de cada item:

**Quantidade planejada** = Quantidade base \* quantidade planejada do cabeçalho da OP + quantidade fixo

Para encontrar o **tempo planejado** de cada recurso:

**Tempo planejado** = Tempo variável \* quantidade planejada do cabeçalho da OP + tempo fixo  

**Custos dos componentes utilizados:**

- Item I009 – R$ 2,50

- Item I010 – R$ 3,00	

Nesse cenário também iremos utilizar o custo do recurso através do GGF antecipado.

**Custo hora dos recursos:**

- MAO01 - R$15,00


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img01.png
   :scale: 100%

Iremos passar pelos campos da aba Custo

**1. Custo não alocado**

São listados os valores de custo alocado no fechamento de custo, caso a OP não tenha entrada de PA no mês do apontamento de horas.

**2. Custo componentes**

Na tela **"BR One :: Detalhe custo de componentes" [...]**, são listados todos os documentos gerados como:

- Entrada de componentes;

O sistema recupera o custo unitário de cada componente que será realizado o documento e multiplica pela quantidade, gerando assim o custo total.

Na Entrada de componentes realizada para o **item I009** de 4 unidades com o custo unitário de R$ 2,50, resultando em um custo total de **R$ 10,00**. Já o **item** **I010** de 4 unidades com o custo unitário de R$ 3,00, totalizando um custo de **R$ 12,00**. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img02.png

Dessa forma, o custo dos componentes é a soma da coluna de custo total dos detalhes, sendo **R$ 22,00**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img03.png

**3. Custo atual do PA**

Na tela **"BR One :: Detalhe custo atual do PA"**, são listados todos os documentos gerados como:

- Saída de mercadoria (PA)
- LCM

**Para encontrar o custo do Recurso por PA:**

*(Custo do recurso encontrado \* tempo planejado em horas/quantidade planejada do produto acabado)*

*(15 \** 0,45 */5) =* **1,35**

O custo do recurso é de **R$ 15,00/hora**, o [tempo planejado](#tempoplanejado) transformado em horas é de 0,45 (ou seja, 27 minutos), a quantidade planejada do produto acabado é 5.

O sistema recupera o custo unitário do PA que será realizado o documento e multiplica pela quantidade, gerando assim o custo total.

Realizada saída de mercadoria (PA) do PA de 4 unidades com o custo unitário de R$ 5,50, resultando em um custo total de **R$ 22,00.**

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img04.png
   :scale: 100%

Para criação do LCM de GGF antecipado é recuperado o GGF antecipado por PA e multiplicado pela quantidade apontada. No caso 1,35 \* 4 = **R$ 5,40**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img05.png
   :scale: 100%

Nesse cenário também houve **Apontamento de refugo** na saída de produto acabado na quantidade de 1 PA. 

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img06.png
   :scale: 100%

Veremos que o custo antecipado estará vinculado a uma LCM, que somará o total da **“Saída de mercadoria”**.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img07.png
   :scale: 100%

**4. Rateios de custo de terceiros**

Exibe os documentos que deram origem ao valor do rateio de custos de terceiros.

**5. Custo atual do SUB**

Na tela **"BR One :: Detalhe custo atual do subproduto"**, são listados todos os documentos gerados como:

- Entrada de Subproduto
- Estorno Entrada Subproduto

**6. Custo por produto**

Na OP de desmontagem esse campo fica com o valor **0,00** . O cálculo desse campo não se aplica para OP de desmontagem.

**7. Desvio total**

O desvio total da OP de desmontagem, possui um cálculo diferente da OP padrão, devido à finalidade de cada uma, a OP de desmontagem nos entrega componentes enquanto a OP padrão entrega um produto acabado. Segue abaixo fórmula e cálculo para exemplificação.

*Custo componentes – (Custo atual do PA + Rateio de custos de terceiros)*

-Custo componentes: R$ 22,00
-Custo atual do PA: R$ 32,90

-Rateio de custos de terceiros: R$0,00

**Desvio total** = R$ 22,00 – (R$ 32,90 + R$ 00,00)

**Desvio total** = R$ - 10,90


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img08.png
   :scale: 100%

**8. Desvio por produto**

Na OP de desmontagem esse campo fica com o valor **0,00** . O cálculo desse campo não se aplica para OP de desmontagem.

**9. Variação %**

Na OP de desmontagem esse campo fica com o valor **0,00** . O cálculo desse campo não se aplica para OP de desmontagem.

**10. Ignorar no fechamento de custos**

As OPs que estiverem com essa opção marcada, não serão consideradas no cálculo do fechamento de custo mensal, para realização do rateio dos gastos gerais de fabricação cadastrados.

**11. Quantidade concluída**

Soma das quantidades que foram realizados os apontamentos na Saída de PA.

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img09.png
   :scale: 100%

**12. Quantidade refugo**

Quantidade refugada em uma Saída de PA. Os componentes que tiverem o depósito **Item de terceiros em minha propriedade serão desconsiderados.**

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img10.png
   :scale: 100%

**13. % refugo**

Para encontrar o % refugo é realizado o cálculo:

*(Quantidade de refugo / (Quantidade de refugo + Quantidade PA)) \* 100*

- Quantidade de refugo: 1

- Quantidade PA: 4

**% refugo** = (1 / (1 + 4)) \* 100

**% refugo** = 20

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img11.png
   :scale: 100%

**14. Data fechamento**

É informado a data que a OP foi fechada


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img12.png
   :scale: 100%

**15. Atraso (dias)**

É informado a quantidade de dias de atraso da OP **(Data fechamento – Data vencimento)**


**16. Observações do diário**

Nas observações do diário são listados todos os lançamentos de ajustes realizados no fechamento da Ordem de Produção.
De acordo com o valor do desvio é realizado a validação das movimentações do item e os ajustes são inseridos.

**Exemplos:**

**1. Desvio positivo**

.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img13.png
   :scale: 100%

- **LCM**

**Crédito:** Conta de desmontagem (configurações de produção na aba OP)

**Débito:**  Conta de Material em Processo (WIP)

**Valor** = Desvio Total 

**Valor** = 11,10


**2. Desvio negativo**


.. image:: /_static/BR\ One\ Produção/Processo/Aba\ custo\ OP/OP\ Desmontagem/img14.png
   :scale: 100%

- **LCM**

**Crédito:** Conta de material em processo (WIP)

**Débito:**  Conta de desmontagem (configurações de produção na aba OP)

**Valor** = Desvio Total \* (-1) 

**Valor** = - 10,90 \* (-1)

**Valor** = 10,90 



**OBS.:** *Informações como **‘Custo por produto’**, **‘desvio por produto’**, **‘variação % da OP de desmontagem’** não são relevantes para a OP de desmontagem, portanto, não são calculadas pelo sistema.*
