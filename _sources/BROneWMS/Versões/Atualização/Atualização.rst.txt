Atualização da API
^^^^^^^^^^^^^^^^^^^

.. caution::

   Antes de realizar a atualização, é altamente recomendado realizar um backup da pasta!

.. image:: WMS-ParandoSite.png
   :align: center

| \

No IIS, dê "Stop" no site que será atualizada a API.

| \

.. image:: WMS-AtualizandoAPI.png
   :align: center

| \

Baixe a versão da API WMS, extraia e substitua os arquivos no diretório de instalação da API em **C:/inetpub**.

.. caution::

   Não substitua os arquivos **appsettings.json** e o **web.config**. Caso sejam substituídos, será necessário editar novamente os arquivos.
