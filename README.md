## Atividade: Sistema de Folha de Pagamento

### Contexto

Você faz parte de um time de desenvolvimento de software responsável por criar um sistema para calcular os descontos e acréscimos na folha de pagamento dos funcionários de uma empresa. Seu objetivo é criar um programa em Python que solicite a matrícula e senha de um funcionário para ter acesso aos seus dados e calcular os descontos e acréscimos mais comuns no Brasil.

### Regras de Descontos e Acréscimos

#### INSS (Instituto Nacional do Seguro Social)

O desconto do INSS é calculado de acordo com a faixa salarial do funcionário:

* Salário até R$ 1.320,00: 7,5%
* Salário de R$ 1.320,01 até R$ 2.571,29: 9%
* Salário de R$ 2.571,30 até R$ 3.856,94: 12%
* Salário de R$ 3.856,95 até R$ 7.507,49: 14%

O valor máximo de desconto do INSS é de R$ 1.051,05.

#### IRRF (Imposto de Renda Retido na Fonte)

O desconto do IRRF é calculado de acordo com a faixa salarial do funcionário e com a quantidade de dependentes:

* Isento: Salário até R$ 2.112,00
* 7,5%: Salário de R$ 2.112,01 até R$ 2.826,65
* 15%: Salário de R$ 2.826,66 até R$ 3.544,00
* 22,5%: Salário de R$ 3.544,01 até R$ 4.256,00
* 27,5%: Salário acima de R$ 4.256,00

Dedução por dependente: R$ 189,59 por dependente.

#### Vale Transporte

Desconto de 6% do salário base do funcionário, caso opte pelo benefício.

#### Vale Refeição

Desconto de 20% do valor do benefício fornecido pela empresa.

#### Plano de Saúde

Desconto fixo de R$ 150,00 por dependente.

### Instruções

1.  Solicite a matrícula e senha do funcionário para ter acesso aos seus dados.
2.  Solicite o salário base do funcionário.
3.  Pergunte se o funcionário deseja receber vale transporte (s/n).
4.  Pergunte o valor do vale refeição fornecido pela empresa.
5.  Calcule os descontos e acréscimos na folha de pagamento do funcionário.
6.  Mostre o salário líquido do funcionário após os descontos e acréscimos.

### Observações

* Considere que o funcionário possui apenas um dependente.
* Considere que o salário base é o salário antes de quaisquer descontos ou acréscimos.
* Considere que o salário base, o vale refeição e o plano de saúde são informados em reais (R$).

### Exemplos de Cálculo

#### Exemplo 1: Salário Baixo (R$ 1.518,00) com 0 Dependentes e Vale Transporte

* Salário Base: R$ 1.518,00
* Dependentes: 0
* Vale Transporte: Sim
* Vale Refeição: R$ 500,00
**Salário Líquido: R$ 1190,30**

#### Exemplo 2: Salário Alto (R$ 10.000,00) com 2 Dependentes e Sem Vale Transporte

* Salário Base: R$ 10.000,00
* Dependentes: 2
* Vale Transporte: Não
* Vale Refeição: R$ 800,00
**Salário Líquido: R$ 6712,69**
