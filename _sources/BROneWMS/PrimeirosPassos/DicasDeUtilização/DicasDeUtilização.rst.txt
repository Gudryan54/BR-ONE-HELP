Dicas de utilização
^^^^^^^^^^^^^^^^^^^

Visando a praticidade e a versatilidade, neste tópico, serão demonstrados recursos disponíveis no BR One WMS que otimizam o uso da solução.

.. |image-link| image:: WMS-EscolhaDeArmazém.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../_images/WMS-EscolhaDeArmazém.png" style="width: 300px;" />
   </div>

| \

Realizando o login no aplicativo, todos os armazéns criados para a filial serão listados. O armazém no BR One WMS, representa o vínculo entre um espaço físico com uma impressora. Pensando no cenário em que o usuário irá realizar suas atividades de expedição, e nesse processo há a necessidade de impressão de etiquetas, de acordo com o armazém selecionado, as etiquetas serão impressas na impressora configurada.

| \

.. tip::

   Você pode saber mais sobre as configurações para impressão de etiquetas clicando **aqui**.

| \

.. |image-link2| image:: WMS-DefinirPerfilUsuário.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../_images/WMS-DefinirPerfilUsuário.gif" style="width: 300px;" />
   </div>

| \

Após a seleção do Armazém, serão listados para o usuário os módulos disponíveis no BR One WMS. É possível no canto inferior, definir um perfil para o usuário logado, ativando a flag e clicando no módulo pré-selecionado, será aberta a lista para a seleção dos módulos. Uma vez definido o perfil para o usuário, no próximo login, acessará automaticamente o módulo definido.


| \

.. |image-link3| image:: WMS-SolicitaçãodeReconexão.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../_images/WMS-SolicitaçãodeReconexão.png" style="width: 300px;" />
   </div>

| \

O BR One WMS se comunica com o SAP Business One através da Service Layer, que por sua vez, possui um tempo máximo de conexão, que pode variar de acordo com a configuração. 

| \

.. |image-link4| image:: WMS-SessionTimeout.png
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../_images/WMS-SessionTimeout.png" style="width: 500px;" />
   </div>
   
| \

.. important::

   A partir da versão 39, o tempo de conexão não é definido mais no appsetings e passa a seguir o tempo da **SL - 1 minuto**, ou seja, se na SL estiver definido 30 minutos, quando atingir 29 minutos de conexão,  o aplicativo solicitará a reconexão do usuário.

   * Para alterar o tempo de conexão na SL, basta alterar o valor do campo **Session Timeout**.
   
| \

Para evitar a perda da conexão com a Service Layer durante os processos, e consequemente, perder as atividades realizadas no aplicativo, é possível configurar na propria SL (Service Layer) um timer, para que o usuário refaça a conexão e continue realizando as suas atividades, garantindo que nada seja perdido.

| \

.. |image-link5| image:: WMS-NavegandopelaNumeração.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../_images/WMS-NavegandopelaNumeração.gif" style="width: 300px;" />
   </div>

| \

Todos os módulos e menus possuem uma numeração, que pode ser usada como atalho, através do teclado numérico do dispositivo.

| \

.. |image-link6| image:: WMS-CampoLeituraCódigodeBarras.gif
   :width: 300px
   :align: middle

.. raw:: html

   <div style="text-align: center;">
     <img src="../../../_images/WMS-CampoLeituraCódigodeBarras.gif" style="width: 300px;" />
   </div>

| \

Em diversas telas do aplicativo, será possível realizar leituras via código de barras, em campos que possuírem a identificação de código de barras, conforme visualizado a cima.