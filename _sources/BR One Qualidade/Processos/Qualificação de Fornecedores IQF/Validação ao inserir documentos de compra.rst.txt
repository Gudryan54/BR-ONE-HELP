Validação ao inserir documentos de compra
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Quando o flag **Qualificação/Item fornecedor** estiver marcado, ao utilizar um fornecedor não qualificado em algum documento de compra, se a configuração **Fornecedor não qualificado** estiver como **BLOQUEAR**, o documento não será inserido.

.. image:: /_static/BR\ One\ Qualidade/Processo/Qualificação\ de\ fornecedores/Aspose.Words.67881489-10be-41d8-9938-4848d61ce893.044.png
   :scale: 100%

.. image:: /_static/BR\ One\ Qualidade/Processo/Qualificação\ de\ fornecedores/Aspose.Words.67881489-10be-41d8-9938-4848d61ce893.045.png
   :scale: 100%

Caso esteja como **ALERTAR**, o seguinte alerta será mostrado, porém, o documento será inserido:

.. image:: /_static/BR\ One\ Qualidade/Processo/Qualificação\ de\ fornecedores/Aspose.Words.67881489-10be-41d8-9938-4848d61ce893.046.png
   :scale: 100%

*BR One :: ALERTA: o fornecedor "x" não está qualificado.*

Quando um documento com fornecedor não qualificado tem como origem um documento que já está adicionado, não será realizada uma nova validação no documento destino.

Os documentos que serão validados são:

- Contrato guarda-chuva de compra 
- Solicitação de compra 
- Oferta de compra 
- Pedido de compra 
- Recebimento de mercadoria 
- Pedido de Solicitação de mercadoria
- Devolução de mercadoria 
- Fatura de Adiantamento de contas a pagar 
- NF de Entrada 
- Devolução de NF de Entrada 
- NF de Recebimento futuro 
- Todos os documentos que fazem parte do Processo de Importação