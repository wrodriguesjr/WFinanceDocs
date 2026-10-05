# Lançamentos que o app cria

Alguns itens não nascem do botão **+**. Eles existem para manter saldos e faturas coerentes.

Os outros guias estão em [Transações](Transactions.md). O que o formulário recusa gravar está em [Como lançar uma transação](ManageTransaction.md#se-o-app-recusar-gravar).

---

## Origem de cada lançamento

| Origem | Quando aparece | Pode editar? |
|--------|----------------|--------------|
| **Manual** | Você criou. | Sim. |
| **Notificação de app** | Você importou de uma [captura](../Capture/Capture.md). | Sim, em geral. |
| **Reconciliação / importação** | Veio de extrato ou fatura. | Com cuidado — já foi conferido. |
| **Saldo inicial** | Valor que a conta já tinha ao ser cadastrada. | Só em investimento. Nas outras contas, apague e faça um ajuste de saldo. |
| **Ajuste de saldo** | Correção pontual do saldo da conta. | Não. Apague e crie outro. |
| **Pagamento de cartão** | Você pagou a fatura. | Não edite. Se errou, exclua e pague de novo. |
| **Previsão de pagamento** | O app estima o pagamento futuro da fatura. | Não. Some sozinha quando o pagamento real é lançado. |
| **Saldo da fatura anterior** | O que não foi pago e passou para o ciclo seguinte. | Não. Some se a fatura anterior for paga no valor exato. |
| **Importação de fatura** | Compra vinda do arquivo do cartão. | Conforme as regras da fatura. |
| **Avaliação de saldo** | Você informou o valor atual do investimento. | Sempre efetivada; o status não muda. A folha está em [Atualizar o saldo](../Investments/UpdateBalance.md). |
| **Aporte direto** | Entrada no investimento sem passar por outra conta. | Sem cópia. |
| **Imposto** | Lançamento de imposto ligado ao investimento. | Sem cópia. |

Se o app recusar a edição, a mensagem indica o caminho: excluir e refazer, ou deixar o automático cuidar.

---

## Importação de extrato e fatura

Além das notificações, você pode importar:

- **extrato bancário** (arquivo OFX, por exemplo) para conferir a conta e marcar lançamentos como [reconciliados](TransactionStatus.md);
- **fatura do cartão**, para cruzar as compras com o arquivo oficial.

A reconciliação diz: “isto bate com o banco”. Lançamentos já reconciliados não devem ser importados de novo.

---

## Excluir

- Lançamento **único**: some só ele. Se for transferência, os dois lados saem juntos.
- **Série**: escolha se apaga só esta, as futuras ou todas. O alcance está em [Parcelas e recorrência](InstallmentsAndRecurrence.md).
- Tags daquele lançamento saem junto.
- Os saldos são recalculados na hora.
- Apagar um **pagamento de fatura** desfaz o pagamento na fatura.

Previsão de pagamento e saldo rolado da fatura anterior não podem ser apagados à mão.

No plano Free há limite de transações por espaço. O Premium remove esse teto — veja [Conta de usuário](../UserAccount.md).

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
