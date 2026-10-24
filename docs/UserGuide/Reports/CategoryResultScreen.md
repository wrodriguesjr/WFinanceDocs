---
description: Tela de receitas e despesas do WFinance — resultado do mês por categoria.
---

# A tela de resultado por categoria

A tela abre no **mês atual**, na moeda padrão do seu perfil. O título é **Receitas e Despesas**.

O que o relatório mede está em [Resultado por categoria](CategoryResult.md). Status dos lançamentos: [Status](../Transactions/TransactionStatus.md).

---

## Período

As setas trocam o intervalo. O toque no título abre o tipo de período.

| Tipo | O que soma |
|------|------------|
| **Mensal** | O mês na tela. É o padrão. |
| **Trimestral** | Os três meses do trimestre. |
| **Anual** | Janeiro a dezembro daquele ano. |
| **3 Anos** | Do ano na tela até dois anos à frente. |
| **5 Anos** | Do ano na tela até quatro anos à frente. |
| **3 Meses**, **6 Meses**, **12 Meses** | A janela que termina no mês na tela. Em outubro, 3 meses é agosto a outubro. |
| **Acumulado no ano** | De janeiro até o mês na tela. |

---

## Filtros

O bloco **Filtros** começa fechado. O número ao lado do título conta quantos filtros estão fora do padrão.

| Filtro | O que faz |
|--------|-----------|
| **Mostrar subcategorias** | Abre todas de uma vez. Desligado, cada categoria abre pelo chevron. Os totais não mudam. |
| **Considerar transações previstas** | Começa ligado. Desligado, ficam só lançamentos [efetivados e reconciliados](../Transactions/TransactionStatus.md). |
| **Valores em cor neutra** | Tira o verde e o vermelho dos valores. As barras de percentual continuam coloridas. |
| **Moeda para exibição** | Converte os totais para a moeda escolhida. |
| **Contas bancárias, carteiras e cartões** | Vazio significa todas. |
| **Categorias de receita** | Restringe as receitas. Se só esta lista tiver seleção, as despesas somem da tela. |
| **Categorias de despesa** | Restringe as despesas. Se só esta lista tiver seleção, as receitas somem da tela. |
| **Tags** | Entra o lançamento que tiver pelo menos uma das tags marcadas. Vazio ignora tag. |

Com as duas listas de categoria preenchidas, cada tipo usa a sua lista. Receita que não está na lista de receitas fica de fora; despesa que não está na lista de despesas também.

O ícone de limpar devolve os filtros ao padrão.

Ao voltar para a tela, os números são recalculados.

---

## A lista

Receitas ficam em cima, despesas embaixo. Dentro de cada bloco, o maior valor vem primeiro.

- O **chevron** abre e fecha as subcategorias daquela linha.
- O **toque no nome** abre os lançamentos da categoria. A lista é só para análise: não há botão de incluir.
- O toque numa **subcategoria** abre só os lançamentos dela.
- Lançamento da categoria sem subcategoria aparece como **Nome da categoria (direto)**.

A barra é a participação da categoria no total do tipo. O texto mostra uma casa decimal. Com [estorno](../Transactions/Reversal.md), uma categoria pode ficar com sinal oposto ao do bloco: o texto mostra o percentual real, e a barra para em 0% ou em 100%.

Sem receita e sem despesa no período, a tela avisa: “Nenhuma transação encontrada para o período selecionado”.

---

## Moeda

O card acima do resumo mostra a moeda em que os totais estão. Lançamento em outra moeda é convertido com a taxa cadastrada.

Se faltar taxa, um aviso no topo lista o par e até que data ela precisa existir. Esse lançamento fica fora dos totais e continua abrindo quando você toca a categoria. Cadastre a taxa em Central → Estrutura financeira → **Taxas de câmbio**. Mais em [Quando falta uma taxa](../Transactions/CurrencyConversion.md#quando-falta-uma-taxa).

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| A tela está vazia | Não há receita nem despesa com categoria nesse período. Transferência e lançamento sem categoria não entram. |
| A compra do cartão apareceu em outro mês | A data usada é a do lançamento, a da compra. O pagamento da fatura não move essa compra. |
| Um previsto sumiu | O filtro **Considerar transações previstas** está desligado. |
| As receitas sumiram ao filtrar despesa | Há seleção só em **Categorias de despesa**. Limpe esse filtro para as receitas voltarem. |
| O total está menor do que a soma dos lançamentos | Falta taxa de câmbio. O aviso no topo indica o par. |
| O percentual passa de 100% ou fica negativo | Um estorno inverteu o sinal de alguma categoria do bloco. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
