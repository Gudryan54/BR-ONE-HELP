Estorno de Produção
~~~~~~~~~~~~~~~~~~~

Na tela Estornos de Produção, selecione no campo **Tipo de OP** a opção **Retrabalho**.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img01.png
   :scale: 80%

Ao filtrar, poderá visualizar na grid os documentos para estorno na ordem decrescente da ultima OP para a primeira.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img02.png
   :scale: 80%

Quando for filtrado por **Entrada de PA**, apenas aparecerão entradas de mercadoria, reavaliação e saída de mercadoria (refugo).

Ao realizar o estorno de entrada de mercadoria que também foi feita uma saída de mercadoria para o mesmo item, será feito o estorno da entrada gerando um documento de saída e o estorno da saída gerando um documento de entrada.

No exemplo fornecido, uma **Entrada de mercadoria** de número **653** foi criada, o que também gerou a criação da **Saída de insumos** de número **930** correspondente.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img03.png
   :scale: 80%

Ao estornar a **Entrada de mercadoria** do número **653**, o sistema também realizará o estorno da **Saída de insumos** do número **930** associado a ela. No entanto, na tela de **BR One :: Estornos de Produção**, somente a **Entrada de mercadoria** será exibida para que o usuário possa realizar o estorno.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img04.png
   :scale: 80%

Ao estonar a entrada, será criado um documento de saída correspondente, e o lote/série utilizado na entrada será associado a esse documento de saída.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img05.png
   :scale: 80%

E, também será estornada a saída, criando uma entrada com o mesmo lote/série utilizado na saída.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img06.png
   :scale: 80%

Ao estornar uma reavaliação de estoque, será criada uma reavaliação de estoque, porém, com o valor da coluna Débito/Crédito negativo.

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img07.png
   :scale: 80%

.. image:: /_static/BR\ One\ Produção/Processo/Retrabalho/Estorno\ de\ Produção/img08.png
   :scale: 80%

A saída de mercadorias criada ao fazer uma entrada de PA como refugo será estornada como uma entrada de mercadorias.

