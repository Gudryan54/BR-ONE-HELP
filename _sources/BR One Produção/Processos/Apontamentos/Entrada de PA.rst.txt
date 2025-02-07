Entrada de Produto Acabado
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta tela é possível realizar a entrada de produtos acabados.

Para acessar essa tela pode utilizar as opções:


- Através do menu **Produção -> Entrada de produto acabado**;


- Através do Terminal de Apontamentos;


- Através do botão direito na Ordem de Produção liberada.


.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.002.png


Para realizar a entrada de produto acabado, basta informar os campos **"Nº da ordem de produção"**, o **"Depósito"** e a **"Quantidade"**. 

O CFL (Choose From List) do campo **“Nº ordem produção”** será carregado da seguinte forma:

- Quando o campo estiver vazio, apenas aparecerão as 100 primeiras OPs para seleção.

- Quando o campo estiver com (*), aparecerão todas as OPs disponíveis para entrada de PA.

- Quando houver algum filtro, aparecerão todas as OPs de acordo com o filtro informado.

**OBS.:** Ordens de produção que possuem a flag **"Ignorar no fechamento de custos"** marcada não serão carregadas no CFL. (Fechamento de custo contábil (xxx)).

Caso o usuário tente adicionar uma entrada sem informar o número da OP, a seguinte mensagem será exibida ao usuário:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.003.png


*BR One :: Informe uma ordem de produção.*

Para o campo **"Depósito"**, caso a base seja multifilias, só poderão ser selecionados depósitos que pertençam à mesma filial do depósito informado na ordem de produção. 

Caso o parâmetro **"Bloquear alteração do campo depósito"** esteja desmarcado, e o usuário tente adicionar uma entrada sem informar o depósito, a seguinte mensagem será exibida ao usuário:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.004.png


*BR One :: Informe um depósito.*

Caso o usuário tente adicionar uma entrada sem informar uma quantidade, a seguinte mensagem será exibida ao usuário:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.005.png


*BR One :: Informe uma quantidade maior que zero.*

Caso o usuário tente adicionar uma entrada de uma ordem de produção que não possua componentes, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.006.png


*BR One :: Não é possível realizar uma Entrada de PA para uma OP sem componentes.*

Caso o usuário tente adicionar uma entrada sem data, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.007.png


*BR One :: Informe uma data do documento.*

Caso o usuário tente adicionar uma entrada e as contas contábeis **"Conta de material em processo"** e/ou **"Conta GGF arbitrado"** estiverem com a flag **"Bloquear lançamento manual"** marcada, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.008.png


*BR One :: Para realização deste processo, o parâmetro "Bloquear lançamento manual" deve estar desmarcado na conta "x"*

Essa situação pode ser revertida, marcando a flag **"Permitir a entrada de PA sem componentes ativos (custo zero)"** (**xxx**).

Ao realizar uma entrada de produto acabado, é feita uma entrada de mercadoria com o item produzido pela ordem de produção, porém, o caminho realizado pelo addon, varia conforme o tipo de ordem de produção.

-**Entrada de PA para uma OP Padrão**

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.010.png


Na ordem de produção padrão, ao adicionar entrada de PA, é realizada:

- Saída de insumos para os componentes que estejam configurados como baixa por explosão; 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.011.png


- Entrada de mercadoria para o PA;

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.012.png


- LCM do GGF arbitrado (se configurado);

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.013.png


- Ficha de analise do PA (se configurado).



-**Entrada de PA para uma OP de Retrabalho**

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.014.png


Na ordem de produção de retrabalho, deve-se levar em consideração o tipo de administração do PA, se o mesmo for administrado por nenhum, ao adicionar a entrada de PA, é realizada:

- Saída de insumos para os componentes que estejam configurados como baixa por explosão; 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.011.png


- Reavaliação de estoque para o PA;

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.016.png


- LCM do GGF arbitrado (se configurado);

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.013.png


- Transferência de estoque: Transfere o item do depósito de retrabalho para o depósito desejado da filial no qual o usuário está logado.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.015.png


- Ficha de analise do PA (se configurado).


Quando o PA é administrado por **lote/série**, e não é realizado a troca de número de lote/série, o processo de entrada é igual ao demonstrado para PA administrado por nenhum, mas se realizar o troca do número do lote ou série, ao adicionar a entrada de PA, é realizada:

- Saída de insumos para os componentes que estejam configurados como baixa por explosão; 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.011.png


- Saída de mercadorias (PA): Baixa do mesmo do depósito de retrabalho

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.018.png


- Entrada de mercadoria (PA): Faz a entrada do **“novo”** lote do PA no depósito de retrabalho

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.019.png


- LCM do GGF arbitrado (se configurado);

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.013.png


- Transferência de estoque: Transfere o item do depósito de retrabalho para o depósito desejado da filial no qual o usuário está logado, deve ser escolhido o número de lote/série informado na entrada de mercadoria.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.015.png



.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.017.png


*BR One :: O(s) lote(s) selecionado(s) precisa(m) ser o(s) mesmo(s) criado(s) na entrada de mercadoria ["x" (x)].*

- Ficha de analise do PA (se configurado).


**Entrada de PA para uma OP de Beneficiamento de Compra**

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.020.png


Na ordem de produção de beneficiamento de compra, ao adicionar entrada de PA, é realizada:

- Saída de insumos para os componentes que estejam configurados como baixa por explosão; 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/image_2023_07_27T17_22_13_628Z.png


- Entrada de mercadoria para o PA: No depósito de terceiro;

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/entradabene.JPG


- Transferência de estoque: Transfere o PA do depósito de terceiro para o depósito padrão do item ou qualquer outro depósito da filial no qual o usuário esteja logado;

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/image_2023_07_27T17_23_38_017Z.png


- Ficha de analise do PA (se configurado).

A transferência de estoque pode ser realizada por DI, dependendo da configuração de beneficiamento, caso contrário a mesma é adicionada manualmente após a adição da entrada de mercadoria. 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.021.png


Para o documento de transferência do estoque é necessário salientar que a mesma é gerada conforme a configuração da tela de configurações de documento, se estiver configurado para gerar pedido de transferência de estoque, este será gerado após a adição da entrada de mercadoria, obrigando neste caso que o usuário realize a adição manual da transferência de estoque.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ PA/Aspose.Words.7153a72b-6582-4c20-bda9-6c733d4a6e6c.022.png

