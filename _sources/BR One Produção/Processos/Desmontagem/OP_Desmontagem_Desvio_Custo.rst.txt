
Desvio de custo
~~~~~~~~~~~~~~~~~~~~~~~~

Na aba **'Custo'**, existe um campo que calcula o desvio de custo do produto. Para contabilizar o valor deste desvio, no momento do fechamento da OP de desmontagem, são realizados lançamentos contábeis para considerar esta diferença.

.. image:: /_static/BR\ One\ Produção/Processo/Desmontagem/030.png
   :scale: 80%

Se o desvio de custo for:

**Positivo**, gera um LCM:

- Crédito – Conta de desmontagem (configurações de produção na aba OP)
- Débito - Conta de Material em Processo (WIP)

**Negativo**, gera um LCM:

- Crédito – Conta de Material em Processo (WIP)
- Débito - Conta de desmontagem (configurações de produção na aba OP)

**Cálculo Desvio Total da OP de Desmontagem**

O desvio total da OP de desmontagem, possui um cálculo diferente da OP padrão, devido a finalidade de cada uma, a OP de desmontagem nos entrega componentes enquanto a OP padrão entrega um produto acabado. 

Segue abaixo fórmula e cálculo para exemplificação.

**OP Desmontagem:**

Desvio total = Custo componentes - (Custo atual do PA + Rateio), exemplo:

- Custo atual do PA = 100 
- Custo componentes = 200
- Rateio = 0,0

Desvio total = 200 - (100 + 0,0) -> **Desvio total = 10**

**OP Padrão:**

Desvio total = Custo atual do PA - (Custo componentes + Rateio), exemplo:

- Custo atual do PA = 100 
- Custo componentes = 200
- Rateio = 0,0

Desvio total = 100 - (200 + 0,0) -> **Desvio total = -100**

Informações como **‘Custo por produto’**, **‘desvio por produto’**, **‘variação % da OP de desmontagem’** não são relevantes para a OP de desmontagem, portanto, não são calculadas pelo sistema.