
Scripts adicionais
~~~~~~~~~~~~~~~~~~~~~~~~~~


Para que a customização que necessita de script específico (que não seja de produto) funcione corretamente, é necessário executar manualmente os scripts.

A conexão possui parâmetros diferentes de acordo com a versão do banco de dados (SQL Server ou SAP HANA), conforme detalhes abaixo:

**SQL Server**

· Server: Nome ou IP do servidor e instância do banco (caso exista).

· Usuário: Nome de usuário para conexão no SQL Server.

· Senha: Senha do usuário.


.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.003.png


**SAP HANA**


· Server: Nome ou IP do servidor seguidos do número da porta. 

· Usuário: Nome de usuário com autorização para criação de objetos no banco de dados.
 
· Senha: Senha do usuário.

.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.004.png

**Importante:**

Os scripts devem ser executados sempre no computador onde está instalado o SAP Business One Client. Caso execute a partir de outro computador, é imprescindível que o driver ODBC HANA esteja instalado na máquina onde se irá executar o script, e deve ser observada a plataforma correta de instalação:

· Para o sistema operacional 32-bit, instalar a versão 32 bits do driver HDBODBC32.

· Para sistema operacional 64-bit, instalar a versão 64 bits do driver HDBODBC.

**Script não instalado** 

Caso a instalação de algum script essencial ao add-on tenha falhado, será exibida a seguinte mensagem ao usuário e o mesmo deverá providenciar a versão especificada do script para realizar a instalação do mesmo:

.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.029.png

**Versão do script**

Do script incorreta É possível que a versão do script instalada na base do cliente não seja a versão exigida pelo add-on. Neste caso, será necessária a providência da versão específica, e a mensagem de erro exibida será a seguinte:

.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.030.png