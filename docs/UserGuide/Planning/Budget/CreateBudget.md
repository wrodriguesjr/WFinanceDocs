---
description: Como montar um orçamento novo no app ou gerar a planilha, a partir do realizado, da média ou em branco.
---

# Como criar um orçamento

Esta página é a tela **Novo orçamento**. Os outros guias estão em [Orçamento anual](Budget.md). O que fazer com o arquivo depois de baixar: [A planilha](BudgetSpreadsheet.md).

---

## Como chegar

| Ação | De onde |
|------|---------|
| **Criar ou baixar do zero** | Botão **+** na [lista](BudgetScreen.md). |
| **Duplicar ou revisar** | No card do orçamento, o ícone de copiar. A origem fica fixa: é aquele orçamento. |

Quem está no espaço só para visualizar não cria nem altera orçamento.

---

## Como quer criar

Três pontos de partida. A tela só mostra as seções que servem para a escolha.

![Novo orçamento a partir do realizado de 2025, por subcategoria, em reais](Budget%20-%20criar%20orcamento%201.png)

| Modo | O que entra no plano |
|------|----------------------|
| **Usar realizado** | Cada mês recebe o que já foi lançado no mesmo mês de um **ano base**. Preserva a sazonalidade. O texto sob o ano base diz de onde vem cada mês. |
| **Média recente** | A média dos últimos **3, 6 ou 12** meses fechados, repetida nos 12 meses. Mês sem movimento conta como zero. Não preserva a sazonalidade. |
| **Em branco** | Só a estrutura de categorias e subcategorias, sem valores. |

No realizado e na média, o **nível de detalhe** escolhe **Por subcategoria** ou **Só por categoria**. Por subcategoria, cada uma recebe o próprio realizado, e a linha “(geral)” recebe o que ficou sem subcategoria. Só por categoria, uma linha leva o realizado da categoria inteira.

O **ajuste percentual** é opcional. Positivo aumenta, negativo reduz. Em branco, nada muda. Na revisão, o ajuste vale só para os meses que ainda não fecharam.

---

## Ano, moeda e nome

**Ano do novo orçamento** é o ano do plano, não necessariamente o ano de onde vêm os números.

A **moeda** é a do orçamento. No realizado e na média, os lançamentos são convertidos para ela com a taxa da data de cada transação. Faltando taxa, o orçamento **não é criado** e o app lista os pares que faltam. Cadastre as taxas em Central → Estrutura financeira → **Taxas de câmbio** e tente de novo. Na cópia e na revisão, a moeda é a do original e não muda.

**Destino** decide o que o botão de baixo faz.

![Novo orçamento em branco, para criar no app com nome e selo de principal](Budget%20-%20criar%20orcamento%202.png)

| Destino | O que acontece |
|---------|----------------|
| **Criar no app** | Grava o orçamento na lista. Peça um **nome** que ainda não exista naquele ano. A estrela **Definir como principal do ano** marca este como o principal. |
| **Baixar planilha** | Gera o `.xlsx` para você ajustar no computador. Não grava orçamento nenhum até você [importar](BudgetSpreadsheet.md). |

Na cópia, o tipo pode ser **Cópia exata** (os mesmos valores, mês a mês) ou **Revisão**. A revisão só aparece se o ano do orçamento já tem mês fechado: esses meses passam a ser o realizado, e os meses abertos continuam com o orçado.

Nada é gravado antes do botão **Criar orçamento** ou **Baixar planilha**. Voltar descarta o que foi escolhido.

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
