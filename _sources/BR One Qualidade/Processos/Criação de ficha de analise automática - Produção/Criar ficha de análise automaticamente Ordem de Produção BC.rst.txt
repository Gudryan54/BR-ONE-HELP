Criar ficha de análise automaticamente na Ordem de Produção - Beneficiamento de Compras
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Configuração para geração das fichas de análise automáticas com base na **Ordem de Produção**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC01.JPG
   :scale: 50%

Abaixo uma tabela da configuração, ações realizadas dentro do sistema e o resultado das fichas geradas para **'Ordem Produção de Beneficiamento de Compra'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC02.JPG
   :scale: 50%

Iremos realizar o processo com o parâmetro de ‘Ficha de análise’ configurado na ‘Ordem de Produção’

**Importante:** para itens administrados por "Lote", a ficha de análise gerada automaticamente para a ordem de produção de beneficiamento de compra, não possui número de lote definido, logo a ficha de análise criada, não levará nenhum valor para o campo "Lote".

**1. Produto Acabado e Operação**

Geração da Ficha de análise para a ordem de produção de beneficiamento de compra configurada no campo **'Ficha de análise'** como **'Produto Acabado e Operação – PO'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC03.JPG
   :scale: 70%

Ao liberar a OP 648 serão validadas as operações que possuem modelos de análises configurados, neste cenário será gerada apenas uma ficha de análise para a operação. Para a ordem de produção de beneficiamento de compra a ficha para o produto acabado é gerado somente no processo de entrada do PA, após na efetivação da transferência de estoque.

- **Ficha de análise para a operação na liberação da OP:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC04.JPG
   :scale: 70%

- **Ficha de análise do produto acabado gerada na entrada do PA na efetivação da transferência de estoque:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC05.JPG
   :scale: 70%

**2. Operação**

Geração da Ficha de análise para a ordem de produção de beneficiamento de compra configurada no campo **'Ficha de análise'** como **'Operação – OP'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC06.JPG
   :scale: 70%

Ao liberar a OP 649, serão validadas as operações que possuem modelos de análises configurados, neste cenário será gerada apenas uma ficha de análise para a operação.

- **Ficha de análise para a operação na liberação da OP:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC07.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para o **produto acabado** na entrada de PA.

**3. Produto Acabado**

Geração da Ficha de análise para a ordem de produção de beneficiamento de compra configurada no campo **'Ficha de análise'** como **'Produto Acabado – PA'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC08.JPG
   :scale: 70%

Na liberação da OP 650, não é gerado nenhuma ficha de análise, pois a ficha de análise para o produto acabado da ordem de produção de beneficiamento de compra é gerada somente no processo de entrada de PA na efetivação da transferência de estoque 

- **Ficha de análise do produto acabado gerada na entrada do PA na efetivação da transferência de estoque:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC09.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para a **operação**.

**4. Nenhum**

Geração da Ficha de análise para a ordem de produção de beneficiamento de compra configurada no campo **'Ficha de análise'** como **'Nenhum – NM'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/OPBC/OPBC10.JPG
   :scale: 70%

Na liberação da OP 651, **não é gerado nenhuma ficha de análise**.