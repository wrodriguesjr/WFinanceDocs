# Projeção das metas

A **projeção** mostra para onde seus gastos do ano estão indo. Ela junta o que já aconteceu nos meses fechados com as [metas](Goals.md) que você cadastrou e estima quanto você terá gasto até dezembro.

Para cadastrar ou editar metas, veja [Como cadastrar uma meta](ManageGoal.md). Visão geral do app: [WFinance](../WFinance.md).

---

## Em uma frase

Até o mês passado você gastou X. Se o resto do ano seguir o modelo escolhido, você fecha dezembro com Y. A meta do ano é Z.

---

## Como chegar

| Caminho                                               | Observação     |
|-------------------------------------------------------|----------------|
| Central → Planejamento → **Projeção anual das metas** | Única entrada. |

A tela não tem filtro de período. Ela sempre olha para o **ano corrente**, que aparece no topo.

---

## Meses fechados e meses restantes

- **Meses fechados** vão de janeiro até o mês **anterior** ao atual. São a base da projeção.
- **Meses restantes** vão do mês atual até dezembro.

O mês atual só entra na base quando fechar. Lançamentos com data no mês atual ou em meses futuros não entram no realizado.

Em **janeiro** nenhum mês fechou ainda. A tela mostra só o ano e avisa que não há dados suficientes para projetar. A partir de fevereiro, janeiro passa a ser a base.

Só contam despesas **efetivadas** ou **reconciliadas**. Lançamentos previstos ficam de fora. Estorno reduz o realizado, que pode até ficar negativo.

---

## O cabeçalho

O cabeçalho tem o seletor do modelo e dois blocos, os dois na **sua moeda**.

### Planejado

É a soma das linhas da lista. Responde: *o que eu planejei está indo para onde?*

| Campo              | O que é                                          |
|--------------------|--------------------------------------------------|
| Realizado          | Gasto dos meses fechados nas categorias da lista |
| Meta               | Meta dos meses fechados                          |
| Percentual         | Realizado ÷ meta                                 |
| Projetado          | Estimativa até dezembro, conforme o modelo       |
| Meta no ano        | Meta de janeiro a dezembro                       |
| Indicador circular | Projetado ÷ meta no ano                          |

Sem nenhuma meta no ano, a lista fica vazia e este bloco fica zerado.

### Não planejado

Tudo o que você gasta em categorias **sem meta**. Responde: *o que eu não planejei também consome dinheiro até o fim do ano.*

| Campo            | O que é                                |
|------------------|----------------------------------------|
| Realizado        | Gasto dos meses fechados fora da lista |
| Projeção até dez | Média mensal dos meses fechados × 12   |

Não tem meta nem percentual. A projeção deste bloco é **sempre** pela média, nos dois modelos: trocar o seletor não muda este número.

---

## A lista

Só aparecem categorias e subcategorias de **despesa** com meta no ano (anual ou de qualquer mês).

- **Categoria com meta**: uma linha da categoria. Ela inclui o gasto de todas as subcategorias. Metas das subcategorias não viram outra linha e não somam no limite.
- **Categoria sem meta**: uma linha para cada subcategoria que tem meta.
- **Categoria e subcategorias sem meta**: não aparecem. O gasto vai para o **não planejado**.

Exemplos:

- Alimentação tem meta de R$ 10.000 e Mercado, de R$ 4.000. A lista mostra só Alimentação, com meta de R$ 10.000. O gasto de Mercado entra em Alimentação.
- Veículo não tem meta. Combustível, IPVA e Manutenção têm. A lista mostra as três. Estacionamento, sem meta, vai para o não planejado, junto com lançamentos de Veículo sem subcategoria.

Lançamentos sem categoria não entram em nenhum dos dois blocos. Tocar numa linha não abre nada.

Cada linha mostra, para os meses fechados, o realizado, a meta e o percentual; e, até dezembro, o projetado, a meta do ano e o indicador circular. Cores: verde abaixo de 80%, laranja de 80% a 99%, vermelho de 100% em diante.

