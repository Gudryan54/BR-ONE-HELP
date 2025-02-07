Entrada de Componentes
~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta tela é possível realizar a entrada de componentes.

Para acessar essa tela pode utilizar as opções:


- Através do menu **Produção -> Entrada de Componentes**;


- Através do Terminal de Apontamentos;


- Através do botão direito na Ordem de Produção de Desmontagem liberada.


.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Aspose.Words.3b7aaf2d-3eae-4028-93b3-b9dcd6d4ba40.002.png


Para realizar a entrada de componentes, basta informar o **“Nº ordem de produção”** e a **“Seq. operação”**, e ao preencher as linhas com os componentes dessa operação, a quantidade do(s)item(ns) será carregada.

O CFL (Choose From List) do campo **“Nº ordem produção”** será carregado da seguinte forma:

- Quando o campo estiver vazio, apenas aparecerão as 100 primeiras OPs para seleção.

- Quando o campo estiver com \*, aparecerão todas as OPs disponíveis para entrada de componentes.

- Quando houver algum filtro, aparecerão todas as OPs de acordo com o filtro informado.


**OBS.:** Somente serão carregadas no CFL, OPs do tipo **Desmontagem**, que possuam o status **"Liberada"**.

Caso o usuário tente adicionar uma entrada de componentes sem informar uma OP, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img01.png


*BR One :: Informe uma ordem de produção.*

Caso o usuário tente adicionar uma entrada de componentes sem informar uma operação, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img02.png


*BR One :: Informe uma operação.*

Caso o usuário tente adicionar uma entrada de componentes com linhas faltando o número do item, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img03.png


*BR One :: Informe o número do item.*

Caso o usuário tente adicionar uma entrada de componentes com linhas faltando o depósito, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img04.png


*BR One :: Informe o depósito de destino.*

Caso o usuário tente adicionar uma entrada de componentes com linhas faltando a quantidade, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img05.png


*BR One :: A quantidade deve ser maior que zero.*

*BR One :: Informe uma data do documento.*

É possível também que a ordem de produção tenha seu status alterado enquanto a tela de entrada de componentes estiver aberta:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img06.png


*BR One :: Ordem de produção deve estar liberada para que seja possível realizar a entrada de componentes.*

Existe a possibilidade de realizar o apontamento para um item alternativo previamente cadastrado na tela Estoque > Administração de itens > Itens alternativos ou diretamente através do botão direito no **“Cadastro do item”**, opção **“Itens alternativos”**.

Para isto, basta que a flag “Permitir edição após liberação” esteja marcada na OP de Desmontagem.

Se o usuário estiver tentando inserir um item que esteja cancelado na OP, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Aspose.Words.3b7aaf2d-3eae-4028-93b3-b9dcd6d4ba40.010.png


*BR One :: Item selecionado na linha x está cancelado na OP. Selecionar itens alternativos pressionando CTRL + TAB no campo n° do item.*

Para inserir um item alternativo, o item pode ou não estar cancelado. Basta criar uma entrada de componentes para o item e, se desejar trocá-lo, pressione CTRL + TAB e o item atual poderá ser trocado por um alternativo a ele.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img07.png


O item será carregado na tela de entrada de componentes:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img08.png


Se o usuário pressionar CTRL + TAB no item que deseja trocar, mas a flag "Permitir edição após liberação" na OP estiver desmarcada, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Aspose.Words.3b7aaf2d-3eae-4028-93b3-b9dcd6d4ba40.013.png


*BR One :: Não é permitido selecionar itens alternativos pois a OP selecionada não permite edição após a liberação.*

A flag **“Selecionar insumos manualmente”** virá desmarcada.

Quando ela estiver marcada, o usuário irá conseguir informar os insumos que possuem **“Método baixa”** iguala a **“Manual”**, para isso será necessário inserir uma nova linha e selecioná-los manualmente.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img09.png


Se houver itens duplicados na OP, ao selecioná-lo, será aberta uma nova tela para ser escolhido o item. Ao selecionar os insumos manualmente, a quantidade carregada será a quantidade pendente.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img10.png


.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img11.png


Quando a flag estiver desmarcada, os insumos serão carregados normalmente.

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img08.png


A flag pode ser marcada ou desmarcada a qualquer momento. Esta tela possui configurações que podem alterar seu comportamento.

Ao clicar no botão **“Calcular”**, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Apontamento/Entrada\ de\ Componentes/Img12.png


*BR One :: As quantidades dos insumos serão recalculadas de acordo com a quantidade informada. Continuar?*

Ao clicar em **“Sim”**, as quantidades dos itens serão recalculadas de acordo com a quantidade de PA.

Por exemplo, se a quantidade base do componente for 0,006 e no campo **“Quantidade PA”** for digitado 2, a mensagem acima será exibida, e se for clicado em **“Sim”**, a quantidade do item será recalculada com o valor 0,012.

**Cálculo:** 2 * 0,006 = 0,012