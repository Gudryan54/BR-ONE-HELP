Estornos de Produção
~~~~~~~~~~~~~~~~~~~~~

Nesta janela é possível realizar os estornos de entradas de PA, saídas de insumos, estorno por refugo, saídas de PA e entradas de componentes.

Para acessar o Estornos de produção é necessário ir  no menu:

**Produção -> Estornos de Apontamento**

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img01.png

	
Os campos do cabeçalho servem como filtro. O resultado será trazido nas linhas. A primeira coluna possui campos de seleção. O usuário irá selecionar as linhas que deseja estornar e irá pressionar o botão **Estornar**.	

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img02.png

	
- **Entrada de PA**

Quando ocorre o estorno de uma entrada de PA, dois lançamentos é realizado. Primeiro é realizado a **Saída de mercadoria** do PA, com os mesmo valores da entrada original. E posteriormente é realizado a **Entrada de mercadoria** dos componentes do PA, com os mesmo valores que foi utilizado para PA.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img03.png

	
.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img04.png


Se for feito o estorno de uma entrada de PA que utilizou valor do rateio em seu custo, ao estornar a entrada de PA, todos os rateios utilizados serão marcados como pendentes novamente.

- **Saída de Insumos**

Ao estornar uma **Saída de insumos** (Saída de mercadoria), será feito o lançamento de uma **Entrada de mercadoria** dos componentes (Insumos), com os mesmos valores da saída e os documentos serão vinculados.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img05.png


.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img06.png


- **Estorno por Refugo**

Ao estornar um estorno por refugo, será feita uma **Entrada de mercadorias** para o PA e uma **Saída de mercadorias** para o componente, estornando o apontamento de refugo.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img07.png


.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img08.png


Com o processo de apontamento de refugo, há também a possibilidade de interferir no estorno de entrada de PA.

**Exemplo:**

Para uma Ordem de produção (OP) 536 com quantidade planejada de 100 peças, foi realizada duas entradas de PA de 15 cada, sendo assim, foi apontado 30 entradas de PA. Foi feito um apontamento de refugo de 20, totalizando então apenas 10 entradas de PA. 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img09.png

	
Na tela **"BR One :: Estornos de produção"**, ao filtrar por Entrada de PA, as duas entradas feitas (PA) de 15 cada estarão disponíveis para estorno. Mas, se atualmente há apenas 10 entradas, não será possível fazer o estorno das entradas. 

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img10.png

	
Caso o usuário tente realizar o estorno das entradas, a seguinte mensagem aparecerá na tela de erros:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img11.png


*Erro ao estornar apontamento de PA nº xxx : Tentativa de estornar quantidade igual a 15. Está disponível para estorno apenas 10.*

- **Saída de PA**

Ao estornar uma saída de PA, será feito o lançamento de uma **Entrada de mercadoria** para o PA e uma **Saída de mercadoria** para os componentes, com os mesmos valores, onde os documentos serão vinculados.


.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img12.png

	
.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img13.png

	
- **Entrada de componentes**

Ao estornar uma entrada de componentes, será feito o lançamento de uma saída de mercadoria para os componentes, com os mesmos valores, onde os documentos serão vinculados.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img14.png

	
.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Estorno\ de\ Apontamento/img15.png

