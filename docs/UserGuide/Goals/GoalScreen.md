# A tela de metas

A lista compara o teto que você cadastrou com as despesas já feitas no período que você está olhando.

Os outros guias estão em [Metas de gastos](Goals.md). Criar ou editar um teto: [Como cadastrar uma meta](ManageGoal.md). Estimar o ano até dezembro: [Projeção das metas](GoalForecast.md).

---

## Como chegar

| Caminho | Observação |
|---------|------------|
| Ícone de **metas** na barra inferior | A tela completa, com filtro de período. |
| Central → Planejamento → Metas de gastos | Mesma tela. |
| Painel inicial → **Ir para metas** | O card da home mostra só as 3 de maior desvio no mês. |
| Aviso de 80% ou 100% | O toque na notificação abre esta tela. |

É preciso ter pelo menos uma **categoria de despesa**. Sem ela, o botão de adicionar avisa e não abre o formulário.

---

## O que cada meta guarda

- **categoria** ou **subcategoria** de despesa;
- **ano**;
- **mês** (meta mensal) ou o ano inteiro (meta **anual**);
- **valor** e **moeda**.

Duas metas no mesmo recorte **somam**. Uma anual de Alimentação e uma mensal de março de Alimentação convivem e entram no mesmo card.

Categoria e subcategoria são recortes **independentes**. Uma meta de Veículo (a categoria toda) e outra de Combustível (subcategoria) viram **dois cards**. Uma despesa de combustível conta nos dois. São perguntas diferentes: “quanto gastei em veículo?” e “quanto gastei em combustível?”.

Só transações de **despesa** entram. Receitas e transferências ficam de fora. [Estorno de despesa](../Transactions/Reversal.md) (reembolso, devolução) reduz o atingido.

---

## A tela

A lista abre no **acumulado no ano**: de janeiro até o mês atual.

![Lista de metas no acumulado de janeiro a junho](Metas%20-%20Acumulado%20Jan%20a%20Jun.png)

De cima para baixo:

- o filtro de período (setas, calendário e o intervalo por extenso);
- o link **Como funcionam as metas?**, se a ajuda contextual estiver ligada;
- um **card por categoria ou subcategoria** que tenha meta naquele intervalo.

Não há um card por meta cadastrada. Se Veículo tem uma meta anual e duas mensais, isso aparece como **um** card. O selo no canto (“2026”, “Jan 2026” ou “2 metas”) diz quais limites entram no intervalo.

O botão **+** cria uma meta **no mês de hoje**, mesmo que o filtro esteja em outro período. O passo a passo está em [Como cadastrar uma meta](ManageGoal.md).

Se a lista estiver vazia, o texto pede para criar uma meta ou mudar o período. Uma meta só de dezembro não aparece no acumulado até março. Ela volta quando o intervalo inclui dezembro.

---

## Um card, várias metas

A meta **anual** é dividida em 12 partes iguais. A de um **mês** se soma à parte daquele mês.

Exemplo, como no card de Veículo da captura:

| O que está cadastrado | Valor |
|-----------------------|-------|
| Meta anual de 2026 | R$ 1.200 (R$ 100 por mês) |
| Extra em janeiro | R$ 2.500 |
| Extra em julho | R$ 1.200 |

Olhando **janeiro até junho**:

- **Meta** do intervalo = 6 × R$ 100 + R$ 2.500 de janeiro = **R$ 3.100**. Julho ainda não entra.
- **Meta (anual)** = os três cadastros = **R$ 4.900**. Julho já conta, porque é o teto do ano inteiro.
- **Atingido** = o que você já gastou de janeiro a junho.

O mesmo card pode mostrar “2 metas” no selo (as que valem no intervalo) e, nos detalhes, **três** linhas (incluindo julho, que é do mesmo ano).

---

## Períodos

O filtro fica **dentro de um único ano**. Não há visão que cruze 2025 e 2026.

| Visão | Intervalo | O que o card destaca |
|-------|-----------|----------------------|
| **Acumulado no ano** (padrão) | 1º de janeiro até o mês escolhido | Atingido, meta do intervalo, **saldo** e **meta do ano** |
| **Mensal** | Só aquele mês | Gasto do mês contra o limite daquele mês (a anual entra pela parte do mês) |
| **Trimestral** | Os 3 meses do trimestre | Soma dos limites e dos gastos dos três meses |
| **Anual** | Janeiro a dezembro | O ano inteiro |

Saldo e meta do ano só aparecem no acumulado. Nas outras visões o card fica mais enxuto: atingido, meta do intervalo e percentual.

Se você estiver na visão anual e voltar para o acumulado, o app mostra até **dezembro** daquele ano. Use as setas para voltar ao mês atual.

---

## Os números do card

| Campo | Significado |
|-------|-------------|
| **Atingido** | Soma das despesas efetivadas ou reconciliadas daquele recorte, no intervalo do filtro. |
| **Meta** | Soma dos limites dos meses que estão no intervalo. |
| **Saldo** | Meta menos atingido. Fica vermelho se passou do teto. Só no acumulado. |
| **Meta (anual)** | Soma dos limites dos 12 meses, inclusive meses depois do selecionado. Só no acumulado. |
| **Progresso** | Atingido dividido pela meta, em % inteiro. |

