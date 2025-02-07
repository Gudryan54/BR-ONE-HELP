Detalhamento do ecossistema
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Visão geral**

O BrOne Franquias é um add-on para o SAP Business One e possui um aplicativo vinculado a ele para facilitar o dia a dia operacional dos clientes do segmento de varejo de grandes franquias de restaurantes, pois além de proporcionar uma melhor organização aos franqueados, sua utilização versátil através de um aplicativo colabora com o ambiente dinâmico de um fast-food.

Para tal, a solução comporta outros add-ons dentro do sistema SAP, como por exemplo “T10 Extreme” da Skill e o “TaxOne” da Invent, que atualmente são utilizados para atuar na área fiscal, também se utiliza o add-on bancário BankPlus da Invent e um add-on de integração entre empresas, o InterCompany do SAP. 

Além disso, outra ferramenta imprescindível ao ecossistema são as APIs de mensageria fiscal (`Clique aqui <OOBJ>`_)e a de integração de cadastro de itens (Arcos Dourados), que criam uma ponte entre a base de dados da franquia no SAP Business One e um sistema ou base de dados externa, trazendo todas as informações requisitadas. Entre os demais serviços, utilizamos a plataforma do CardServices da empresa Atos Capital, que é a responsável pela conciliação de recebíveis, comunicando-se com o SAP Business One.

Outro ponto a se mencionar é a infraestrutura utilizada, optou-se pelo uso em nuvem através da solução Auto.Sky da Sky.One para que assim os custos de operação fossem reduzidos, o que significa que nem o franqueado ou a equipe de TI precisarão instalar o SAP Business One em suas máquinas para utilizar o sistema ERP, obtendo um ganho em performance sem precisar de computadores potentes para comportar todo o SAP.

.. image:: /_static/BR\ One\ Franquias/Cadastro/Detalhamento\ do\ ecossistema/Aspose.Words.33262046-518f-42ed-8965-0867230ceab3.001.png

**SAP Business One**

O SAP Business One na solução BrOne franquias utiliza os seguintes módulos para viabilizar as operações: Finanças, Compras, Vendas, Parceiro de negócios, Banco, Estoque, Produção, Recursos Humanos e Relatórios. A seguir serão descritos os detalhes das interações, além disso, a imagem a seguir representa de forma visual e resumida cada função exercida dentro dos módulos do sistema.

.. image:: /_static/BR\ One\ Franquias/Cadastro/Detalhamento\ do\ ecossistema/Aspose.Words.33262046-518f-42ed-8965-0867230ceab3.002.png

**Finanças**

Após as configurações feitas do franqueado no módulo de administração, temos o módulo de “Finanças” logo abaixo, no qual contém uma série de utilidades, dentre elas é utilizada a função de Plano de contas, que durante a implementação, é configurado uma única vez de acordo com as regulamentações financeiras do país e após determinado suas finanças e segmentos de conta será criado o Plano de Contas.

Também é utilizada a função de Lançamento contábil manual e Pré-lançamentos contábeis, que é idêntico à janela de Lançamento contábil manual, porém é um esboço que não cria valores no Razão.

Por fim, é utilizado a função de Lançamentos recorrentes (serve para criar um modelo para lançamentos periódicos e definir a respectiva frequência e data de vencimento) e Ativos fixos (`Clique aqui <fornece ambos os controles físico e financeiro sobre o ciclo de vida completo do ativo, da aquisição pela depreciação, reavaliação até a baixa ou venda).

**Vendas**

O módulo de Vendas possui um vasto conjunto de funcionalidades, no entanto, para a solução BrOne Franquias, a maioria delas não são necessárias, sendo utilizada somente as de Nota Fiscal de Saída, com suas particularidades devido às integrações com o add-on fiscal ao realizar apuração de impostos e declarações para Receita Federal. Além disso, o módulo possui uma tela do BrOne que conta com duas funcionalidades: log de erro de integração (`Clique aqui <usado para reprocessar notas fiscais de saída ou baixa no estoque que apresentaram erros>`_)e motor fiscal (`Clique aqui <simula a geração de impostos de venda ao consumidor final e envia esses dados para a mensageria da OOBJ).

