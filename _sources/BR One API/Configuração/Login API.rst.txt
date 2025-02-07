Login API
~~~~~~~~~~~~~~~~~~
Para realizar o login na API é obrigatório criar uma senha de acesso na API diretamente no SAP com o BR One ativo. Para isso, deve-se acessar a tela "Usuário", e buscar o usuário desejado, e assim, definir uma senha no campo "Senha BR One API".

Essa senha será utilizado no Swagger ou Postman, para realizar o login na API e assim liberar o Token de acesso da API.

.. image:: /_static/BR\ One\ API/Login/006.png
   :scale: 90%
   :align: center

|

Para realizar o login na API o usuário deve utilizar a URL **'/api/v1/login'** e informar o JSON abaixo:

.. code-block:: json

   {
      "userName": "determina o usuário que irá utilizar a API",
      "password": "deve ser a senha cadastrada no campo 'Senha BR One API' no SAP para o usuário acima",
      "companyDB": "determina a base que será utilizada nos envios da API"
   }


**Exemplo**

.. image:: /_static/BR\ One\ API/Login/001.png
   :scale: 100%
   :align: center

|

Ao executar o JSON, será informado uma **'Bearer token'**:

.. image:: /_static/BR\ One\ API/Login/002.png
   :scale: 60%
   :align: center

|

Devemos copiar esse **'token'** (não copiar as “) e colar no campo **'Authorize'**, escrevendo o parâmetro **'Bearer'** na frente, ficando como exemplo abaixo:

**Bearer eyJhbGciOiJIUzI1NiIsI...**

.. image:: /_static/BR\ One\ API/Login/003.png
   :scale: 60%
   :align: center

|

.. image:: /_static/BR\ One\ API/Login/004.png
   :scale: 100%
   :align: center

|

Após colar o **'token'**, basta clicar em **'Authorize'**, assim será realizado o login na API.

.. image:: /_static/BR\ One\ API/Login/005.png
   :scale: 100%
   :align: center

|

Depois de efetuar o login, basta clicar em **'Close'** que a janela será fechada, caso seja clicado em **'Logout'** o usuário será deslogado.