Cores da barra e do percentual:

| Faixa | Cor |
|-------|-----|
| Abaixo de 80% | Verde |
| 80% a 99% | Laranja |
| 100% ou mais | Vermelho |

A barra visual para em 100%. O número escrito pode passar disso: 130% aparece escrito, com a barra cheia.

Quem está no espaço só para visualizar vê a lista, sem criar, editar nem excluir.

---

## O que entra no atingido

Entram lançamentos:

- do tipo **despesa** (estorno de despesa diminui o total);
- com status **efetivado** ou **reconciliado**;
- da categoria ou subcategoria do card;
- com data **dentro do intervalo** que o filtro está mostrando.

Previsto fica de fora. Quando o lançamento vira efetivado, o card atualiza sozinho.

O intervalo inteiro conta, mesmo nos meses em que você não cadastrou meta. Se existe teto só em janeiro e você olha o 1º trimestre, o limite é o de janeiro, mas o atingido soma janeiro, fevereiro e março. O percentual pode passar de 100%. O card responde “quanto gastei no período que estou olhando”.

Valores em outra moeda são convertidos pela taxa da **data do lançamento**, para a moeda da meta.

---

## Detalhes da meta

Toque no card. Editar, copiar e excluir ficam aqui.

![Detalhes da meta, com limites do ano e gráfico mensal](Metas%20-%20Bottom%20sheet%20v2.png)

### Ver transações da meta

Abre a lista das despesas que formaram o **atingido do card**, no mesmo intervalo do filtro. No exemplo, “Jan 2026 até Jun 2026”. É o conjunto do card, não de uma linha só.

A lista abre em [modo relatório](../Transactions/TransactionLists.md#modo-relatório): aqueles lançamentos, sem incluir novos.

### Metas do período

Uma linha para cada limite cadastrado naquele recorte. Anual primeiro, depois os meses.

No acumulado e na visão anual, a lista traz **todas as mensais do ano**, inclusive meses que ainda não estão no filtro. Por isso julho aparece mesmo com a tela em janeiro–junho.

Em cada linha: **editar**, **copiar** e **excluir**. Excluir pede confirmação. Se era o último limite do card, a ficha fecha.

Pela **home**, essa ficha abre sem esses três ícones: o painel só consulta.

### Gráfico

Os **12 meses do ano** do filtro. As barras são o gasto de cada mês. A linha tracejada é o limite daquele mês (parte da anual mais o extra mensal, se houver).

Meses futuros ficam mais claros. A barra pode ficar negativa se, naquele mês, os estornos superarem as despesas. A soma das barras fecha com o atingido.

---

## No painel inicial

O card de metas da [home](../MainDashboard.md#metas) mostra as **três** com maior desvio no **mês corrente**, misturando percentual e valor estourado. Meta anual entra pela parte daquele mês.

No topo: maior desvio em % e maior estouro em valor, na sua moeda padrão. **Ir para metas** abre esta tela.

---

## Avisos de 80% e 100%

O app pode notificar:

- **80%** — você está perto do teto;
- **100%** — o teto foi atingido.

Cada aviso olha **uma meta cadastrada no período dela inteiro**: o mês todo, ou o ano todo. Na tela, o percentual muda conforme o filtro. Por isso o aviso de uma meta anual pode chegar enquanto a lista, em visão mensal, mostra outro número.

O toque na notificação abre a tela de metas. Se o atingido cair (um estorno, por exemplo), o app pode avisar de novo quando a marca for cruzada outra vez.

---

## Plano e espaço

No **Free**, o teto é de **5 metas por espaço**. O que conta é cada cadastro (anual de Veículo + janeiro + julho = **3**), não o card na lista.

Itens de um espaço em que você só visualiza não se editam. Trocar de espaço na [conta](../UserAccount.md) troca as metas junto: cada espaço tem as suas.

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| Lista vazia, mas você cadastrou meta | O filtro pode não incluir aquele mês. No acumulado até março, meta só de dezembro não aparece. |
| Percentual estourou sem você ter gasto tanto no mês da meta | O atingido soma todo o intervalo do filtro, inclusive meses sem teto. |
| Dois cards para a mesma categoria | Um é a categoria toda. O outro é uma subcategoria. |
| Aviso de 80% ou 100% com % diferente na tela | O aviso usa o período completo daquela meta. A tela usa o filtro. |
| Números não mudam depois de lançar | A despesa precisa estar efetivada ou reconciliada, na mesma categoria ou subcategoria, e no intervalo. |
| Não consigo tocar em + | Falta categoria de despesa, ou você está só para visualizar neste espaço. |
| Meta não soma com a outra no mesmo card | Precisam ser o mesmo recorte e o mesmo ano. Moedas diferentes no mesmo ano não são aceitas. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
