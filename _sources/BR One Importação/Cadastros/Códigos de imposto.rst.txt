Códigos de imposto
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para acessar a tela de **Códigos de imposto**, é necessatio ir ao menu:

**Admininstração -> Definição -> Finanças -> Imposto -> Códigos de imposto**

Assim como na Combinação de impostos, o flag **Despesas adicionais** deve ser marcado para os impostos que participarão do processo que seleciona qual imposto será atribuído às colunas **Despesas adicionais código de imposto** na linha do item na NF de nacionalização (NF de entrada).

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.001.png

Os impostos utilizados nas telas **Configurações importação** ou **Config. impostos do processo de importação** não poderão ser inativados. Caso o usuário tente inativar um imposto em uso, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.002.jpeg

*(-12) BR One :: BR One :: Não é possível inativar o imposto, pois ele está sendo usado no processo de importação.*

****Exemplo de utilização do código de imposto para despesas adicionais:****

Ao gerar a NF Nacionalização, ele pega o imposto da linha e busca de acordo com as configurações outro imposto e coloca na coluna **Despesas adicionais código de imposto**. Ao ser gerada a NF de nacionalização nº 5, o imposto das colunas **Despesas adicionais código de imposto** será calculado de acordo com o imposto da coluna **Código de imposto**.

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.003.png

O add-on fará uma busca do imposto a ser atribuído de acordo com as seguintes configurações:

- Será verificado o imposto tipo ICMS 

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.004.png

- No imposto do tipo ICMS, será verificado quais os valores dos campos **Alíquota, Base de Cálculo, Base Isenta** e **Base Outras.**

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.005.png

- Após ter o valor dos quatro campos, será realizada uma busca de qual imposto a ser setado na coluna **Despesas adicionais código de imposto** atenda as seguintes condições:

- Ter o campo **Despesas adicionais** marcado;

- Ter um imposto do tipo **ICMS**;

- Os quatro campos do **ICMS** têm que ser **iguais** ao do **ICMS do imposto da linha**;

- Ter o campo **CFOP entrada** igual ao do imposto da linha;

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.006.png

- A combinação de impostos do código do imposto tem que estar com o flag **Desp. adic. Importação** marcado;

Após validar essas condições, será definido o imposto, que no exemplo, será o **3101-Dp2**.

.. image:: /_static/BR\ One\ Importação/Configurações/Códigos\ de\ imposto/Aspose.Words.1f87ae05-bb8f-4a68-a64e-c9d301a711cc.007.png


