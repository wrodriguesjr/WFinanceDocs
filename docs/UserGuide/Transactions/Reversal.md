# Estorno

Um **estorno** é o mesmo tipo de lançamento com o **sinal invertido**. A consulta continua sendo despesa de Saúde. O que muda é o sentido do dinheiro: uma parte voltou.

Os outros guias estão em [Transações](Transactions.md). No formulário, o sinal fica nos botões **+** e **−** — veja [Como lançar uma transação](ManageTransaction.md#valor-sinal-e-moeda).

---

## Em uma frase

Reembolso, devolução e crédito na fatura **reduzem a despesa** (ou a receita) daquela categoria. Eles não criam um lançamento de natureza nova.

Essa separação entre tipo e sinal praticamente não existe nos outros apps de controle financeiro pessoal. Neles, o caminho disponível para um reembolso é lançar uma **receita**.

---

## O que distorce sem estorno

Sem estorno, o reembolso entra como dinheiro ganho no mês. A despesa original fica inteira. O resultado passa a mostrar duas coisas ao mesmo tempo: uma receita que não existiu e um gasto maior do que o que saiu do bolso.

Com estorno, a categoria guarda os dois lançamentos e o relatório mostra o gasto **líquido**. A [meta](../Goals/Goals.md) daquela categoria também desce, porque o atingido soma despesas e subtrai estornos de despesa.

O saldo da conta, esse sim, sobe: o dinheiro voltou. Subir o saldo e aumentar a receita do mês são contas diferentes.

---

## A consulta e o reembolso do plano

Na conta Conjunta, em outubro de 2026:

![Consulta de R$ 400 e reembolso de R$ 150, os dois em Saúde](Transacoes%20-%20Reembolso%20plano%20saude.png)

| Data | Lançamento | Categoria | Valor | Status |
|------|------------|-----------|-------|--------|
| 1º de outubro | Consulta médica | Saúde · Plano/Médicos | R$ 400, saindo | Efetivada |
| 5 de outubro | Reembolso do plano de saúde | Saúde · Plano/Médicos | R$ 150, voltando | Efetivada |

Os dois são **despesa**. O primeiro está no sinal normal (−). O segundo é estorno (+): na lista ele aparece em verde, sem o sinal de saída.

O saldo do dia vai de R$ 4.190 para R$ 4.340. Os R$ 150 entraram na conta.

No resultado, a receita do mês não cresce. Saúde fica com R$ 400 − R$ 150 = **R$ 250**. É o que a consulta custou de fato.

Se o reembolso tivesse sido lançado como receita, o mês mostraria R$ 400 de despesa em Saúde e R$ 150 de receita. O gasto da consulta continuaria parecendo R$ 400, e o mês ganharia uma entrada que não é salário, nem rendimento, nem qualquer outra receita.

---

## Os três sinais

| Tipo | Sinal normal | Estorno | Exemplo |
|------|--------------|---------|---------|
| **Despesa** | − dinheiro saindo | + reembolso, devolução, crédito | Consulta R$ 400 (−); plano devolve R$ 150 (+) |
| **Receita** | + dinheiro entrando | − devolução do que você tinha recebido | Cliente pagou R$ 1.000 (+); você devolve R$ 200 (−) |
| **Transferência** | − saiu da origem e entrou no destino | + desfaz o movimento | Poupança → corrente; depois você reverte |

Na lista, o estorno de despesa entra nas **Entradas** e o estorno de receita nas **Saídas**, porque a barra acompanha o sentido do dinheiro. O tipo gravado continua despesa ou receita. É esse tipo que os relatórios de categoria e as metas usam.

---

## Quando usar

Use estorno quando o dinheiro volta (ou sai) **por causa de um lançamento que já tinha natureza**:

- o plano reembolsa uma consulta;
- a loja devolve uma compra;
- a fatura recebe um crédito;
- você devolve parte de um valor que tinha recebido.

Mantenha o tipo original e inverta o sinal. No formulário de despesa, o normal é **−**; o estorno é **+**.

Transferir da poupança para a corrente não é estorno: o dinheiro só mudou de conta. Isso é [transferência](TransactionTypes.md#transferência).

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
