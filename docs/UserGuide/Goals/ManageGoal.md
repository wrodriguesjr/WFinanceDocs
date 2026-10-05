# Como cadastrar uma meta

Esta página é o passo a passo da tela que **cria, edita e copia** um teto de gasto. Os outros guias estão em [Metas de gastos](Goals.md). O que a lista mostra está em [A tela de metas](GoalScreen.md).

---

## Como chegar

| Ação | De onde |
|------|---------|
| **Criar** | Botão **+** na tela de metas. Abre sempre no **ano e mês de hoje**, mesmo que o filtro esteja em outro período. |
| **Editar** | Toque no card → em **Metas do período**, o lápis da linha. |
| **Copiar** | Toque no card → o ícone de copiar da linha. Traz ano, mês e tipo da meta copiada, não a data de hoje. |

É preciso ter pelo menos uma **categoria de despesa**. Sem ela, o **+** avisa e não abre o formulário. Quem está no espaço só para visualizar não cria nem altera metas.

Se você sair sem gravar, o app pergunta se quer descartar.

---

## O que esta tela pede

### Tipo: mensal ou anual

- **Mensal** — o teto vale só naquele mês. Aparece o seletor de mês.
- **Anual** — o teto vale de janeiro a dezembro. O app divide o valor em 12 partes iguais na lista. O seletor de mês some.

Os dois tipos **podem coexistir** no mesmo recorte. Uma anual de R$ 1.200 e um extra de R$ 50 em março somam: março fica com R$ 150. Não há “a mensal substitui a anual”.

Na **edição**, o tipo (e o mês) ficam travados. Para mudar o período, copie ou exclua e crie outra.

### Categoria ou subcategoria

Toque no bloco da categoria. A lista mostra só categorias de **despesa**.

- Escolher a **categoria** (Alimentação, Veículo…) cobre todas as subcategorias daquele grupo. Na lista isso aparece como “(meta geral da categoria)”.
- Escolher uma **subcategoria** (Mercado, Combustível…) cobre só aquele recorte.

Os dois podem existir ao mesmo tempo e viram **cards separados**. Na edição, a categoria também fica travada.

### Ano (e mês)

O ano pode ser o atual, até dois anos para trás ou alguns à frente.

Na criação pelo **+**, ano e mês já vêm **de hoje**. Na cópia, vêm da meta de origem — útil para repetir o teto de janeiro em fevereiro, ou de 2026 em 2027.

Na edição, ano e mês ficam travados.

### Valor e moeda

O teto que você quer respeitar naquele período. Precisa ser maior que zero.

Todas as metas do **mesmo recorte e mesmo ano** precisam da **mesma moeda**. O app recusa gravar se já existir outra em moeda diferente. Anos diferentes podem usar moedas diferentes.

Na edição, **só valor e moeda** mudam.

---

## O que o app não deixa gravar

| Recado | Por quê |
|--------|---------|
| Selecione uma categoria | A meta precisa de um recorte de despesa. |
| Insira um valor válido | Zero ou vazio não são teto. |
| Já existe uma meta para esta categoria neste mês/ano | Não dá para ter duas anuais iguais, nem duas mensais do mesmo mês. Anual + mensal, sim. |
| Já existe uma meta desta categoria neste ano em outra moeda | No mesmo ano o card soma os limites; isso só funciona numa moeda só. |
| Você não tem permissão para editar metas neste grupo | Papel de somente leitura neste espaço. |

No plano **Free** há limite de **5 metas por espaço**. Cada linha que você grava conta (anual + três mensais = 4), ainda que a lista mostre um único card. O Premium remove esse teto — veja [Conta de usuário](../UserAccount.md).

---

## Depois de salvar

A lista de metas atualiza sozinha. O novo teto entra no card daquela categoria, no período em que o intervalo do filtro o alcança.

Se a lista parecer vazia, mude o filtro: uma meta de dezembro não aparece no acumulado até março. Detalhes em [A tela de metas](GoalScreen.md#a-tela).

Editar o valor **zera o histórico de avisos** de 80% e 100% daquela meta, para o app poder avisar de novo se o teto for cruzado.

---

## Dicas rápidas

- Comece com uma **anual** da categoria grande e acrescente **mensais** só nos meses atípicos (férias, IPVA, presente de fim de ano).
- Use subcategoria quando quiser um teto mais apertado dentro do grupo (Combustível dentro de Veículo).
- Copiar é o caminho mais rápido para repetir o mesmo teto em outro mês ou no ano seguinte.
- Lançamentos **previstos** não empurram a meta. Efetive quando o gasto acontecer.
- Reembolso é [estorno de despesa](../Transactions/Reversal.md): a meta desce, sem virar receita.
- Metas não substituem [reservas](../Reserves/Reserves.md). Teto de gasto é uma coisa; dinheiro separado para um objetivo é outra.
