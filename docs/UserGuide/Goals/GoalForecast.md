# Projeção das metas

A projeção estima **como o ano fecha em dezembro**. Ela olha o que você já gastou nos meses que já terminaram e completa o resto do ano de um de dois jeitos: repetindo a meta que falta, ou repetindo o ritmo em que você tem gastado.

Os outros guias estão em [Metas de gastos](Goals.md). A lista do dia a dia está em [A tela de metas](GoalScreen.md).

---

## Como chegar

Central → Planejamento → **Projeção anual das metas**.

A tela não tem filtro de mês. Ela olha o **ano que está no título**. Em outubro, o título é “Projeção das metas de 2026”.

---

## O que a tela está olhando

Os meses se dividem em dois grupos.

- **Meses fechados** — de janeiro até o mês anterior ao atual. São a base. Em outubro, a base é janeiro a setembro: **9 meses fechados**.
- **Meses que ainda vêm** — do mês atual até dezembro. Em outubro, são outubro, novembro e dezembro.

O mês em que você está não entra no “já gastei”. Ele ainda não fechou. Lançamento previsto também fica de fora. Entram despesas **efetivadas** ou **reconciliadas**. Estorno reduz o que já foi gasto.

Em janeiro nenhum mês fechou. A tela avisa que ainda não há base para projetar. A partir de fevereiro, janeiro passa a contar.

---

## Um exemplo, em outubro

A captura abaixo está no modelo **Metas futuras**. A base é janeiro a setembro.

![Projeção de 2026 em outubro, no modelo Metas futuras](Metas%20-%20projecao%20anual.png)

### O que já aconteceu, nas categorias com meta

| | Valor | Em palavras |
|--|-------|-------------|
| **Meta** | R$ 42.498,43 | A soma dos tetos de janeiro a setembro. |
| **Realizado (jan a set)** | R$ 34.602,73 | O que você já gastou nessas mesmas categorias. |
| **81%** | | 34.602,73 ÷ 42.498,43. Até setembro, o gasto ficou em 81% do que estava planejado. |

O 81% está em laranja: na mesma escala da lista de metas, de 80% a 99% é “perto do teto”, ainda abaixo de 100%.

### Para onde o ano vai, se daqui para a frente você cumprir a meta

| | Valor | Em palavras |
|--|-------|-------------|
| **Meta no ano** | R$ 47.848,43 | A soma dos tetos de janeiro a dezembro. |
| **Projetado até dez** | R$ 39.952,74 | O que já foi gasto, mais a meta que ainda falta em outubro, novembro e dezembro. |
| **83%** | | 39.952,74 ÷ 47.848,43. É o anel laranja. |

A conta do meio, em voz alta: a meta do ano menos a meta até setembro deixa **R$ 5.350,00** para os três meses que faltam (47.848,43 − 42.498,43). Somando isso ao que já foi gasto: 34.602,73 + 5.350,00 = **R$ 39.952,73**, que a tela mostra como R$ 39.952,74.

Ou seja: o modelo não repete um gasto atípico de janeiro. Ele assume que, nos meses que faltam, você gasta **o teto que cadastrou** para esses meses.

### O outro botão mudaria esse número

**Meu ritmo atual** olha o 81% e imagina que outubro, novembro e dezembro também fiquem em cerca de 81% da meta deles. O projetado até dezembro fica menor do que R$ 39.952,74, e o percentual do ano tende a continuar perto dos 81%, em vez de subir para 83%.

Realizado, meta até setembro e meta do ano **não mudam** quando você troca o botão. O que muda é o **projetado até dezembro** e o anel.

### Gastos que não têm meta

Embaixo, **Projeção de despesas sem metas** junta o que você gastou em categorias sem teto.

| | Valor |
|--|-------|
| **Realizado (jan a set)** | R$ 9.187,94 |
| **Projetado até dez** | R$ 12.250,59 |

São cerca de R$ 1.021 por mês nos nove meses fechados. Doze meses nesse mesmo ritmo dão R$ 12.250,59.

Esse bloco é uma média. Trocar entre **Metas futuras** e **Meu ritmo atual** não mexe nele. A tela lembra que esse dinheiro também sai até o fim do ano, mesmo sem teto cadastrado.

---

## Os dois modelos

A tela abre em **Metas futuras**.

O aviso perto dos botões vale para os dois: a projeção é uma conta em cima do passado. Quanto menos meses fechados, mais um gasto fora do comum pesa no resultado.

