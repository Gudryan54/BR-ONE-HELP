
Validações obrigatórias do add-on
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Existem algumas validações de consistência de dados que são obrigatórias estarem devidamente configuradas na base de dados para assegurar o funcionamento pleno do BR One, de acordo com os modulos habilitados.

Exemplo de validação do Script chamado P_Br1_Valida-BROne.

.. image:: /_static/Geral/Validações\ obrigatórias/Aspose.Words.54053868-55dc-4e92-b6b4-1f273be0f376.004.png

**Falta chamada na Transaction Notification**

Todos as “Valida”, por exemplo, P\_Br1\_Valida-BrOne, devem ter suas chamadas realizadas na procedure do SAP “SBO\_SP\_TransactionNotification”, caso alguma das suas validas não tenham suas chamadas realizadas, a seguinte mensagem será exibida:

.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.031.png

Para solucionar este erro basta seguir os seguintes passos:

 Acessar na base de dados da “Company” específica a procedure “SBO\_SP\_TransactionNotification”, na opção de “Modificar”.

.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.032.png

No trecho específico para inclusão de novos códigos, colocar a chamada da procedure específica:


.. image:: /_static/Geral/Script/Aspose.Words.7110e183-625e-42a0-b23f-3fb4c7e031ef.033.png