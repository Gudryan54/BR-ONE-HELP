Operações - Calcular
~~~~~~~~~~~~~~~~~~~~~~~~

Através do botão **Operações -> Calcular** realiza o cálculo dos itens


.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.048.jpeg
   :scale: 80%


Se o usuário clicar no botão *Calcular* antes de copiar algum documento, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.049.jpeg
   :scale: 80%

*BR One :: Processo só permitido depois da realização da função "Copiar de".*

Se o usuário não informar nenhum valor no campo "Taxa de câmbio" e/ou "Lista de preço atual", a seguinte mensagem aparecerá:

.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.050.jpeg
   :scale: 80%

*BR One :: Os campos "Lista de preços atual" e "Taxa de câmbio" são de preenchimento obrigatório para este processo.*

A seguinte mensagem será exibida ao clicar em *Calcular,* informando que se o documento possuir muitas linhas, o cálculo poderá demorar alguns minutos:

.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.051.jpeg
   :scale: 80%

*BR One :: Caso o documento possua muitas linhas, o processo poderá demorar alguns minutos. Deseja atualizar os cálculos do documento?*



Ao clicar em *Sim*, os cálculos serão realizados e as seguintes mensagens serão exibidas:

.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.052.jpeg
   :scale: 80%

*Realizando cálculos do processo*

*BR One :: Realizando cálculos do processo. Linha [x] de [x]. Aguarde...*


Na barra de status será mostrada de 100 em 100 as linhas que foram processadas e também quantas linhas tem ao total.

O campo **Taxa de câmbio** não poderá ser modificado após o processo ***Copiar de** se ele tiver sido feito a partir da opção **Lista de preços**. Se o usuário tentar modificar o campo após copiar de uma lista de preços, a seguinte mensagem será exibida: 

.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.054.jpeg
   :scale: 80%

*BR One :: Campo não pode ser alterado quando o tipo da origem for "Lista de preços".*



Na caixa **Valor fixo**, a opção **Calcular** difere nos cálculos de **Antes** e **Depois**.


.. image:: /_static/BR\ One\ Produção/Processo/Formacao\ de\ preco\ de\ venda/Aspose.Words.2faae23a-b3e8-4b3e-832f-b2ae73293b58.055.png
   :scale: 80%


Ao selecionar a opção **Antes,** é realizada a soma da coluna **Base de cálculo** com os valores preenchidos no **Valor Fixo**. Com o resultado obtido, há a multiplicação pelos valores de **Impostos** e **Markup**: 


(Base De cálculo + (Frete + Custo Fixo + Outros)) \* (Impostos + Markup) = **R$ Sugerido** e **Valor a atualizar**.


Quando selecionada a opção **Depois,* é realizada a multiplicação da coluna **Base De cálculo** com **Impostos** e **Markup**. 
Com o valor obtido, é realizada a soma com os valores preenchidos no **Valor Fixo**: 


(Base De cálculo \* (Impostos + Markup)) + (Frete + Custo Fixo + Outros) = **Valor a Atualizar.** 