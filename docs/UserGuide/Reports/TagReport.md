# Transações por tag

O relatório **Transações por tag** responde: “quanto esta viagem, esta obra ou este projeto consumiu e gerou?”. Uma tag é um rótulo livre que você coloca no lançamento, ao lado da categoria. O relatório junta, por tag, as receitas e as despesas daquele rótulo.

No menu o nome é **Transações por tag**. A tela se chama **Transações por Tag**.

A data usada é a do lançamento, a mesma do [resultado por categoria](CategoryResult.md). Uma compra no cartão entra no mês da compra. O pagamento da fatura não move esse valor para outro mês.

Os outros relatórios estão em [Relatórios](Reports.md). Como marcar uma tag no lançamento: [Como lançar uma transação](../Transactions/ManageTransaction.md#observações-e-tags).

---

## Como chegar

Central → **Relatórios** → Análises → **Transações por tag**.

A tela abre no mês atual. Entram receitas e despesas que tenham pelo menos uma tag. Previstas entram com o filtro ligado, que é o padrão.

---

## De março a agosto de 2026

A captura usa o período **6 Meses**, terminando em agosto. Há uma tag no recorte: **Europa 2026**.

![Tag Europa 2026, de março a agosto, com R$ 2.700 em viagens](Relatorio%20-%20Tags.png)

### O número da tag

| | Valor | Em palavras |
|--|-------|-------------|
| **Europa 2026** | R$ 2.700,00 | O saldo da tag. Na tela ele aparece negativo: só houve despesa. |

O valor da tag é a soma das receitas e das despesas dela. Despesa entra negativa. Se a tag tivesse uma receita, o número do topo seria o líquido dos dois.

Não há total geral do relatório. Cada tag é uma conta própria.

### O que está dentro

A tag abre em dois blocos, quando existem: **Receitas** e **Despesas**. Nesta captura só há despesas, então o bloco de receitas não aparece.

| Nível | Valor |
|-------|-------|
| **Viagens/Férias** | R$ 2.700,00 |
| Hospedagem | R$ 1.500,00 |
| Passagem aérea | R$ 1.200,00 |

1.500 + 1.200 = 2.700. A categoria fecha com as duas subcategorias, e a tag fecha com essa categoria. Não há barra de percentual: a fatia é pergunta do [resultado por categoria](CategoryResult.md). Aqui o assunto é o recorte da tag.

A ordem é do maior para o menor dentro de cada bloco. Entre as tags, vem primeiro a de maior valor absoluto.

### O que este recorte diz

De março a agosto, a tag Europa 2026 reuniu R$ 2.700,00 de viagem: hospedagem e passagem. Nada com essa tag entrou como receita no período. Um salário sem a tag continua no resultado por categoria e não aparece aqui.

---

## A mesma despesa em duas tags

Um lançamento pode ter várias tags. O valor inteiro entra em cada uma. Uma passagem marcada com **Europa 2026** e **Família** aparece nos dois cards, com os R$ 1.200,00 em cada um.

Por isso somar as tags não dá o gasto do período. O mesmo dinheiro seria contado duas vezes. O relatório olha uma tag de cada vez.

---

## Como ler a lista

- O **chevron da tag** abre receitas e despesas.
- O **toque no nome da tag** abre todos os lançamentos dela. O título fica “Tag: Europa 2026”.
- O **chevron da categoria** abre as subcategorias.
- O **toque no nome da categoria** abre os lançamentos daquela categoria na tag.
- O toque na **subcategoria** abre só ela.
- Lançamento sem subcategoria aparece como **Nome da categoria (direto)**.

A lista é de análise: não há botão de incluir.

O filtro **Mostrar subcategorias** abre as subcategorias. A tag em si continua abrindo pelo chevron dela.

---

## Período e filtros

O período e os demais filtros são os da [tela de resultado por categoria](CategoryResultScreen.md): mês, trimestre, ano, janelas de 3, 6 e 12 meses, acumulado no ano, previstas, moeda, contas e categorias.

O filtro **Tags** aqui escolhe quais tags aparecem. Vazio mostra todas as que tiverem lançamento no período. No resultado por categoria, o mesmo filtro escolhe lançamentos, não cards.

Sem tag no período, a tela avisa: “Nenhuma transação com tag encontrada para o período selecionado”.

Se a ajuda contextual estiver ligada, o link **Como funciona o relatório de tags?** explica a tela de novo dentro do app.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
