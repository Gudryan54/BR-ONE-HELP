Configuração de Vínculo de depósitos e utilizações por filial
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para bases multifilias, o depósito não será definido na tela **"Utilização"**, e sim na tela **"Vínculo de depósitos e utilizações por filial"**.

Para acessar a tela é necessário ir no menu:

**Administração > Definição > Estoque > Vínculo de depósitos e utilizações por filial.**

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.002.png


Nessa tela é possível cadastrar cada filial vinculando a utilização com o depósito. A filial é selecionada no campo **"Filial"** e os vínculos ocorrem nas linhas das colunas **"Utilização"** e **"Depósito"**.

No campo **"Utilização"**, aparecerão apenas as utilizações cadastradas na **tela "Utilização – Definição".**

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.003.png


No campo **"Depósito"**, serão filtrados apenas os depósitos da filial selecionada no campo **"Filial"**, independentemente do tipo.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.004.png


Após selecionar a utilização e o depósito que deseja realizar o vínculo, basta atualizar a tela **"Vínculo de depósitos e utilizações por filial"**, desta forma o vínculo para a Filial escolhida estará feito.

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.005.png


Se no campo **"Filial"** for escolhida uma filial que já possua cadastro, a seguinte mensagem de erro será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.006.png


*BR One :: Filial já existente.*

Para utilizações que tenham a flag **"Transf. Estoque"** marcada, só será possível selecionar um depósito que seja de **Envio Direto**.

Caso seja selecionado depósito que não seja de envio direto para uma utilização que tenha a flag **"Transf. Estoque"** marcada, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.007.png


*BR One :: Utilização de transferência de estoque deve ter depósito de envio direto. Linha: x*

Se o usuário tentar inserir a mesma utilização para a mesma filial, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.008.png


*BR One :: Não pode existir duas utilizações iguais para a mesma filial.*

Se o usuário tentar inserir um cadastro sem ter inserido uma utilização ou tentar escolher um depósito sem utilização, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.009.png


*BR One :: Selecione uma utilização.*

Se o usuário tentar inserir um cadastro com uma utilização sem depósito, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.010.png


*BR One :: Selecione um depósito. Linha: x*

Apenas será possível definir um depósito para uma utilização na tela **"Utilização - Configuração"** se a base não for Multi-filial. Se o usuário tentar definir um depósito para a utilização em uma base Multi-filial, a seguinte mensagem será exibida:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.011.png


*BR One :: Para bases multi-filial os depósitos devem ser configurados na tela de “Vínculo de depósitos e utilizações por filial”.*

Caso uma utilização cadastrada na tela **"Vínculo de depósitos e utilizações por filial"** não tenha a flag **"Transf. estoque"** marcada e seu depósito não seja de envio direto e o usuário queira checar esse flag na tela **"Utilização - Configuração"** para essa utilização, não será permitido e será exibida uma mensagem de erro:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.012.png


.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.013.png


*BR One :: A utilização "x" não pode ser marcada como transferência de estoque, pois no vínculo de utilização com filiais, a filial "x" possui esta utilização vinculada com um depósito que não é de envio direto.*

Após inserir a utilização e configurá-la nas "Configurações do beneficiamento", os flags não poderão mais ser desmarcados. Se o usuário tentar desmarcar a flag PN gratuito ou Transf. estoque, as seguintes mensagens de erro serão exibidas:

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.014.png


*BR One :: Utilização "x" está configurada para o processo de beneficiamento de compra de serviço e deve estar com o flag "PN gratuito" marcado.*

.. image:: /_static/BR\ One\ Produção/Cadastros/Configurações\ de\ Multifiliais/Configuração\ de\ Vínculo\ de\ depósitos\ e\ utilizações\ por\ filial/Aspose.Words.d4e83007-4ec4-487a-b40e-e65a02467cb9.015.png


*BR One :: Utilização "x" está configurada para o processo de beneficiamento de compra de serviço e deve estar com o flag transferência de estoque marcado.*
