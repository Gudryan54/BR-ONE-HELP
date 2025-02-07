Boas práticas de saldo com itens de terceiro
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Houve uma transição de ERP para o BR One e existem processos de Beneficiamento de Compra em aberto? Siga atentamente as orientações abaixo para assegurar uma transição suave, e a correta finalização do processo de **Beneficiamento de Compra** utilizando o BR One. 

Segue sugestões:

- **Inserir um recebimento de mercadoria simbólico de peças não industrializadas e depois emitir novamente a remessa pela Ordem de Produção.**

Usuário deve inserir um recebimento de mercadorias não industrializados simbólico, onde os componentes desse documento devem ser iguais aos componentes utilizados no processo antigo de beneficiamento de compra, as quantidades devem ser equivalentes ao enviado na remessa e deve ser utilizada a **Utilização** que está configurada como **Utilização para dev. mat. não indust.**

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Compra/Saldos\ iniciais/01.png
   :scale: 100%

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Compra/Saldos\ iniciais/02.png
   :scale: 70%

Ao adicionar o **Recebimento de mercadorias** acima conforme orientações, será aberto a tela de **Transferência de estoque** com todas as informações preenchidas, onde irá transferir os itens do depósito de terceiro (depósito do fornecedor) para o depósito próprio padrão do item conforme filial escolhida.

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Compra/Saldos\ iniciais/03.png
   :scale: 80%

Ao adicionar a **Transferência de estoque**, as quantidades que foram enviadas anteriormente através da remessa do processo estarão disponíveis novamente no depósito próprio, permitindo assim, que o processo seja reiniciado utilizando o BR One.

- **Inserir uma transferência de estoque do deposito de terceiro para o próprio e criar a remessa na Ordem de Produção.**

A **Transferência de estoque** deve conter todos os componentes do processo de beneficiamento de compra, e as quantidades devem ser equivalentes ao enviado na remessa, porém, os depósitos dever ser contrários, no caso o campo **Do depósito** deve ser o depósito de terceiro (depósito do fornecedor) e o campo **Para depósito** deve ser o depósito próprio.

Segue abaixo exemplo de **Transferência** de estoque gerada manualmente, levando em consideração as informações citadas acima.

.. image:: /_static/BR\ One\ Produção/Processo/Beneficiamento\ de\ Compra/Saldos\ iniciais/04.png
   :scale: 80%
   
Após inserir a **Transferência de estoque** acima, usuário deve iniciar novamente o processo Beneficiamento de Compra através da Ordem de Produção adicionada pelo BR One, com isso o processo irá ocorrer normalmente.

- **Cancelar remessa no processo antigo e inserir novamente a Remessa através do BR One.**

Usuário deve cancelar a remessa criada no processo de Beneficiamento de Compra utilizando o sistema ERP no qual a mesma foi gerada e após, poderá iniciar o processo utilizando o BR One.

- **Finalizar o processo de retorno da remessa no sistema antigo.**

Usuário deve finalizar o processo de retorno da remessa aberto no sistema ERP no qual o mesmo foi iniciado.

