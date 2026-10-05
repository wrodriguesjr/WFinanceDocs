# Status

O status diz se o valor já vale para o saldo real.

Os outros guias estão em [Transações](Transactions.md). Trocar o status se faz na [lista](TransactionLists.md), deslizando o lançamento. O formulário não muda o status.

---

## Previsto, efetivado e reconciliado

| Status | O que significa | Entra no saldo? |
|--------|-----------------|-----------------|
| **Previsto** | Ainda vai acontecer, ou você está só planejando. | Não. Aparece só no saldo previsto. |
| **Efetivado** | Já aconteceu. | Sim. |
| **Reconciliado** | Conferido com extrato bancário ou fatura importada. É o maior nível de confiança. | Sim. |

Regras práticas:

- Lançamentos **avulsos** costumam nascer **efetivados**.
- **Parcelas e recorrências** nascem **previstas**. Você confirma quando o dinheiro de fato sai ou entra. O detalhe da série está em [Parcelas e recorrência](InstallmentsAndRecurrence.md).
- **Compras no cartão** já nascem **efetivadas**. Fatura não tem “previsto”.
- Na **carteira** (dinheiro vivo), o ciclo é previsto ↔ efetivado. Reconciliado não se usa.
- Os dois lados de uma transferência **sempre** têm o mesmo status.

Só o que está **efetivado** ou **reconciliado** muda o saldo da conta, os totais da barra inferior e o progresso das [metas](../Goals/Goals.md).

---

## O que entra no saldo

- **Saldo real** = efetivados + reconciliados.
- **Saldo previsto** = real + o que ainda está previsto.
- **Metas** = só efetivados e reconciliados.
- **Estorno** continua sendo receita, despesa ou transferência. Só o [sinal](Reversal.md) inverte. O valor efetivado entra no saldo no sentido do sinal.
- **Saldo do período**, na visão geral, soma entradas e saídas da lista, sem puxar meses anteriores.
- **Saldo inicial e final** de uma conta bancária ou carteira consideram o que veio do mês passado.

Na visão geral, transferências aparecem nos dois lados (saiu daqui, entrou ali). No extrato de uma conta, você vê só a perna daquela conta.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
