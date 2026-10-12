# Extratos bancários

O relatório **Extratos bancários** responde: “quanto entrou, quanto saiu e com quanto cada conta bancária fechou o mês?”. As barras são o movimento do mês. A linha é o **saldo no fim do mês**.

No menu o nome é **Extratos de conta bancária**. A tela se chama **Extratos bancários**.

Entram só contas bancárias, e só lançamentos [efetivados e reconciliados](../Transactions/TransactionStatus.md). O [fluxo de caixa](CashFlow.md) também olha o banco, com outra conta: lá uma transferência entre duas contas suas some do total. Aqui cada conta guarda o seu extrato. Os outros relatórios estão em [Relatórios](Reports.md).

---

## Neste guia

- [A tela](BankStatementsScreen.md) — período, contas, os dois modos de lista, o gráfico e a moeda.

---

## Como chegar

Central → **Relatórios** → Contas → **Extratos de conta bancária**.

A tela abre em **Acumulado no ano**, de janeiro até o mês atual.

---

## O que o saldo da linha representa

Cada ponto da linha é a soma dos saldos das contas **no fim daquele mês**. Esse saldo já traz o que havia no mês anterior.

O **saldo líquido** do resumo é outra conta: entradas do período mais saídas do período. Ele diz se entrou mais do que saiu. A linha diz quanto havia nas contas.

No app, o link **Como funciona o relatório de extratos bancários?** resume o gráfico, os dois modos de lista e a moeda, quando a ajuda contextual está ligada.

---

## De março a agosto de 2026

A captura usa o período **6 Meses**, terminando em agosto. Há três contas: Alimentação, Conjunta e Conta salário. As barras verdes são entradas, as vermelhas são saídas e a linha clara é o saldo de fim de mês.

![Extratos de março a agosto de 2026: entradas de R$ 77.950, saídas de R$ 72.570 e saldo líquido de R$ 5.380](Relatorio%20-%20Extrato%20bancario%20-%20grafico%20e%20resumo.png)

### O resumo do período

| | Valor | Em palavras |
|--|-------|-------------|
| **Total de entradas** | R$ 77.950,00 | O que entrou nas três contas nos seis meses. |
| **Total de saídas** | R$ -72.570,00 | O que saiu. Na tela o valor aparece em vermelho, com o sinal de menos. |
| **Saldo líquido** | R$ 5.380,00 | 77.950 − 72.570. Entrou mais do que saiu. |
| **Média mensal (entradas)** | R$ 12.991,67 | 77.950 ÷ 6. |
| **Média mensal (saídas)** | R$ -12.095,00 | 72.570 ÷ 6, com o sinal de saída. |

Os seis meses tiveram movimento, então a média usa os seis. Um mês sem entrada e sem saída continua no gráfico e fica de fora da média.

### Março, conta por conta

A lista abaixo do resumo está em **Meses / Contas**. O valor à direita do mês é o saldo das contas naquele fim de mês.

![Março a maio de 2026, com Alimentação, Conjunta e Conta salário](Relatorio%20-%20Extrato%20bancario%20-%20lista%20meses%20e%20contas.png)

| Conta | Entradas | Saídas | Saldo no fim |
|-------|----------|--------|--------------|
| **Alimentação** | R$ 500,00 | R$ -450,00 | R$ 50,00 |
| **Conjunta** | R$ 5.000,00 | R$ -3.950,00 | R$ 700,00 |
| **Conta salário** | R$ 7.000,00 | R$ -7.180,00 | R$ 120,00 |
| **Mar/2026** | | | **R$ 870,00** |

50 + 700 + 120 = 870. Esse R$ 870,00 é o primeiro ponto da linha.

Alimentação fecha a conta do mês: 500 − 450 = 50. Ela começou março zerada.

Conjunta movimentou 5.000 − 3.950 = 1.050, e fechou em 700. Fevereiro tinha deixado a conta em −350. −350 + 1.050 = 700.

Conta salário movimentou 7.000 − 7.180 = −180, e fechou em 120. Fevereiro tinha deixado 300. 300 − 180 = 120.

### Abril e maio

O saldo de abril nasce do saldo de março, mais as entradas, mais as saídas.

| | Alimentação | Conjunta | Conta salário | Saldo do mês |
|--|-------------|----------|---------------|--------------|
| **Abr/2026** | R$ 0,00 | R$ 1.750,00 | R$ -130,00 | **R$ 1.620,00** |
| **Mai/2026** | R$ 50,00 | R$ 2.800,00 | R$ 200,00 | **R$ 3.050,00** |

Alimentação em abril: 50 + 500 − 550 = 0. Conjunta: 700 + 5.000 − 3.950 = 1.750. Conta salário: 120 + 7.000 − 7.250 = −130. A soma é 1.620.

Em maio, Conta salário recebe 7.550 e sai 7.220. −130 + 7.550 − 7.220 = 200. O mês das três contas fecha em 3.050.

A linha acompanha esses fechamentos: 870 em março, 1.620 em abril, 3.050 em maio, e segue até agosto.

### O que estes seis meses dizem

As três contas receberam R$ 77.950,00 e pagaram R$ 72.570,00. O movimento do período ficou positivo em R$ 5.380,00. Esse número é a soma das entradas e das saídas. O dinheiro que já estava nas contas antes de março continua na linha do saldo, mês a mês.

Conta salário ficou negativa no fim de abril (R$ -130,00) e voltou ao positivo em maio (R$ 200,00).

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