**Compras**

O SAP Business One permite a administração de todo o processo de compra, desde as solicitações de compra até o processamento de notas fiscais de entrada, no entanto, para a atual necessidade apenas as funcionalidades de Recebimento de mercadorias (`Clique aqui <na qual o SAP atualiza as quantidades e contabiliza a entrada no estoque), Fatura de adiantamento de contas a pagar, Nota fiscal de entrada, Devolução de Nota fiscal de entrada e Transações recorrentes são utilizadas. 

Funcionam de forma diferente do que o padrão quando se usa somente o B1, ou seja, não existe a etapa do pedido de compra, com o uso do add-on fiscal através do serviço de distribuição de Documentos Fiscais Eletrônicos (`Clique aqui <DF-e>`_)o processo começa a partir da NF emitida de acordo com os CNPJ dos franqueados. É utilizado também o add-on bancário para pagamentos, usado somente no processo de compras.

**Parceiro de negócios**

É utilizado a função de Cadastro do parceiro de negócios. Majoritariamente, o Cadastro de parceiro de negócios é usado para Fornecedores, o motivo disso é porque o McDonalds tem apenas um cliente, no caso o Consumidor. Existem casos de cadastrarem parceiros como clientes, por exemplo: eles vendem para algum cliente o óleo usado nas lojas ou as caixas de papelões acumuladas. 

Vale destacar que as primeiras versões das integrações de cartões de contas a receber utilizavam as adquirentes como Parceiro de Negócios do tipo clientes, mas foram substituídas e passamos a utilizar somente contas contábeis.

**Banco**

O módulo “Banco” é o responsável por realizar todas as transações monetárias que envolvem contas bancárias, sendo elas a criação manual e automática de contas a receber e a pagar para vários meios de pagamento e performance manual e automática de reconciliações internas e externas. Para a solução BrOne Franquias são utilizadas as funções de Contas a receber, Contas a pagar, Depósitos e Boleto.

**Estoque**

O módulo de “Estoque” é utilizado para administrar todo o inventário da loja, sendo utilizadas as funções de Cadastro do item (`Clique aqui <o SAP Business One permite administrar todos os itens que a empresa compra, produz, vende ou mantém em estoque), Códigos de barras, Administração de itens e Transações de estoque (`Clique aqui <incluindo entrada e saída de mercadorias, transferências de estoque, transações de contagens de estoque etc.). 

Em sua base funciona de forma padrão no B1, as particularidades se devem às integrações com a mensageria fiscal (`Clique aqui <responsável por emitir as notas fiscais e realizar os ajustes no estoque>`_)e a função de contagem no aplicativo BrOne Franquias (`Clique aqui <gera documentação e reflete diretamente na contagem de estoque), que permitem respectivamente, a baixa imediata dos itens vendidos e manipulações das informações do estoque através do aplicativo que funciona no tablet. 

**Produção**