### Metas futuras

Pega o que você já gastou e soma a **meta dos meses que faltam**.

Serve para gasto que você já sabe quanto vai ser: aluguel, condomínio, mensalidade. Um conserto em janeiro não é copiado para o resto do ano. A referência dos meses que faltam continua sendo o teto cadastrado.

Uma meta anual continua valendo nesses meses. Um IPVA pago inteiro em janeiro ainda entra com a fatia de outubro, novembro e dezembro, se a meta anual existir.

### Meu ritmo atual

Pega o que você já gastou e soma a meta dos meses que faltam **multiplicada pelo seu ritmo**.

O ritmo é o realizado dividido pela meta dos meses fechados. No exemplo, 81%. Quem está acima da meta vê os meses que faltam também acima, na mesma proporção.

Serve para gasto que varia: supermercado, lazer, delivery, combustível.

- Mês que não tem meta continua em zero. Um IPVA com teto só em janeiro não é espalhado pelos outros meses.
- Se o realizado dos meses fechados for zero, a projeção fica igual ao que já foi gasto.
- Se não houver meta nenhuma nos meses fechados, a linha usa a média mensal vezes 12.

O ritmo não tem teto. Quanto maior a diferença entre o gasto e a meta até aqui, maior o número. Um presente ou uma viagem nos primeiros meses é espalhado pelo resto do ano de propósito: é o que esse modelo faz. Com poucos meses fechados, o efeito é forte. Em fevereiro, com só janeiro de base, um gasto atípico pode dobrar a projeção. Conforme o ano avança, a base cresce e o efeito diminui.

Se você não quer esse espalhamento, use **Metas futuras**.

O mesmo aviso está no link **Como funciona a projeção?**, no topo da tela.

---

## Por categoria

A lista começa fechada. Toque em **Ver projeções por categoria** para abrir. O mesmo controle passa a ocultá-la. Sem meta no ano, o controle não aparece.

Só entram categorias e subcategorias de despesa com meta no ano.

- **Categoria com meta** — uma linha da categoria. O gasto das subcategorias entra nela. A meta da subcategoria não vira outra linha e não soma no limite.
- **Categoria sem meta, subcategoria com meta** — uma linha para cada subcategoria.
- **Sem meta nenhuma** — não aparece na lista. O gasto vai para **despesas sem metas**.

Exemplos:

- Alimentação tem meta de R$ 10.000 e Mercado, de R$ 4.000. A lista mostra só Alimentação, com meta de R$ 10.000. O gasto de Mercado entra em Alimentação.
- Veículo não tem meta. Combustível, IPVA e Manutenção têm. A lista mostra as três. Estacionamento, sem meta, vai para as despesas sem metas.

Lançamento sem categoria não entra em nenhum dos dois blocos. Tocar numa linha não abre detalhe.

Cada linha repete a lógica do topo: realizado e meta dos meses fechados, projetado e meta do ano, e o percentual. As cores são as mesmas da lista de metas: verde abaixo de 80%, laranja de 80% a 99%, vermelho a partir de 100%.

A meta de cada mês segue a [tela de metas](GoalScreen.md#um-card-várias-metas): um doze avos da meta anual, mais a meta mensal daquele mês.

---

## Moedas

Cada linha usa a **moeda da meta**. O topo converte tudo para a **sua moeda** antes de somar.

Meses fechados usam a taxa do último dia do mês. Meses que ainda vêm usam a taxa mais recente.

Se faltar taxa, a tela não calcula e mostra o erro. Cadastre a taxa e volte.

---

## Atualização

A tela se atualiza sozinha enquanto está aberta: ao criar, editar ou excluir uma meta do ano, ou ao lançar, editar ou excluir uma transação do ano.

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| “Não há dados suficientes” | É janeiro. A projeção começa em fevereiro. |
| Gasto deste mês não aparece no realizado | O mês atual só entra na base quando fechar. |
| Subcategoria com meta não aparece na lista | A categoria dela tem meta. O gasto está na linha da categoria. |
| Projeção muito alta no começo do ano, em Meu ritmo atual | Poucos meses fechados e algum gasto pontual. Use Metas futuras se quiser repetir o teto, não o ritmo. |
| Despesas sem metas não mudam com o botão | Esperado. Esse bloco é sempre a média mensal vezes 12. |
| Erro de taxa de câmbio | Falta taxa para uma das moedas das metas ou das transações. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
