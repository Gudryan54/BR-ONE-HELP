Assistente de cancelamento de retorno
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

No assistente de cancelamento, é possível cancelar todos os documentos gerados no processo de retorno. 

Para acessar a tela de Assistente de cancelamento de retorno é necessário ir  no menu:

**Produção -> Beneficiamento -> Compras -> Assistente de cancelamento de retorno**

A tela de **BR One :: Assistente de cancelamento de retorno** exibe todos os documentos já emitidos, cada linha corresponde a um retorno gerado que pode ter até 3 documentos por linha. Podemos filtrar os retornos pelo **Nº NF de Entrada** e **Fornecedor**.

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Compra/Cancelamento\ de\ Retorno/img01.png
   :scale: 80%

Quando é realizado o cancelamento dos documentos vários processos são cancelados de acordo com o tipo de retorno, são eles:

**Retorno de Documentos separados, são gerados os cancelamentos:**

- Cancelamento da Nota Fiscal de Entrada (Item de serviço);

- Cancelamento do Recebimento de Mercadoria (Componentes peças boas);

- Cancelamento do Recebimento de Mercadoria (Componente não Industrializado e Refugo);

- Cancelamento da saída de insumos (Componentes peças boas), e gera uma entrada de mercadoria no depósito de terceiros;

- Cancelamento da transferência de estoque dos materiais não industrializados (Transferência trocando os depósitos ou com os mesmos depósitos e quantidade negativa);
 
- Cancelamento da saída de insumos (Componente refugado), e gera uma entrada de mercadoria no depósito de terceiros;

- Cancelamento do rateio de terceiro.


**Retorno de Mesmo documento, são gerados os cancelamentos:**

- Cancelamento da NF entrada (Item de serviço + Componentes peças boas);

- Cancelamento do Recebimento de Mercadoria (Componente não Industrializado e Refugo);

- Cancelamento da saída de insumos (Componentes peças boas), e gera uma entrada de mercadoria no depósito de terceiros;

- Cancelamento da transferência de estoque dos materiais não industrializados (Transferência trocando os depósitos ou com os mesmos depósitos e quantidade negativa);

- Cancelamento da saída de insumos (Componente refugado), e gera uma entrada de mercadoria no depósito de terceiros;

- Cancelamento do rateio de terceiro.

Exemplo abaixo de um processo do tipo de retorno **DOCUMENTOS SEPARADOS** cancelado:

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Compra/Cancelamento\ de\ Retorno/img02.png
   :scale: 80%