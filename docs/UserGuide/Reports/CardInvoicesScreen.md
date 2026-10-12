# A tela de faturas de cartão

A tela abre no **ano atual**, de janeiro a dezembro, na moeda padrão do seu perfil. O título é **Faturas de cartão de crédito**.

O que o relatório mede está em [Faturas de cartão](CardInvoices.md). O ciclo de uma fatura está em [As listas](../Transactions/TransactionLists.md#fatura-do-cartão).

---

## Período

As setas trocam o intervalo. O toque no título abre o tipo de período.

| Tipo | O que mostra |
|------|----------------|
| **Mensal** | O mês na tela. |
| **Trimestral** | Os três meses do trimestre. |
| **Anual** | Janeiro a dezembro daquele ano. É o padrão ao abrir. |
| **3 Meses**, **6 Meses**, **12 Meses** | A janela que termina no mês na tela. |
| **Acumulado no ano** | De janeiro até o mês na tela. A [captura](CardInvoices.md#de-janeiro-a-outubro-de-2026) está nesse modo, de janeiro a outubro. |

O mês da lista é o mês da fatura. Uma compra feita no fim de março pode cair na fatura de abril, se o fechamento do cartão já tiver passado. O seletor está em [Fatura (só cartão)](../Transactions/ManageTransaction.md#fatura-só-cartão).

---

## Cartões

Os chips são os cartões. Nenhum marcado significa todos os cartões ativos.

**Exibir cartões inativos** começa desligado. Ligado, o cartão arquivado entra nos chips e na soma, se estiver no recorte.

---

## O gráfico e o resumo

Cada mês é uma barra empilhada, uma faixa por cartão. A ordem das faixas segue o total do cartão no período, do maior para o menor.

Com mais de seis cartões no recorte, o gráfico fica com os seis maiores e junta o restante numa faixa **Outros**. A lista, abaixo, continua cartão por cartão.

A linha **Total** aparece quando alguma fatura do período ficou com saldo a seu favor. Na captura de janeiro a outubro só há barras: as faturas são de gasto.

No resumo:

- **Total gasto** soma os meses que tiveram valor.
- **Maior mês** é o maior total entre os meses do período.
- **Menor mês** ignora o mês zerado. Na captura, janeiro é R$ 0,00 e o menor mês é março, R$ 230,00.
- **Média mensal** divide o total pela quantidade de meses com valor. Janeiro fica de fora: 5.110 ÷ 9 = 567,78.

---

## O status de cada fatura

O rótulo fica ao lado do valor.

| Status | O que significa |
|--------|-----------------|
| **Sem movimento** | Não há fatura, ou o total do ciclo é zero. |
| **Aberta** | O ciclo ainda está aberto. |
| **Futura** | O ciclo ainda não começou. |
| **Fechada** | Já fechou e aguarda o pagamento. |
| **Paga** | Já houve um pagamento. O valor ao lado continua sendo o total da fatura. |
| **Vencida** | Passou do vencimento sem pagamento. |

**Paga** em verde e **Vencida** em vermelho, como na captura: o Corporativo pago e a Mastercard família vencida.

---

## Dois modos de lista

Os chips ficam abaixo do resumo. O padrão é **Meses / Cartões**.

| Modo | O que você vê |
|------|----------------|
| **Meses / Cartões** | Cada mês, e dentro dele os cartões, com status e valor. |
| **Cartões / Meses** | Cada cartão, e dentro dele os meses. O valor ao lado do nome é a soma das faturas do cartão no período. |

Toque no cartão (no modo Meses / Cartões) ou no mês (no modo Cartões / Meses) para abrir a [fatura daquele cartão](../Transactions/TransactionLists.md#fatura-do-cartão), naquele mês. O cabeçalho do mês, sozinho, não abre lista.

Sem cartão no recorte, a tela avisa: “Nenhum dado encontrado para o período selecionado”.

---

## Moeda

Os totais e o gráfico usam a moeda padrão do seu perfil. A taxa é a do **vencimento** da fatura.

Se faltar taxa, o relatório continua aberto. A fatura sem taxa fica na lista, na moeda dela, com o aviso “sem taxa” ao lado do status, e sai das somas. O aviso no topo lista o par e a data. Cadastre a taxa em Central → Estrutura financeira → **Taxas de câmbio**. Mais em [Quando falta uma taxa](../Transactions/CurrencyConversion.md#quando-falta-uma-taxa).

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| A compra de março apareceu em abril | O mês é o da fatura, não o dia da compra. |
| Paguei e o valor continuou na linha | Esperado. A linha é o total da fatura. **Paga** só registra que houve pagamento. |
| Janeiro está em zero e o menor mês é outro | **Menor mês** e a média ignoram o mês zerado. |
| A média não fecha com o total dividido por todos os meses | O mês sem valor ficou de fora da divisão. |
| Um cartão sumiu do gráfico e virou Outros | Há mais de seis cartões. Os menores compartilham a faixa **Outros**. A lista ainda mostra cada um. |
| Um cartão sumiu da tela | Ele está inativo e **Exibir cartões inativos** está desligado, ou o chip dele está de fora quando há outros marcados. |
| O total está menor e há um aviso de câmbio | A fatura sem taxa ficou de fora da soma e continua na lista. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
