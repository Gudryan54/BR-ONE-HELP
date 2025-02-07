Recebimento
^^^^^^^^^^^^

.. image:: WMS-AutorizaçõesRecebimento.png
   :align: center

| \

Na seção Recebimento, você encontrará todas as autorizações que adicionam comportamentos no módulo Recebimento e no SAP.

| \

Autorização Usuários - alerta de divergência
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. image:: WMS-AutUsuárioRecb.png
   :align: center

| \

Nesta autorização, caso seja definido "Sem autorização" o usuário não terá acesso a tela **BR One :: Usuários - alerta de divergência** da aba Recebimento. Para permitir o acesso, defina a autorização como "Autorização total".

| \

Autorização Visualiza quantidade quando conferência as cegas estiver ativa
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. |image-link| image:: WMS-AutConfCegas.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AutConfCegas.png" style="width: 300px;" />
   </div>

| \

Quando nas Configurações WMS, na aba Recebimento, o parâmetro **Utilizar conferência às cegas** estiver ativo, definindo a autorização **Visualiza quantidade quando conferência as cegas estiver ativa** como "Autorização total", o usuário conseguirá visualizar as quantidades do documento.

| \

Autorização Realizar recebimento quando houver divergência
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. |image-link2| image:: WMS-AutConclDiver.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AutConclDiver.png" style="width: 300px;" />
   </div>

| \

No menu Conferência, caso o usuário conclua uma conferência com divergência, possuindo "Autorização total", o documento de destino será gerado definitivo no SAP. Sendo "Sem autorização", o usuário concluindo com divergência, o documento de destino será gerado como esboço.

| \

Autorização Permitir acesso ao menu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. |image-link3| image:: WMS-AutPermiteAcessRecb.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../../_images/WMS-AutPermiteAcessRecb.gif" style="width: 300px;" />
   </div>

| \

Na autorização **Permitir acesso ao menu Recebimento/Conferência**, se estiver definido "Sem autorização", não será permitido que o usuário acesse o menu. Pode ser dada "Autorização total" no menu que o usuário terá acesso permitdo.