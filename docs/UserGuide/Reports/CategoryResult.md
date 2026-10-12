# Resultado por categoria

O relatório **Resultado por categoria** responde: “o que eu ganhei e o que eu consumi neste período?”. Ele junta receitas e despesas pela **data do lançamento** e mostra a fatia de cada categoria.

No menu o nome é **Resultado por categoria**. A tela se chama **Receitas e Despesas**.

O resumo do mês no [painel inicial](../MainDashboard.md) usa a mesma conta. Os outros relatórios estão em [Relatórios](Reports.md). A visão geral do app está em [WFinance](../WFinance.md).

---

## Neste guia

- [A tela](CategoryResultScreen.md) — período, filtros, subcategorias, moeda e a lista de lançamentos.

---

## Como chegar

| Caminho | O que abre |
|---------|------------|
| Atalho **Relatório de resultado**, na Central | A tela, no mês atual. |
| Central → **Relatórios** → Análises → **Resultado por categoria** | A mesma tela. |
| [Painel](../MainDashboard.md#resumo-financeiro), visão **Resultado**, toque nos valores | A mesma tela, já com o interruptor de previstas do painel. |

---

## O que é análise por resultado

O resultado registra o valor no período em que ele foi gerado. A data do pagamento pode ser outra.

Na prática:

- Uma despesa entra no mês da compra ou da contratação.
- Uma receita entra no mês em que foi gerada.
- O saldo do período diz se você gerou mais do que consumiu. No painel, saldo positivo aparece como **Lucro** e saldo negativo como **Prejuízo**.

Compra no cartão em 25/03 compõe as despesas de março. O pagamento da fatura em 10/04 é uma [transferência](../Transactions/TransactionTypes.md#transferência): o dinheiro sai da conta e quita o cartão. Esse pagamento não cria outra despesa e não muda março neste relatório.

Entram receitas e despesas **com categoria**. O filtro de previstas começa ligado, então um salário ainda previsto entra no mês da data dele. Transferência fica de fora, porque não tem categoria. Lançamento sem categoria também fica de fora.

O dia em que o dinheiro entrou ou saiu da conta é a pergunta do fluxo de caixa. Este relatório serve para ver o padrão de consumo e de renda ao longo do tempo.

O mesmo texto está no app, no link **Como funciona o relatório de resultado?**, quando a ajuda contextual está ligada. No painel, o link equivalente é **O que é Resultado?**.

---

## Outubro de 2026

A captura está em reais, no mês de outubro.

![Resultado de outubro de 2026: salário de R$ 7.500, despesas de R$ 4.200 e saldo de R$ 3.300](Relatorio%20-%20Resultado%20por%20categorias.png)

### Os três números do topo

| | Valor | Em palavras |
|--|-------|-------------|
| **Receitas** | R$ 7.500,00 | O que o mês gerou. |
| **Despesas** | R$ 4.200,00 | O que o mês consumiu. Na tela o valor aparece negativo. |
| **Saldo** | R$ 3.300,00 | 7.500 − 4.200. O mês gerou mais do que consumiu. No painel, isso é lucro. |

Esses R$ 3.300 medem o mês pela data do lançamento. Uma compra de outubro no cartão já está nas despesas, mesmo que a fatura seja paga em novembro. O saldo da conta bancária pode contar outra história.

### Para onde foi cada parte

A barra é a fatia da categoria **dentro do seu tipo**. Receita compara com o total de receitas. Despesa compara com o total de despesas.

| Categoria | Valor | Fatia | Leitura |
|-----------|-------|-------|---------|
| **Salário** | R$ 7.500,00 | 100,0% | Única receita do mês. |
| **Moradia** | R$ 3.650,00 | 86,9% | 3.650 ÷ 4.200. Quase todo o consumo. |
| **Saúde** | R$ 250,00 | 6,0% | 250 ÷ 4.200. |
| **Trabalho** | R$ 200,00 | 4,8% | 200 ÷ 4.200. |
| **Assinaturas e serviços** | R$ 100,00 | 2,4% | 100 ÷ 4.200. |

Moradia está aberta: Aluguel/Condomínio R$ 3.500,00 e Acessórios R$ 150,00. As duas somam os R$ 3.650,00 da categoria. As outras despesas continuam fechadas; o chevron de cada uma abre o detalhe.

A lista vai da maior para a menor. Moradia vem primeiro porque é a maior despesa. Salário vem sozinho nas receitas.

Saúde em R$ 250,00 já é o líquido. No guia de [estorno](../Transactions/Reversal.md), a consulta de R$ 400 e o reembolso de R$ 150 ficam os dois em Saúde, e o relatório mostra a diferença.

### O que este mês diz

A renda do mês é um salário. O consumo está concentrado em moradia. Saúde, trabalho e assinaturas são o restante. O mês gerou R$ 3.300,00 a mais do que consumiu.

Para ver se esse dinheiro já está na conta, ou se ainda vai sair no pagamento da fatura, use o [fluxo de caixa](CashFlow.md).

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
