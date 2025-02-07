Criar ficha de análise automaticamente na Entrada de produto acabado - Padrão
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Configuração para geração das fichas de análise automáticas com base na **'Entrada de Produto Acabado'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/01.JPG
   :scale: 50%

Abaixo uma tabela da configuração, ações realizadas dentro do sistema e o resultado das fichas geradas para **'Ordem Produção Padrão'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP02.JPG
   :scale: 50%

**Para a operação a ficha deve ser sempre gerada no momento da liberação da ordem de produção.**

**1. Produto Acabado e Operação**

Geração da Ficha de análise para a ordem de produção padrão configurada no campo **'Ficha de análise'** como  **'Produto Acabado e Operação – PO'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP03.JPG
   :scale: 70%

No momento da liberação da OP 652, serão validadas as operações que possuem modelo de análise configurado e no processo de entrada de PA será validado se o produto acabado possui configurado modelos de análises, neste cenário serão geradas uma para a operação na liberação e será gerada ficha de análise para o produto acabado em cada entrada de PA realizada.

-**Ficha de análise para a operação na liberação da OP:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP04.JPG
   :scale: 70%

-**Ficha de análise para o produto acabado gerada na entrada PA:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP05.JPG
   :scale: 70%

**2. Operação**

Geração da Ficha de análise para a ordem de produção padrão configurada no campo **'Ficha de análise'** como  **'Operação – OP'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP06.JPG
   :scale: 70%

Na liberação da OP 653, serão validadas as operações que possuem modelo de análise configurado, neste cenário será gerada apenas uma ficha de análise para a operação na liberação da ordem de produção.

- **Ficha de análise para a operação na liberação da OP:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP07.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para o **produto acabado** na entrada de PA.

**3. Produto Acabado**

Geração da Ficha de análise para a ordem de produção padrão configurada no campo **'Ficha de análise'** como **'Produto Acabado - PA'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP08.JPG
   :scale: 70%

Ao realizar o processo de entrada de PA para a OP 654, será validado se o produto acabado da ordem de produção possui modelo de análise configurado, neste cenário será gerada ficha de análise para o produto acabado em cada entrada de PA realizada.

- **Ficha de análise para o produto acabado gerada na entrada de PA:**

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP09.JPG
   :scale: 70%

**Obs.:** Para este cenário **não** serão criadas fichas para a **operação**.

**4. Nenhum**

Geração da Ficha de análise para a ordem de produção padrão configurada no campo **'Ficha de análise'** como  **'Nenhum – NM'**.

.. image :: /_static/BR\ One\ Qualidade/Processo/Automatico\ Prod/PAPadrão/PAP10.JPG
   :scale: 70%

Na liberação e na entrada de PA da OP 655, **não é gerado nenhuma ficha de análise**.
