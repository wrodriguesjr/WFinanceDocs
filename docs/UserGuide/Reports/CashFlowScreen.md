---
description: Tela de fluxo de caixa do WFinance — quando o dinheiro entrou e saiu das contas bancárias.
---

# A tela de fluxo de caixa

A tela abre no **acumulado do ano**, de janeiro até o mês atual, na moeda padrão do seu perfil. O título é **Fluxo de Caixa**.

O que o relatório mede está em [Fluxo de caixa](CashFlow.md). O outro critério de data está em [Resultado por categoria](CategoryResult.md).

---

## Período

As setas trocam o intervalo. O toque no título abre o tipo de período.

| Tipo | O que soma |
|------|------------|
| **Mensal** | O mês na tela. É o recorte do card no painel. |
| **Trimestral** | Os três meses do trimestre. |
| **Anual** | Janeiro a dezembro daquele ano. |
| **3 Meses**, **6 Meses**, **12 Meses** | A janela que termina no mês na tela. A [captura](CashFlow.md#de-junho-a-agosto-de-2026) está em 3 meses, de junho a agosto. |
| **Acumulado no ano** | De janeiro até o mês na tela. É o padrão ao abrir. |

---

## Filtros

O bloco **Filtros** começa fechado.

| Filtro | O que faz |
|--------|-----------|
| **Contas bancárias** | Vazio significa todas. Com uma conta só, a transferência para outra conta passa a contar como entrada ou saída. |
| **Saldo acumulado** | Começa desligado. Ligado, cada mês ganha uma linha com a soma desde o início do período. O gráfico e o resumo do período continuam mês a mês. |
| **Incluir transações previstas** | Começa ligado. Desligado, ficam só lançamentos [efetivados e reconciliados](../Transactions/TransactionStatus.md). Vindo do painel, acompanha o interruptor de lá. |
| **Considerar investimentos restritos no fluxo** | Começa ligado. Liga ou tira a aplicação e o resgate de FGTS e previdência privada. |
| **Moeda para exibição** | Converte os totais para a moeda escolhida. |

Ao voltar para a tela, os números são recalculados.

---

## O que entra

Só movimento de **conta bancária**, na data do lançamento.

- **Receita** na conta: entrada.
- **Despesa** na conta: saída. Um [estorno](../Transactions/Reversal.md) reduz essa saída.
- **Pagamento de fatura**: saída, no dia em que o dinheiro sai da conta.
- **Saque** para a carteira: saída. **Depósito** da carteira na conta: entrada.
- **Aplicação** em investimento de [liquidez restrita](../Investments/ManageInvestmentAccount.md#tipo-de-investimento) (FGTS e previdência): saída. **Resgate**: entrada. O filtro precisa estar ligado.

---

## O que fica de fora

- **Compra no cartão.** Ela entra no resultado por categoria, no mês da compra. Aqui só o pagamento da fatura.
- **Gasto pago direto com a carteira.** A carteira só aparece na hora do saque ou do depósito.
- **Transferência entre duas contas bancárias** que estão no relatório. O dinheiro mudou de conta; o caixa total não mudou. Se o filtro deixar só uma das contas, a transferência passa a contar.
- **Aplicação e resgate** de investimento com liquidez (CDB, poupança, fundo e os outros grupos). O dinheiro continua seu. O filtro de restritos não muda isso.
- **Aporte direto** no investimento, sem passar pela conta bancária.
- **Saldo inicial** da conta. Ele não é tratado como entrada do período.
- **Saque no cartão.** O efeito no caixa fica no pagamento da fatura, para não contar duas vezes.

Mês em que todo lançamento ficou de fora some da lista. A tela não mostra um mês zerado no lugar.

---

## O gráfico e o detalhe

Cada mês tem três barras: **Entradas** (verde), **Saídas** (vermelho) e **Saldo** (azul). Entradas e saídas usam o tamanho do valor. O saldo guarda o sinal: saldo negativo desce.

No detalhe mensal, toque em:

- **Entradas** — os lançamentos que entraram naquele mês. O título fica “Fluxo de Caixa - Entradas - Jun 2026”.
- **Saídas** — os que saíram.
- **Saldo** — os dois juntos.

A lista é de análise: não há botão de incluir. Um valor zerado não abre lista.

Com **Saldo acumulado** ligado, junho da captura mostraria R$ 2.500,00, julho R$ 5.530,00 (2.500 + 3.030) e agosto R$ 7.830,00, o saldo do período.

Sem movimento no período, a tela avisa: “Nenhuma transação encontrada para o período selecionado”.

Se faltar taxa de câmbio, o aviso no topo lista o par. Esse lançamento fica fora dos totais e continua na lista ao tocar o mês. Veja [Quando falta uma taxa](../Transactions/CurrencyConversion.md#quando-falta-uma-taxa).

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| O total é maior que o card do painel | O card é o mês corrente. A tela abre no acumulado do ano. Troque para **Mensal**. |
| A compra do cartão não aparece | Esperado. Ela entra no mês do pagamento da fatura. |
| Transferi da conta A para a conta B e nada mudou | As duas contas estão no relatório. O caixa total não muda. |
| Apliquei num CDB e o saldo do período não caiu | Investimento com liquidez fica de fora. FGTS e previdência entram, se o filtro de restritos estiver ligado. |
| Um previsto sumiu | **Incluir transações previstas** está desligado. |
| O total está menor do que a soma dos lançamentos | Falta taxa de câmbio. O aviso no topo indica o par. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
