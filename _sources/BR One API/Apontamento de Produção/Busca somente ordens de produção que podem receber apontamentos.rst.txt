Busca somente ordens de produção que podem receber apontamentos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este endpoint realizar uma busca das ordens de produção que estão aptas a receber um apontamento. Para realizar a busca o usuário deve informar o '**DocNum**' da OP que deseja confirmar se pode receber um apontamento. 

.. image:: /_static/BR\ One\ API/Apontamento\ de\ Produção/013.png
   :scale: 60%
   :align: center

| \

Exemplo de retorno da API, onde é informado os dados da ordem de produção:

.. code-block:: json

   [
     {
       "docNum": 761,
       "docEntry": 761,
       "codigoItem": "pa lote",
       "nomeItem": "pa lote"
     }
   ]
