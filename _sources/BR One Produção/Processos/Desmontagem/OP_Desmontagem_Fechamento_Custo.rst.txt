Fechamento de custo contábil
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para OPs de desmontagem o fechamento de custo é realizado da seguinte forma:

- Rateio por quantidade
- Horas apontadas
- Horas previstas

Com base sempre no PA desmontado.

O LCM do arbitrado se mantém da mesma forma da OP padrão gerando:

- **Débito:** Conta GGF Arbitrado (Parametrizada nas configurações de Produção, aba Geral);
- **Crédito:** Conta de Alocação Temporária de custos (Parametrizada nas configurações de Produção, aba Geral).

O LCM do cadastro do GGF é feito com base no rateio da mesma forma da OP padrão gerando:

- **Débito:** Conta de Alocação Temporária de custos (Parametrizada nas configurações de Produção, aba Geral);
- **Crédito**: Conta do cadastro do GGF.

Após isso é realizada a validação do que foi arbitrado na OP de desmontagem com que foi rateado no fechamento de custo. Caso o valor do arbitrado foi menor que o do rateio deverá fazer:

- **Débito:** Conta de desmontagem (Configurações de produção na aba OP);
- **Crédito:** Conta de Alocação Temporária de custos (Parametrizada nas configurações de Produção, aba Geral).

Caso o valor do arbitrado foi maior que o do rateio deverá fazer:

- **Débito:** Conta de Alocação Temporária de custos (Parametrizada nas configurações de Produção, aba Geral);
- **Crédito:** Conta de desmontagem (Configurações de produção na aba OP).

Caso o valor do arbitrado foi o mesmo do rateio deverá:

Nesse cenário foi arbitrado um valor exatamente igual ao que foi realizado (Fechamento de Custo), então nesse caso o BR One não irá realizar nenhum lançamento de reavaliação de estoque e nenhum LCM para essa Ordem de Produção.

Caso não tenha arbitrado deve fazer o lançamento do LCM do cadastro do GGF é feito com base no rateio da mesma forma da OP padrão gerando:

- **Débito:** Conta de Alocação Temporária de custos (Parametrizada nas configurações de Produção, aba Geral);
- **Crédito:** Conta do cadastro do GGF.

E um LCM realizando o valor para desmontagem:

- **Débito:** Conta de desmontagem (Configurações de produção na aba OP);
- **Crédito:** Conta de Alocação Temporária de custos (Parametrizada nas configurações de Produção, aba Geral).