No módulo “Produção” é utilizada a função Estrutura de Produtos, na qual são cadastrados os itens de venda, contendo os códigos de itens Master que compõem este item, sendo a relação entre o PLU e os Masters. A estrutura de produtos é utilizada em qualquer processo de baixa de estoque (`Clique aqui <por exemplo, em caso de Vendas, Break ou Desperdícios).

**Recursos Humanos**

O módulo de “Recursos Humanos” insere e atualiza informações sobre os colaboradores da empresa ao utilizar a função Cadastro de Colaboradores, na qual o usuário do RH faz esse controle dos funcionários. Ele é a relação de vínculo com o cadastro de usuário do SAP, mesmo que sem licença dentro do sistema, para controle de autorizações, sendo também responsável pelos vínculos por filiais.<a name="_heading=h.ruyoaqxmwlmu"></a> Logo, seu uso, apesar de ter outras finalidades, está ligado unicamente em cadastrar colaboradores responsáveis pela abertura e fechamento de caixas dentro do aplicativo<a name="_heading=h.q5h8i8b9z3mk"></a><a name="_heading=h.1m06hlt8q9z4"></a>.

**Add-ons do SAP Business One**

Como dito anteriormente, o SAP Business One possui inúmeras funcionalidades, e muitas delas são utilizadas em conjunto com a solução BrOne Franquias, no entanto, as particularidades das rotinas operacionais, fiscais e contábeis necessitam funcionalidades complementares para operarem de acordo com o desejado, portanto como somente o sistema ERP não consegue dar todo o suporte, os add-ons são utilizados para suprir essa lacuna.


**T10 Extreme - Skill**

O T10 Extreme da Skill na solução BrOne Franquias é um Add-on** fiscal para o SAP B1, utilizado para a validação automática dos documentos fiscais e gestão de notas fiscais eletrônicas. São utilizadas as seguintes funções: Escrituração Contábil Fiscal, EFD Reinf, Importação de Arquivos Digitais, Administrador de Documentos e Cadastro de Códigos de Serviços. 

Para mais informações sobre este add-on, (`Clique aqui <https://gruposkill.com.br/skillconsulting/>`_)para acessar o manual oficial.

**Triple One - Skill**

O Triple One é um Add-on fiscal desenvolvido pela empresa Skill para o SAP B1 utilizado para a emissão de livros fiscais e obrigações (`Clique aqui <principais e acessórias).**  Estão disponíveis as seguintes funções: ECD - Contábil, EFD - Fiscal, EFD - Contribuições, FCI - Ficha Conteúdo Importação, FCONT - Controle Fiscal, NFe - Nota Fiscal Eletrônica Federal, MDF-e, GNRE, NFSe - Nota Fiscal de Serviços Eletrônica, NFCe - Nota fiscal do consumidor, PROFIS - Procedimentos Fiscais.

Para mais informações sobre este add-on, (`Clique aqui <https://gruposkill.com.br/skillconsulting/>`_)para acessar o manual oficial.

**Tax One – Invent**

**O Tax One é um add-on desenvolvido pela empresa Invent usado para obrigações fiscais, possui um conjunto de módulos que são:** TaxPlus (`Clique aqui <Emissão de livros fiscais e obrigações - principais e acessórias); TaxPlus DFe (`Clique aqui <Validação automática dos documentos fiscais); TaxPlus NFe (`Clique aqui <Gestão de notas fiscais eletrônicas automáticas e eficientes). 

Para mais informações sobre os  módulos deste add-on, (`Clique aqui <http://docs.inventsoftware.info/TaxOne/>`_)para acessar o manual oficial da TaxPlus, (`Clique aqui <http://docs.inventsoftware.info/TaxOne.Nfe.Importer/>`_)para acessar o manual oficial da TaxOne DF-e e (`Clique aqui <http://docs.inventsoftware.info/TaxOne.Nfe/>`_)para acessar o manual oficial da TaxOne NF-e.

**BankPlus - Invent**

O BankPlus é um add-on bancário também desenvolvido pela Invent que tem como objetivo automatizar os processos financeiros das empresas, de forma a reduzir o tempo das atividades diárias e repetitivas, reduzindo possibilidades de erros nos processos financeiros. Estão disponíveis as seguintes funções: Cobrança Bancária Eletrônica, Pagamento Eletrônico, Conciliação de Cartão e Conciliação Bancária, no entanto são utilizados pelas franquias McDonald’s apenas as funcionalidades de Pagamento Eletrônico e em alguns casos a Conciliação Bancária.

Para mais informações sobre este add-on, (`Clique aqui <http://docs.inventsoftware.info/IntBank/>`_)para acessar o manual oficial da BankPlus.

**Intercompany**

O Intercompany é um add-on do SAP que permite administrar transações de uma empresa para múltiplas empresas replicando automaticamente as transações correspondentes através de uma base de dados de múltiplas empresas. Ao automatizar esta replicação de transações, os esforços requeridos para gerar demonstrações financeiras de negociação entre empresas são reduzidos significativamente. 

As funcionalidades chaves da integração do Intercompany são: Replicação de dados master e compartilhamento de conteúdo, Suporte para processos padronizados e transparentes entre entidades de negócios, Visibilidade financeira e operacional entre entidades de negócios, Controle e colaboração entre entidades de negócios.

**Plataforma de Conciliação bancária**

**Card Services - Atos Capital:**

O Card Services da Atos Capital na solução BrOne Franquias é uma tecnologia financeira especializada na Gestão e Conciliação de Cartões Eletrônicos. Por meio dela o usuário poderá gerenciar todas as transações de cartões crédito/débito de diversas Adquirentes (`Clique aqui <operadoras>`_)simultaneamente, sejam elas via TEF, POS ou E-Commerce.

Além disso, o Card Services está integrado automaticamente às principais Adquirentes (operadoras), bandeiras de alimentação e benefícios, possibilitando assim uma gestão integrada de todo o ambiente de recebimento de cartões eletrônicos. Todas as transações são capturadas automaticamente, transação a transação, NSU a NSU ou Códigos de Autorização por Código de Autorização.

**APIs**

**API OOBJ – Mensageria Fiscal**

A OOBJ na solução BrOne Franquias é um sistema em nuvem de mensageria fiscal responsável pela comunicação com a Sefaz para emissão, recebimento, armazenamento e análise de documentos fiscais eletrônicos (realizando o processamento fiscal dos mais diversos tipos de documentos: NF-e, NFC-e, NFS-e, NF3e, CT-e e MDF-e).


(`Clique aqui <https://conteudo.oobj.com.br/solicitar-contato-decisao?ref=blogpost-mensageria-fiscal>`_) é quem valida as informações da empresa e do cliente e as manda para a Sefaz para poder autorizar a nota.



**API Arcos Dourados – Cadastros de Master, Ingredientes, PLUs, Receitas e Combos.**

Para que seja feita a gestão e padronização dos itens de venda de acordo com a matriz do McDonald’s no Brasil é utilizada uma API que se comunica entre a base de dados da Arcos Dourados e a base de dados do franqueado, essa API busca os códigos que devem ser integrados ao SAP para conferência, revisão e completo para cadastro nos padrões exigidos pelo SAP B1 e esta integração é feita manualmente no sistema. 

**API Arcos Dourados – Exportação de Dados de Vendas**

Conforme a necessidade de negócios da Arcos Dourados, é preciso exportar os dados de vendas da mensageria fiscal, portanto as vendas são agrupadas e enviadas via API Arcos Dourados para conferência e complemento dos dados de vendas pela franqueadora.

**API Arcos Dourados – Recebimento de Dados de Vendas**

A API de vendas dos franqueados da Arcos Dourados foi utilizada inicialmente para consumo das vendas, enquanto o projeto de mensageria com a OOBJ era desenvolvido. O consumo desta API foi descontinuado temporariamente, pois novas lojas e franqueados já são ativados com a mensageria Uppertools e OOBJ.

**Infraestrutura**

**Auto.Sky – Business One**

O Auto.Sky Business One na solução BrOne Franquias oferece acesso a uma infraestrutura de SAP em Nuvem para aliviar o gerenciamento de infraestruturas locais, ganhando performance e reduzindo custos. A disponibilidade via web faz com que os usuários possam acessar o sistema de onde estiverem e em qualquer máquina, independendo de configurações de hardware necessárias para comportar todo o SAP B1.