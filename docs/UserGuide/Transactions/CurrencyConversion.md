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

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
