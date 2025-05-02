## Atividade: Sistema de Folha de Pagamento

### Contexto

Você faz parte de um time de desenvolvimento de software responsável por criar um sistema para calcular os descontos e acréscimos na folha de pagamento dos funcionários de uma empresa. Seu objetivo é criar um programa em Python que solicite a matrícula e senha de um funcionário para ter acesso aos seus dados e calcular os descontos e acréscimos mais comuns no Brasil.

---

## Regras de Descontos e Acréscimos

### INSS (Instituto Nacional do Seguro Social)

O desconto do INSS é calculado de acordo com a faixa salarial do funcionário:

| Faixa Salarial (R$)                   | Alíquota | Parcela a Deduzir (R$) |
|--------------------------------------|----------|-------------------------|
| Até R$ 1.518,00                       | 7,5%     | —                       |
| De R$ 1.518,01 até R$ 2.793,88        | 9%       | 113,85                  |
| De R$ 2.793,89 até R$ 4.190,83        | 12%      | 189,54                  |
| De R$ 4.190,84 até R$ 8.157,41        | 14%      | 318,38                  |


O teto de contribuição (faixa máxima) é R$ 8.157,41, o que gera um desconto máximo de **R$ 1.142,04** (14% de R$ 8.157,41).

---

### IRRF (Imposto de Renda Retido na Fonte)

O desconto do IRRF é calculado de acordo com a faixa salarial do funcionário e com a quantidade de dependentes:

| Base de Cálculo (R$)              | Alíquota (%) | Parcela a Deduzir (R$) |
|----------------------------------|--------------|-------------------------|
| Até 2.259,20                     | Isento       | —                       |
| De 2.259,21 até 2.826,65         | 7,5%         | 169,44                  |
| De 2.826,66 até 3.751,05         | 15%          | 381,44                  |
| De 3.751,06 até 4.664,68         | 22,5%        | 662,77                  |
| Acima de 4.664,68                | 27,5%        | 896,00                  |


Dedução por dependente: R$ 189,59 por dependente.

---

### Vale Transporte

Desconto de 6% do salário base do funcionário, caso opte pelo benefício.

---

### Vale Refeição

Desconto de 20% do valor do benefício fornecido pela empresa.

---

### Plano de Saúde

Desconto fixo de R$ 150,00 por dependente — aplicado somente ao dependente, não incide sobre o salário do funcionário.

---

## Instruções

1.  Solicite a matrícula e senha do funcionário para ter acesso aos seus dados.
2.  Solicite o salário base do funcionário.
3.  Pergunte se o funcionário deseja receber vale transporte (s/n).
4.  Pergunte o valor do vale refeição fornecido pela empresa.
4.  Pergunte ao usuário a quantidade de dependentes.
5.  Calcule os descontos e acréscimos na folha de pagamento do funcionário.
6.  Mostre o salário líquido do funcionário após os descontos e acréscimos.

---

## Observações

* Considere que o funcionário possui apenas um dependente.
* Considere que o salário base é o salário antes de quaisquer descontos ou acréscimos.
* Considere que o salário base, o vale refeição e o plano de saúde são informados em reais (R$).

---

## Exemplos de Cálculo

| Exemplo | Salário Base | Dependentes | Vale Transporte | Vale Refeição | Salário Líquido |
|---------|--------------|-------------|------------------|----------------|------------------|
| 1       | R$ 1.518,00  | 0           | Sim              | R$ 500,00      | R$ 1.190,30      |
| 2       | R$ 10.000,00 | 2           | Não              | R$ 800,00      | R$ 6.118,13      |**


Bom desenvolvimento!

