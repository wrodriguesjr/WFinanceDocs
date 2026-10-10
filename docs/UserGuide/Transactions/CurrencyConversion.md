# Conversão de moeda

Cada lançamento pode ter dois valores: o da **operação** (o que você pagou ou recebeu) e o da **conta** (o mesmo movimento já na moeda da conta ou do cartão). Quando as moedas coincidem, os dois são o mesmo número e a faixa de câmbio fica oculta.

Os outros guias estão em [Transações](Transactions.md). Os botões de recarregar e editar a taxa, no formulário, estão em [Como lançar uma transação](ManageTransaction.md#quando-a-conversão-de-moeda-aparece).

---

## Quando a seção aparece

A seção **Conversão de moeda** entra na tela de criação quando a moeda da transação é diferente da moeda da conta ou do cartão.

Ela também aparece em **transferência** entre contas de moedas diferentes. Nesse caso, a moeda do lançamento fica presa à moeda da **conta origem**. Cada lado guarda o valor na moeda daquela conta.

O título da faixa é “Taxa e data de conversão para a moeda da conta”.

---

## Uma despesa de 10 dólares

A lembrança de viagem foi lançada em **dólar** no cartão **Mastercard família**, que é em reais. Por isso a conversão aparece.

![Despesa de US$ 10 no cartão em reais, com taxa e valor convertido](Transacoes%20-%20Despesa%20em%20outra%20moeda.png)

| Campo | Na captura |
|-------|------------|
| Tipo | Despesa |
| Descrição | Lembrança de viagem |
| Valor | US$ 10,00 |
| Data | 05/10/2026 |
| Conta | Mastercard família, fatura de novembro de 2026 |
| Categoria | Viagens/Férias · Outros |
| Taxa | 5,15380, na data da compra |
| Valor na moeda do cartão | R$ 51,54 |

O cartão registra os **R$ 51,54**. O lançamento continua guardando os **US$ 10,00**, para você saber o preço original.

10 × 5,15380 = 51,538, que o app mostra como R$ 51,54.

Ao lado da taxa há dois ícones: um recarrega a cotação da data, o outro limpa a taxa para você informar outra.

---

## De onde vem a taxa

O app usa a taxa do dia da transação, ou a que você digitar. As moedas que você usa com mais frequência ficam em Central → Estrutura financeira → **Moedas preferenciais**. As cotações ficam em **Taxas de câmbio**.

Sem taxa para aquela data, a conversão não inventa um número: a faixa pede a cotação.

---

## Quando falta uma taxa

Totais, metas, reservas e relatórios também convertem valores para uma moeda só. Duas regras valem para todos:

- **A taxa é sua.** Cada pessoa cadastra as próprias taxas. Num espaço compartilhado, a taxa de outro membro não vale para você: o mesmo relatório pode abrir para ele e avisar para você.
- **A data importa.** O app usa a taxa mais recente com data **até** a data do valor. Uma taxa cadastrada hoje não converte um lançamento de fevereiro. Por isso os avisos mostram “com data até 01/02/2026”: cadastre a taxa nessa data ou antes.

O app nunca soma um valor em dólar como se fosse real. O que não converte fica de fora, e a tela avisa com o ícone de câmbio:

| Onde | O que acontece |
|------|----------------|
| [Reservas](../Reserves/ReserveScreen.md#de-onde-vem-o-total) | O total soma só as contas que converteram. A conta sem taxa aparece com o saldo na moeda dela, e a barra de progresso some. |
| [Metas](../Goals/GoalScreen.md#o-que-entra-no-atingido) | Atingido e meta mostram só o que converteu. Percentual, barra e sobra somem até a taxa existir. |
| Relatórios de categorias, tags, fluxo de caixa e faturas | O relatório abre com os valores que converteram. Um aviso no topo lista as moedas que ficaram de fora e a data de cada taxa. |
| Relatórios de patrimônio, extratos e [investimentos](../Investments/InvestmentScreen.md#moeda) | O relatório não abre. Saldos são fotos de cada mês: uma conta faltando inventaria ganho ou perda. O aviso lista **todas** as taxas que faltam, de uma vez. |
| [Projeção das metas](../Goals/GoalForecast.md) | A tela mostra o erro e não calcula. |

As taxas ficam em Central → Estrutura financeira → **Taxas de câmbio**.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
