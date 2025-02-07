Conclusão dos apontamentos de produção
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint, possibilita realizar a conclusão de um apontamento de produção, logo, usuário deve utilizar o método **"PATCH"** e enviar os dados do JSON abaixo:

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/025.png
   :scale: 75%
   :align: center

| \

.. code-block:: json

   [
     {
       "docNumApontamento": 0,
       "docEntryOrdemProducao": 0,
       "sequenciaOperacao": 0
     }
   ]

Segue abaixo exemplo de JSON preenchido e enviado na API:

.. code-block:: json

   [
     {
       "docNumApontamento": 129,
       "docEntryOrdemProducao": 761,
       "sequenciaOperacao": 10
     }
   ]

Apontamento de produção após ser concluído pela API:

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/028.png
   :scale: 70%
   :align: center

| \