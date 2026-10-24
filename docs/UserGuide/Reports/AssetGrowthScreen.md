---
description: Tela de evolução de patrimônio do WFinance — o saldo das contas no fim de cada mês.
---

# A tela de evolução de patrimônio

A tela abre no **acumulado do ano**, de janeiro até o mês atual, na moeda padrão do seu perfil. O título é **Evolução de Patrimônio**.

O que o relatório mede está em [Evolução de patrimônio](AssetGrowth.md).

---

## Período

As setas trocam o intervalo. O toque no título abre o tipo de período.

| Tipo | O que mostra |
|------|----------------|
| **Trimestral** | Os três meses do trimestre, cada um com o saldo de fim de mês. |
| **Anual** | Janeiro a dezembro. |
| **3 Meses**, **6 Meses**, **12 Meses** | A janela que termina no mês na tela. |
| **Acumulado no ano** | De janeiro até o mês na tela. É o padrão ao abrir. A [captura](AssetGrowth.md#de-janeiro-a-outubro-de-2026) está nesse modo. |

Não há visão de um mês só.

---

## Os três níveis

Os chips ficam abaixo dos filtros. Nenhum marcado significa os três níveis.

| Chip | O que soma |
|------|------------|
| **Disponível imediato** | Contas bancárias e carteira. |
| **Investimentos com liquidez** | Contas de investimento, exceto FGTS e previdência. |
| **Investimentos restritos** | FGTS e previdência privada. |

Marcar um ou mais chips limita o gráfico, a lista e o resumo a esses níveis. O patrimônio total e a variação passam a ser só do que está marcado. Desmarcar todos devolve os três.

---

## Filtros

O bloco **Filtros** começa fechado.

| Filtro | O que faz |
|--------|-----------|
| **Contas (bancárias, carteira, investimentos)** | Vazio significa todas, inclusive inativas. |
| **Tipos de investimento** | Vazio significa todos. Com tipos marcados, só esses investimentos entram. Conta bancária e carteira continuam. |
| **Incluir transações previstas** | Começa desligado. Ligado, o saldo de fim de mês também leva os lançamentos [previstos](../Transactions/TransactionStatus.md). |
| **Moeda para exibição** | Converte cada saldo com a taxa do **último dia daquele mês**. |

Ao voltar para a tela, os números são recalculados.

---

## O gráfico e a lista

Cada mês é uma barra empilhada: verde na base (disponível imediato), azul no meio (investimentos com liquidez) e laranja no topo (restritos), quando o nível está ligado.

A linha branca, **Patrimônio Total**, entra quando algum nível fica negativo em algum mês. Ela marca o saldo do mês mesmo que uma faixa da barra atravesse o zero. Sem saldo negativo no período, o gráfico fica só com as barras.

A lista repete o mês: o valor de cada nível, a fatia dele no total daquele mês e o total. O toque na linha não abre lançamentos. Esta tela é a posição, não o movimento.

Sem conta no período, a tela avisa: “Nenhum dado encontrado para o período selecionado”.

---

## Moeda

Se faltar taxa para algum saldo, a tela não calcula. O aviso lista os pares e a data de cada um, e o gráfico some até a taxa existir. Uma taxa faltando num mês e presente no outro mudaria a variação sem o dinheiro ter mudado.

Cadastre a taxa em Central → Estrutura financeira → **Taxas de câmbio**. Mais em [Quando falta uma taxa](../Transactions/CurrencyConversion.md#quando-falta-uma-taxa).

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| O percentual passou de 1000% | A base é pequena. Na captura, R$ 1.000,00 viraram R$ 19.670,00, e a tela mostra +1867,0%. |
| A fatura do cartão não reduziu o patrimônio | Cartão não entra. A dívida da fatura fica de fora desta conta. |
| FGTS não aparece | O chip **Investimentos restritos** está desmarcado, ou o filtro de tipos de investimento o excluiu. |
| Apliquei num CDB e o disponível imediato caiu | O dinheiro saiu da conta e foi para **Investimentos com liquidez**. O total muda pelo saldo das duas contas no fim do mês. |
| Um previsto não mudou o saldo | **Incluir transações previstas** começa desligado. |
| A tela só mostra o aviso de câmbio | Falta taxa no fim de algum mês. O relatório não mostra número parcial. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
