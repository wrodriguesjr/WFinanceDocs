---
description: O resumo de um orçamento, as quatro formas de orçar uma categoria e a edição dos doze meses.
---

# O detalhe do orçamento

Toque num card da [lista](BudgetScreen.md) para abrir este resumo. Os outros guias estão em [Orçamento anual](Budget.md).

---

## O resumo

![Detalhe do orçamento principal, com totais do ano, formas e origem](Budget%20-%20bottom%20sheet%20de%20detalhes.png)

O topo mostra o nome e se ele é o **principal** daquele ano. Os ícones, da esquerda para a direita:

| Ícone | O que faz |
|-------|-----------|
| Lápis | Abre a lista de categorias, para ver e editar. |
| Comparar | Abre [Orçado × realizado](BudgetComparison.md) com este orçamento. |
| Copiar | Abre [Novo orçamento](CreateBudget.md) para duplicar ou revisar. |
| Baixar | Gera a [planilha](BudgetSpreadsheet.md) deste orçamento. |
| Metas | Abre [Metas a partir do orçamento](BudgetGoals.md). |
| Estrela | **Tornar principal**. Só aparece se este ainda não for o principal. |
| Lixeira | Exclui. Se era o principal, outro orçamento do ano assume o lugar. |

Abaixo, receitas, despesas, saldo do ano e saldo médio por mês. **Formas** resume como as categorias foram orçadas. **Origem** diz se nasceu no app ou de qual arquivo veio.

Enquanto uma categoria ou subcategoria estiver em algum orçamento, de qualquer ano, o app não deixa excluí-la.

---

## As quatro formas

O lápis abre todas as categorias de receita e de despesa. O total do card é o orçado do ano. Expanda para ver a linha **(geral)** e as subcategorias.

![Detalhe das categorias, com salário orçado por inteiro e outras linhas sem orçamento](Budget%20-%20tela%20de%20detalhes.png)

Cada categoria usa uma forma:

| Forma | Como preencher | O que a lista mostra |
|-------|----------------|----------------------|
| **Orçamento zero** | Tudo em branco. | **Sem orçamento**. Qualquer gasto nela conta como estouro na comparação. |
| **Categoria inteira** | Só a linha **(geral)**. O valor vale para qualquer subcategoria. | **Categoria inteira**. |
| **Detalhado** | Só as subcategorias. A categoria vale a soma delas. | O total das subcategorias. |
| **Detalhado com folga** | Subcategorias e também a **(geral)**, que vira uma folga para o que não couber no detalhe. | **Folga (geral)** mais as subcategorias. |

**Mostrar categorias inativas** revela as que você desligou. A inativa que já tem valor orçado aparece sempre, para o dinheiro não sumir da lista.

O nome do orçamento se edita no lápis ao lado do título.

---

## Editar uma linha

O lápis de uma linha abre os 12 meses. Valores positivos. Em branco vale zero. **Salvar** com tudo zerado tira a linha do orçamento.

**Atalhos** preenchem os 12 meses; você ainda ajusta antes de salvar.

| Atalho | O que faz |
|--------|-----------|
| **Repetir em todos os meses** | Copia o primeiro mês preenchido. |
| **Anual ÷ 12** | Você digita o total do ano e ele se divide pelos 12 meses. |
| **Igual ao ano anterior** | O realizado dessa linha no ano anterior, mês a mês. |
| **Média dos últimos 3 meses** | A média do realizado dos últimos 3 meses fechados, igual nos 12. |

Orçar uma subcategoria de uma categoria que era **inteira** passa essa categoria para **detalhado com folga**: o valor antigo vira a folga. A tela avisa antes de gravar.

A linha **Criar metas a partir deste orçamento** abre o guia de [metas](BudgetGoals.md).

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
