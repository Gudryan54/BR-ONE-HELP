Exclui uma linha de conteúdo na Ordem de Produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint permite excluir uma linha no GRID da Ordem de Produção, para realizar a exclusão ao usuário deve informar os campos '**docNumOrdemProducao**' e o campo '**lineId**'.

.. image:: /_static/BR\ One\ API/OP/089.png
   :scale: 70%

A OP selecionada deve possuir status '**Planejada**', caso contrário a API exibirá uma validação que impedirá a exclusão da linha. 