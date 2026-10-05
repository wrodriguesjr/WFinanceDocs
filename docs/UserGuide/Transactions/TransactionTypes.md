# Os três tipos

O app trata **três tipos**: receita, despesa e transferência. O tipo diz a natureza do lançamento. O [estorno](Reversal.md) inverte o sinal, sem trocar o tipo.

Os outros guias estão em [Transações](Transactions.md). O formulário está em [Como lançar uma transação](ManageTransaction.md).

---

## Receita

Dinheiro **entrando** na conta: salário, freelance, aluguel recebido.

- Exige **conta** e **categoria**.
- Pode ir para conta bancária, carteira ou cartão de crédito.
- Aceita **recorrência fixa** (salário, pensão) e **parcelamento**, quando fizer sentido.
- Na lista, entra nas **Entradas**.
- O sinal normal é **positivo (+)**.

Devolver parte de um valor que você tinha recebido é [estorno de receita](Reversal.md), não uma despesa nova.

---

## Despesa

Dinheiro **saindo** da conta: mercado, luz, assinatura, consulta médica.

- Exige **conta** e **categoria**.
- Pode sair de conta bancária, carteira ou cartão de crédito.
- Aceita **parcelamento** e **recorrência fixa** (aluguel, escola, streaming).
- Na lista, entra nas **Saídas**.
- O sinal normal é **negativo (−)**.

Reembolso do plano, devolução da loja e crédito na fatura são [estorno de despesa](Reversal.md). A categoria continua a mesma.

---

## Transferência

Dinheiro **saindo de uma conta e entrando em outra**, no mesmo espaço. Exemplos: PIX da corrente para a poupança, pagamento da fatura, aplicação em investimento, saque para a carteira.

- Exige **conta origem** e **conta destino**.
- Fica **sem categoria**. O dinheiro mudou de lugar. Não entra no “quanto gastei” como uma compra.
- Vira **dois lançamentos ligados**. Se você editar ou apagar um lado, o outro acompanha. Os dois compartilham o mesmo status.
- Aceita contas de moedas diferentes, com [conversão](CurrencyConversion.md).
- Cartão de crédito fica de fora. Compra e estorno de compra no cartão são despesa no próprio cartão.
- Conta de investimento só aparece aqui — é assim que se faz aplicação e resgate.

O sinal normal é **negativo (−)** na origem: saiu daqui, entrou ali. O sinal invertido desfaz a transferência.

---

## Em quais contas cada tipo vive

| Conta | Receita / despesa | Transferência | Como a lista se comporta |
|-------|-------------------|---------------|--------------------------|
| **Conta bancária** | Sim | Sim | Extrato do mês, com saldo de cada dia. |
| **Carteira** | Sim | Sim | Controle do dinheiro em espécie. |
| **Cartão de crédito** | Sim | Não | Fatura do ciclo, não o mês civil. |
| **Investimento** | Não | Só aplicação e resgate | Aportes, resgates e avaliações de saldo. |

O detalhe de cada lista está em [As listas](TransactionLists.md).

Uma transação também guarda:

- **descrição** (obrigatória);
- **categoria e subcategoria** (obrigatórias em receita e despesa);
- **observações** (opcional);
- **tags** (rótulos livres, como “viagem” ou “reforma”);
- **moeda e valor** — o valor original e, se for o caso, o valor já convertido para a moeda da conta.

---

## Aplicação e resgate

São transferências.

**Aplicação (aporte)** — conta bancária → investimento. Aumenta o valor investido.

**Resgate** — investimento → conta bancária. Leva uma parte do valor investido e uma parte do resultado, na proporção do saldo naquele momento. O detalhe está em [Como a rentabilidade é calculada](../Investments/Profitability.md).

A conta bancária precisa ser a **mesma associada** àquele investimento. Se a conta não bater, o app não conclui o lançamento.

Rendimento, perda e imposto ficam na [avaliação de saldo](../Investments/UpdateBalance.md) e em **Outros** no extrato do investimento, não como aplicação.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
