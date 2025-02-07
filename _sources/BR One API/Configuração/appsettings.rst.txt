Configurar "appsettings.json"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O arquivo **'appsettings.json'** em uma aplicação RESTful (ou REST API) geralmente é usado para armazenar configurações e informações de configuração para a aplicação. 

Ele é parte integrante do ambiente ASP.NET Core e é usado para definir várias configurações, como conexões de banco de dados, configurações de log, configurações de autenticação, e outras variáveis de ambiente.

No BR One API não é diferente, o **'appsettings.json'** deve ser configurado corretamente para garantir a conformidade da aplicação. 

Segue abaixo exemplo do **'appsettings.json'** disponível para configuração:

.. code-block:: json

	{
	  "Logging": {
		"Seq": {
		  "Url": "http://localhost:5341/"
		}
	  },
	  "AllowedHosts": "*",
	  "OpenApiInfo": {
		"Title": "BR One API",
		"Description": "APIs REST para interação com os módulos do BR One através de integrações via requisições web.",
		"Contact": {
		  "Name": "Uppertools",
		  "Email": "contato@uppertools.com.br"
		}
	  },
	  "JwtSettings": {
		"Secret": "81b4dada80b2f4126ea7244d328c2270",
		"ExpiracaoSegundos": 600,
		"Emissor": "BROne",
		"ValidoEm": "https://localhost"
	  },
	  "Kestrel": {
		"EndPoints": {
		  "Http": {
			"Url": "http://localhost:4300/"
		  },
		  "Https": {
			"Url": "https://localhost:4301/"
		  }
		}
	  },
	  "FeatureManagement": {
		"EnableVersionInterceptor": false
	  },
	  "ServerCredentials": {
		"Type": "HANA",
		"Driver": "HDBODBC",
		"Server": "hanab1:30015",
		"User": "SYSTEM",
		"Password": "1234",
		"EncryptedPassword": null
	  },
	  "ServiceLayer": {
		"Url": "https://hanab1:50000/b1s/v1",
		"User": "manager",
		"Password": "1234",
		"EncryptedPassword": null
	  }
	}

Segue abaixo detalhe sobre os campos disponíveis no **appsettings.json**:

.. code-block:: json
	
	{
	  "Logging": {
		"Seq": {
		  "Configurations": "Configurações para integração com o Seq, uma plataforma de registro e análise de logs.",
		  "Url": "O endereço onde o Seq está sendo executado (http://localhost:5341/)."
		}
	  },
	  "AllowedHosts": {
		"Description": "Este campo indica quais hosts são permitidos para acessar a aplicação. No exemplo, o valor \"*\" indica que qualquer host é permitido."
	  },
	  "OpenApiInfo": {
		"Title": "Título da API (\"BR One API\").",
		"Description": "Uma descrição breve da API.",
		"Contact": {
		  "Name": "Nome da organização ou pessoa de contato (\"Uppertools\").",
		  "Email": "Endereço de e-mail de contato (\"contato@uppertools.com.br\")."
		}
	  },
	  "JwtSettings": {
		"Secret": "A chave secreta usada para assinar os tokens JWT.",
		"ExpiracaoSegundos": 600,
		"Emissor": "O emissor dos tokens JWT (\"BROne\").",
		"ValidoEm": "O URI válido para o qual os tokens são emitidos (\"https://localhost\")."
	  },
	  "Kestrel": {
		"Description": "Configurações para o servidor web Kestrel, que é um servidor web embutido no ASP.NET Core.",
		"EndPoints": {
		  "Http": {
			"Description": "Define as configurações para o endpoint HTTP.",
			"Url": "O endereço em que o servidor Kestrel estará ouvindo (http://localhost:4300/)."
		  },
		  "Https": {
			"Description": "Define as configurações para o endpoint HTTPS.",
			"Url": "O endereço em que o servidor Kestrel estará ouvindo em HTTPS (https://localhost:4301/)."
		  }
		}
	  },
	  "FeatureManagement": {
		"Description": "Configurações para a gestão de funcionalidades (feature flags).",
		"EnableVersionInterceptor": false
	  },
	  "ServerCredentials": {
		"Description": "Configurações de credenciais do servidor de banco de dados.",
		"Type": "O tipo de banco de dados (\"HANA\").",
		"Driver": "O driver do banco de dados (\"HDBODBC\").",
		"Server": "O nome do servidor e a porta separados por dois pontos (\"hanab1:30015\").",
		"User": "O nome de usuário do banco de dados (\"SYSTEM\").",
		"Password": "A senha do banco de dados (\"1234\").",
		"EncryptedPassword": "Neste exemplo, não há uma senha criptografada."
	  },
	  "ServiceLayer": {
		"Description": "Configurações para a camada de serviço.",
		"Url": "O endereço da camada de serviço (\"https://hanab1:50000/b1s/v1\").",
		"User": "O nome de usuário para autenticação na camada de serviço (\"manager\").",
		"Password": "A senha para autenticação na camada de serviço (\"1234\").",
		"EncryptedPassword": "Neste exemplo, não há uma senha criptografada."
	  }
	}
