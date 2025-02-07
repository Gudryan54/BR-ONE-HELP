Processo de Importação
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para acessar a tela **Processo de Importação**, é necessatio ir ao menu:

**Compras -> Processo de Importação**

.. image:: /_static/BR\ One\ Importação/Processo/Processo\ de\ importação/Aspose.Words.2f730182-e58c-4927-8a2d-d4fa11683465.001.png
   :scale: 80%


- **Cabeçalho**

A tela que será aberta contém no cabeçalho os dados a serem preenchidos (obrigatoriamente):

- Tipo de Importação
    -	Direta
    -	Conta e ordem:
         - Caso o usuário selecione o tipo **"Conta e ordem"**, o layout da Tela será alterado, contendo as funcionalidades para atender o processo de conta e ordem.

- Fornecedor (código do PN) 

- Despachante (código do PN) 

- Tipo de moeda e a filial (apenas no caso de multi-filiais)

.. image:: /_static/BR\ One\ Importação/Processo/Processo\ de\ importação/Aspose.Words.2f730182-e58c-4927-8a2d-d4fa11683465.002.png
   :scale: 80%


O campo **Nº** indica o número do documento criado, o campo **Status** mudará de acordo com o processo de importação, sendo alterados **automaticamente** conforme as gerações dos documentos dentro do processo de importação. Os Status possíveis serão os seguintes:

- **Aberto:** Receberá este status quando criado um documento para o processo de importação, informando Fornecedor, Despachante e a Moeda;
- **Proforma:** Receberá este status quando copiado os itens dos pedidos de compra para tela do processo de importação;
- **Invoice:** Receberá este status quando for gerada a Invoice;
- **LCM Desp. Nac.:** Receberá este status quando for gerado o LCM de despesas adicionais + impostos no processo de “Conta e Ordem”.
- **Nacionalização:** Receberá este status quando for gerada a NF de Nacionalização (NF de Entrada);
- **Recebimento de Mercadoria:** Receberá este status quando for gerada a Transferência de estoque entre os depósitos usado no processo de importação para o estoque de venda; 
- **Despesas de Importação:** Receberá este status quando for gerada as Despesas de importação BR One;
- **Fechamento de Numerário:** Receberá este status quando realizado o LCM (Lançamentos contábeis) de fechamento do despachante;
- **Conciliação de importação:** Receberá este Status quando for gerado o processo de conciliação de importação.
- **Fechamento de importação:**  Receberá este status após o usuário realizar o Fechamento do processo de importação.
- **Fechado:** Receberá este status quando o processo de importação for fechado;
- **Cancelado:** Receberá este status quando o processo de importação for cancelado;

O campo **Data de criação** será a data que o processo foi criado e o campo **Última alteração**  terá a data em que o processo foi alterado pela última vez.

O campo **Nº proc. Importação** é um campo livre para o usuário inserir o número do processo de importação que desejar.

O campo **Status canal** poderá ser utilizado para sinalizar o processo de importação. Há 4 opções: **Canal verde, Canal amarelo, Canal vermelho** e **Canal cinza**.

.. image:: /_static/BR\ One\ Importação/Processo/Processo\ de\ importação/Aspose.Words.2f730182-e58c-4927-8a2d-d4fa11683465.003.png
   :scale: 80%


.. image:: /_static/BR\ One\ Importação/Processo/Processo\ de\ importação/Aspose.Words.2f730182-e58c-4927-8a2d-d4fa11683465.004.png
   :scale: 80%


.. image:: /_static/BR\ One\ Importação/Processo/Processo\ de\ importação/Aspose.Words.2f730182-e58c-4927-8a2d-d4fa11683465.005.png
   :scale: 80%


.. image:: /_static/BR\ One\ Importação/Processo/Processo\ de\ importação/Aspose.Words.2f730182-e58c-4927-8a2d-d4fa11683465.006.png
   :scale: 80%


O campo **Receb. de mercadoria** poderá ser preenchido com **Total** ou **Parcial**.

Mas ele apenas terá valor após ser feito um **Recebimento de mercadorias.** 

O campo ficará como:

**Total**: quando todos os recebimentos de mercadoria forem criados.

**Parcial**: será quando houver recebimentos pendentes.


