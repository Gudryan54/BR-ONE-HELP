Criar ficha de análise automaticamente na Entrada de produto acabado - Retrabalho
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Configuração para geração das fichas de análise automáticas com base na **'Entrada de Produto Acabado'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/01.JPG
   :scale: 50%

Abaixo uma tabela da configuração, ações realizadas dentro do sistema e o resultado das fichas geradas para **'Ordem produção Retrabalho'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR02.JPG
   :scale: 50%

**Para a operação a ficha deve ser sempre gerada no momento da liberação da ordem de produção.**

**1. Produto Acabado e Operação**

Geração da Ficha de análise para a ordem de produção de retrabalho configurada no campo **'Ficha de análise'** como **'Produto Acabado e Operação – PO'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR03.JPG
   :scale: 70%

Ao liberar a OP 1033, serão validadas as operações que possuem modelos de análises configurados, neste cenário será gerada apenas uma  ficha de análise para a operação. Para a ordem de produção de retrabalho a ficha para o produto acabado é gerado somente no processo de entrada do PA na efetivação da transferência de estoque.

- **Ficha de análise para a operação na liberação da OP:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR04.JPG
   :scale: 70%

- **Ficha de análise do produto acabado gerada na entrada do PA sem a troca de lote na efetivação da transferência de estoque:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR05.JPG
   :scale: 70%

- **Ficha de análise do produto acabado gerada na entrada do PA com a troca de lote na efetivação da transferência de estoque:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR06.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para a **operação**.

**2. Operação**

Geração da Ficha de análise para a ordem de produção de retrabalho configurada no campo **Ficha de análise** como **Operação – OP**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR07.JPG
   :scale: 70%

Ao liberar a OP 657 serão validadas as operações que possuem modelos de análises configurados, neste cenário será gerada apenas uma ficha de análise para a operação.

- **Ficha de análise para a operação na liberação da OP:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR08.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para o **produto acabado** na entrada de PA.

**3. Produto Acabado**

Geração da Ficha de análise para a ordem de produção de retrabalho configurada no campo **'Ficha de análise'** como **'Produto Acabado – PA'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR09.JPG
   :scale: 70%

Na liberação da OP 658, não é gerado nenhuma ficha de análise, pois a ficha de análise para o produto acabado da ordem de produção de retrabalho é gerada somente no processo de entrada de PA na efetivação da transferência de estoque. 

- **Ficha de análise do produto acabado gerada na entrada do PA sem a troca de lote na efetivação da transferência de estoque:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR10.JPG
   :scale: 70%

- **Ficha de análise do produto acabado gerada na entrada do PA com a troca de lote na efetivação da transferência de estoque:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR11.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para a **operação**.

**4. Nenhum**

Geração da Ficha de análise para a ordem de produção de retrabalho configurada no campo **'Ficha de análise'** como **'Nenhum – NM'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PARet/PAR12.JPG
   :scale: 70%

Na OP **não é gerado nenhuma ficha de análise**.