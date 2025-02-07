Ordem de Produção com Item Fictício
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Não é permitido criar Ordem de Produção para um roteiro de item fictício, apenas utilizar o item fictício em linhas de um outro item que não seja fictício.

Ao criar uma OP que contenha linhas de roteiro de item fictício, o roteiro é exibido dentro da operação, caso tenha itens ou recursos semelhantes, é realizado a soma das quantidades e tempo e exibido apenas em uma única linha, somente se o depósito ou método de baixa for diferente irá exibir 2 linhas repetidas.

**Exemplo:**

Roteiro de um **PA001** que consome o item **FT01** (item fictício) na **operação 10- Cortar,  FT02** (item fictício)  na **operação 20-Montar**

.. image:: /_static/BR\ One\ Produção/Processo/ItemFicticio/img7.JPG
   :scale: 80%

**Roteiro do item FT01**

.. image:: /_static/BR\ One\ Produção/Processo/ItemFicticio/img8.JPG
   :scale: 80%


**Roteiro do item FT02**

.. image:: /_static/BR\ One\ Produção/Processo/ItemFicticio/img9.JPG
   :scale: 80%


Dentro do roteiro do F02 possui um outro Fictício que é o FT03.

**Roteiro do item FT03**

.. image:: /_static/BR\ One\ Produção/Processo/ItemFicticio/img10.JPG
   :scale: 80%

Ao abrir a Ordem de Produção para o Item PA001, a estrutura ficará:

.. image:: /_static/BR\ One\ Produção/Processo/ItemFicticio/img11.JPG
   :scale: 80%

A **quantidade planejada e tempo planejado** será modificado de acordo com a quantidade que será **planejada do PA**.