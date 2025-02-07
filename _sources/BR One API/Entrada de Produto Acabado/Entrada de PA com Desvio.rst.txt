Entrada de PA com desvio na OP de Retrabalho
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O parâmetro **% desvio da quantidade planejada da OP de retrabalho** quando marcado possibilita configurar uma porcentagem de desvio para a entrada de PA nas OPs de Retrabalho. Onde ao realizar a entrada de PA pela API com a configuração do desvio ativa, foi necessário realizar alguns ajustes nos campos do JSON da entrada.

.. image:: /_static/BR\ One\ API/EntradaPAcomDesvio/01.png
   :scale: 100%
   :align: center

| \

- **OP de Retrabalho com desvio configurado, PA administrado por lote, sem troca de lote:**

Onde para uma entrada que possua quantidade planejada e quantidade sobressalente (desvio configurado), os arrays “lotes” e “lotesTransferenciaEstoque” possuem respectivamente a seguinte função:

- **Array “lotes”:**

Indica o número de lote das quantidades sobressalentes, que no add-on é adicionado através de uma entrada de mercadoria e consequentemente o número de lote será utilizado na transferência de estoque gerada no processo.

- **Array “lotesTransferenciaEstoque”:**

Indica o número de lote que será utilizado na transferência de estoque para os itens referentes a quantidade planejada da OP, ou seja, deve ser utilizado o número de lote informado na liberação da OP de Retrabalho.

Segue abaixo um exemplo de JSON, que deve ser enviado para realizar a entrada de PA da OP de Retrabalho (Exemplo de OP com 10 peças planejadas e desvio de 100%):

**Entrada de PA de apenas quantidades planejadas:**

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 5,
      "trocaLoteEntradaRetrabalho": false,
      "lotesTransferenciaEstoque": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ]
   }


**Entrada de PA de quantidades planejadas e sobressalentes:**

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 10,
      "trocaLoteEntradaRetrabalho": false,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ]
   }


**Entrada de PA de apenas quantidades sobressalentes:**

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 5,
      "trocaLoteEntradaRetrabalho": false,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ]
   }


Importante observar que para esse caso as quantidades dos arrays, são somados e devem ser igual a quantidade informada no campo “quantidade”.

- **OP de Retrabalho com desvio configurado, PA administrado por lote, com troca de lote:**

Onde para uma entrada que possua quantidade planejada e quantidade sobressalente (desvio configurado), os arrays “lotes” e “lotesTransferenciaEstoque” possuem respectivamente a seguinte função:
 
- **Array “lotes”:**

Indica o número de lote das quantidades que serão utilizados na saída de insumos para a realização da troca de lote.

- **Array “lotesTransferenciaEstoque”:**

Indica o número de lote da entrada de mercadoria e o número de lote que será utilizado na transferência de estoque.

Segue abaixo um exemplo de JSON, que deve ser enviado para realizar a entrada de PA da OP de Retrabalho (Exemplo de OP com 10 peças planejadas e desvio de 100%):

**Entrada de PA de apenas quantidades planejadas:**

.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 5,
      "trocaLoteEntradaRetrabalho": true,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L02",
            "quantidade": 5
         }
      ]
   }

**Entrada de PA de quantidades planejadas e sobressalentes:**


.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 10,
      "trocaLoteEntradaRetrabalho": true,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ],
      "lotesTransferenciaEstoque": [
         {
            "lote": "L02",
            "quantidade": 10
         }
      ]
   }

**Entrada de PA de apenas quantidades sobressalentes:**


.. code-block:: json

   {
      "docNumOrdemProducao": 0,
      "dataDocumento": "2024-11-01",
      "codigoDeposito": "",
      "quantidade": 5,
      "trocaLoteEntradaRetrabalho": true,
      "lotes": [
         {
            "lote": "L01",
            "quantidade": 5
         }
      ]
   }
