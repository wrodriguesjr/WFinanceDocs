---
description: Crie ou atualize metas de gastos com os valores do orçamento. Receitas não entram.
---

# Metas a partir do orçamento

Esta ação copia valores do orçamento para [metas de gastos](../Goals/Goals.md). Os dois continuam separados: mudar a meta depois não reescreve o orçamento, e o contrário também vale, até você pedir de novo.

Os outros guias estão em [Orçamento anual](Budget.md).

---

## Como chegar

| Caminho | Onde |
|---------|------|
| Linha **Criar metas a partir deste orçamento** | Na [lista de categorias](BudgetDetail.md) do orçamento. |
| Ícone de metas | No [resumo](BudgetDetail.md) do card. |

Só vale para o **ano corrente e os dois seguintes**. Fora dessa faixa, o ícone não segue e o app explica o motivo. Receitas não viram meta.

Quem está no espaço só para visualizar não aplica a ação.

---

## O que você escolhe

Primeiro, **Selecionar categorias**: só despesas que têm valor orçado, e que estejam ativas. Categoria e subcategoria são escolhas independentes. A linha “(geral)” não vira meta sozinha; o valor dela entra na meta da categoria.

A tela seguinte mostra o que vai mudar, antes de gravar.

![Prévia das metas do orçamento, com o que será criado, atualizado e excluído](Budget%20-%20criar%20metas%20a%20partir%20do%20orcamento.png)

| Coluna | O que significa |
|--------|-----------------|
| **Criar** | Ainda não há meta naquele recorte. |
| **Atualizar** | Já há meta, e o teto passa a ser o do orçamento. |
| **Excluir** | A meta que existe hoje não cabe no formato novo e sai. |

**Detalhe das alterações** abre cada categoria. Nada é gravado antes de **Aplicar**. Se alguma meta for excluída, o app pede confirmação.

O limite de cada mês fica igual ao orçamento daquele mês. Meses iguais podem virar uma meta anual. Meses diferentes podem virar uma meta anual mais algumas mensais, só com a diferença. Por isso o número de metas pode ser maior que o número de categorias.

Metas de categorias que você não marcou ficam como estão. Uma categoria inativa do orçamento não ganha meta; o app avisa antes, se houver outras ativas para seguir.

A meta nasce na moeda do orçamento. Rodar de novo, mesmo a partir de outro orçamento do mesmo ano, atualiza as mesmas metas. Não cria um segundo teto ao lado.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
