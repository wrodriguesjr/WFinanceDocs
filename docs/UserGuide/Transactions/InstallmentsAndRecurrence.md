# Parcelas e recorrência

Recorrência fixa e parcelamento são **mutuamente exclusivos**: no mesmo lançamento você escolhe um ou nenhum.

Os outros guias estão em [Transações](Transactions.md). Os campos do formulário estão em [Como lançar uma transação](ManageTransaction.md).

---

## Parcelamento

O valor total é dividido em N parcelas iguais. A primeira pode receber o ajuste dos centavos. Todas as parcelas são criadas de uma vez, com status **previsto**, cada uma na data certa.

No cartão, cada parcela cai na **fatura correspondente**.

Útil para compra em 10 vezes, inscrição anual dividida, financiamento.

Cada parcela pode ser ajustada depois, sozinha.

---

## Recorrência fixa

O mesmo valor se repete a cada período, até o limite da série. Também nasce **previsto**. Você efetiva cada ocorrência quando o dinheiro sai ou entra. O significado do status está em [Status](TransactionStatus.md).

Útil para salário, aluguel, escola, streaming, pensão.

Frequências: diária, semanal, bi-semanal, quinzenal, mensal, bimestral, trimestral, semestral, anual e bi-anual.

O app limita o tamanho da série para não criar lançamentos demais de uma vez. No diário, cerca de 1 ano. No mensal, alguns anos.

---

## Ao editar ou apagar uma série

Você escolhe o alcance:

| Opção | Efeito |
|-------|--------|
| **Só esta** | Altera ou apaga apenas o lançamento aberto. Os outros da série continuam. |
| **Esta e as futuras** | A partir desta data, inclusive. **Sobrescreve** ajustes que você tinha feito à mão nessas ocorrências. O passado fica como está. |
| **Toda a série** | Todas as ocorrências, inclusive as passadas. Também **sobrescreve** ajustes individuais. |

Uma ocorrência editada sozinha vira uma **exceção**: o restante da série não muda, até você escolher “futuras” ou “todas”.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
