# A tela de extratos bancários

A tela abre no **acumulado do ano**, de janeiro até o mês atual, na moeda padrão do seu perfil. O título é **Extratos bancários**.

O que o relatório mede está em [Extratos bancários](BankStatements.md). O extrato de um dia está em [As listas](../Transactions/TransactionLists.md#extrato-bancário).

---

## Período

As setas trocam o intervalo. O toque no título abre o tipo de período.

| Tipo | O que mostra |
|------|----------------|
| **Mensal** | O mês na tela. |
| **Trimestral** | Os três meses do trimestre. |
| **Anual** | Janeiro a dezembro daquele ano. |
| **3 Meses**, **6 Meses**, **12 Meses** | A janela que termina no mês na tela. A [captura](BankStatements.md#de-março-a-agosto-de-2026) está em 6 meses, de março a agosto. |
| **Acumulado no ano** | De janeiro até o mês na tela. É o padrão ao abrir. |

---

## Contas

Os chips são as contas bancárias. Nenhum marcado significa todas as contas ativas.

**Exibir contas inativas** começa desligado. Ligado, a conta arquivada entra nos chips e na soma, se estiver no recorte.

Carteira, cartão e investimento ficam de fora desta tela.

---

## O que entra

Só movimento de **conta bancária**, já [efetivado ou reconciliado](../Transactions/TransactionStatus.md). Previsto fica de fora. Não há interruptor para incluí-lo.

- **Receita** na conta: entrada. O saldo de fim de mês sobe.
- **Despesa** na conta: saída.
- **Transferência** para outra conta bancária: saída nesta conta e entrada na outra, se as duas estiverem no relatório. O saldo líquido do período se anula nesse valor. As barras continuam mostrando os dois lados.
- **Pagamento de fatura**, **saque** e **aplicação**: saída, no dia em que o dinheiro sai da conta.
- **Depósito** e **resgate** que voltam para a conta: entrada.

O saldo de cada conta no fim do mês já inclui o saldo inicial e tudo o que ficou dos meses anteriores. O saldo inicial em si não entra na coluna de entradas do período.

---

## O gráfico e o resumo

Cada mês tem duas barras: **Entradas** (verde) e **Saídas** (vermelho). As duas crescem para cima, no tamanho do valor. A linha clara, **Saldo**, é a soma dos saldos de fim de mês.

No resumo:

- **Total de entradas** e **Total de saídas** somam os meses que tiveram movimento.
- **Saldo líquido** é entradas mais saídas. Saída já entra com sinal negativo.
- **Média mensal** divide esses totais pela quantidade de meses com movimento. Mês zerado fica de fora da média e continua no gráfico.

---

## Dois modos de lista

Os chips ficam abaixo do resumo. O padrão é **Meses / Contas**.

| Modo | O que você vê |
|------|----------------|
| **Meses / Contas** | Cada mês, e dentro dele as contas. Entradas, saídas e saldo estão na moeda do seu perfil. |
| **Contas / Meses** | Cada conta, e dentro dela os meses. Os valores ficam na **moeda da conta**. O saldo ao lado do nome é o saldo do **último mês** do período, na moeda dela. |

Toque na conta (no modo Meses / Contas) ou no mês (no modo Contas / Meses) para abrir o [extrato daquela conta](../Transactions/TransactionLists.md#extrato-bancário), já naquele mês. O cabeçalho do mês, sozinho, não abre lista.

Sem conta no recorte, a tela avisa: “Nenhum dado encontrado para o período selecionado”.

---

## Moeda

Os totais, o gráfico e a lista **Meses / Contas** usam a moeda padrão do seu perfil. A taxa é a do **último dia daquele mês**.

Se faltar taxa para algum saldo, a tela não calcula. O aviso lista os pares e a data de cada um, e o gráfico some até a taxa existir. Cadastre a taxa em Central → Estrutura financeira → **Taxas de câmbio**. Mais em [Quando falta uma taxa](../Transactions/CurrencyConversion.md#quando-falta-uma-taxa).

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| Entradas menos saídas não fecham com o saldo do mês | O saldo é o de fim de mês. Ele carrega o que já havia. Na captura, Conjunta movimentou R$ 1.050,00 em março e fechou em R$ 700,00. |
| Transferi da conta A para a B e as duas barras cresceram | Cada conta registra o seu lado. O saldo líquido do período cancela esse valor. |
| A compra do cartão não aparece | Ela fica na [fatura](CardInvoices.md). Aqui entra o pagamento, como saída da conta. |
| Um previsto não mudou o saldo | Este relatório usa só efetivado e reconciliado. |
| Uma conta sumiu | Ela está inativa e **Exibir contas inativas** está desligado, ou o chip dela está de fora quando há outras marcadas. |
| A média parece baixa | Mês sem entrada e sem saída fica de fora da divisão. |
| A tela só mostra o aviso de câmbio | Falta taxa no fim de algum mês. O relatório não mostra número parcial. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