A meta de cada mês segue a mesma regra da tela de metas: 1/12 da meta anual mais a meta mensal daquele mês.

---

## Os dois modelos

A tela sempre abre no **Plano Futuro**. A escolha não fica gravada.

O modelo só muda a **projeção do bloco planejado**. Realizado, meta e o bloco não planejado não mudam.

### Plano Futuro

`projetado = realizado dos meses fechados + meta dos meses restantes`

Melhor para despesas **fixas ou previsíveis**: aluguel, condomínio, mensalidade. Um conserto em janeiro não é repetido pelo resto do ano: a meta cadastrada continua sendo a referência dos meses que faltam.

Uma meta anual continua valendo nos meses restantes: um IPVA anual pago todo em janeiro ainda soma as fatias de setembro a dezembro.

### Tendência

`projetado = realizado dos meses fechados + meta de cada mês restante × ritmo`

O **ritmo** é o realizado dividido pela meta dos meses fechados. Quem está 37% acima da meta até aqui vê os meses restantes 37% acima da meta.

Melhor para despesas **variáveis**: supermercado, lazer, delivery, combustível.

- A forma da meta se mantém: mês restante com meta zero continua zero. Um IPVA com meta só em janeiro não é espalhado pelos outros meses.
- Se o realizado for zero ou negativo, o ritmo é zero: a projeção fica igual ao realizado.
- Se não houver meta nos meses fechados, a linha usa a média mensal × 12.

---

## Cuidado com distorções

A Tendência **não tem limite**. Quanto maior a diferença entre o realizado e a meta nos meses fechados, maior o ritmo. Ela existe para mostrar o ritmo real, não para suavizá-lo.

Por isso, qualquer gasto pontual dos meses fechados — um conserto, um presente, uma viagem — é **espalhado pelo resto do ano, de propósito**. Não é defeito: é o que o modelo faz.

**Quanto menos meses fechados, maior o risco.** Em fevereiro, com só janeiro como base, um único gasto fora do comum pode dobrar a projeção. Com o passar dos meses, a base aumenta e o efeito diminui.

Se você não quer esse efeito, use o **Plano Futuro**. Ele ignora o ritmo real e repete a meta cadastrada nos meses restantes.

O aviso aparece também na tela, perto do seletor, e no **Como funciona a projeção?**.

---

## Moedas

- Cada linha usa a **moeda da meta**. Se o mesmo recorte tem metas em moedas diferentes (dado antigo), a linha usa a sua moeda e mostra um aviso, como na tela de metas.
- O cabeçalho converte cada linha para a **sua moeda** antes de somar.
- Meses fechados usam a taxa do **último dia do mês**. Meses restantes usam a **taxa mais recente** disponível.
- Se faltar taxa de câmbio, a tela **não calcula** e mostra o erro. Cadastre a taxa que falta e volte.

---

## Atualização

A tela se atualiza sozinha enquanto está aberta: ao criar, editar ou excluir uma meta do ano, ou ao lançar, editar ou excluir uma transação do ano.

---

## Se algo não bate

| Situação                                   | O que conferir                                                                                                             |
|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| “Não há dados suficientes”                 | É janeiro. A projeção começa em fevereiro.                                                                                 |
| Gasto deste mês não aparece                | O mês atual só entra na base quando fechar.                                                                                |
| Subcategoria com meta não aparece na lista | A categoria dela tem meta: o gasto está na linha da categoria.                                                             |
| Tendência muito alta no começo do ano      | Poucos meses fechados e algum gasto pontual. Veja [Cuidado com distorções](#cuidado-com-distorções) ou use o Plano Futuro. |
| Não planejado não muda com o seletor       | É esperado: esse bloco é sempre pela média.                                                                                |
| Erro de taxa de câmbio                     | Falta taxa para uma das moedas das metas ou das transações.                                                                |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
