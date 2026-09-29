# Reservas para objetivos

Uma **reserva** é uma caixinha com propósito: viagem, troca de carro, fundo de emergência. Você associa contas que já existem; o app soma os saldos e mostra quanto já está separado para aquele objetivo.

Esta página explica a lista, o que o total representa e os detalhes. Para criar ou editar, veja [Como cadastrar uma reserva](ManageReserve.md). Visão geral do app: [WFinance](../WFinance.md).

---

## Em uma frase

A reserva responde: **“quanto eu já tenho separado para este objetivo?”**

Ela **não cria transação**, **não altera saldo** e **não move dinheiro** entre contas. O valor continua onde estava. Para limitar gasto por categoria, use [metas](../Goals/Goals.md).

---

## Como chegar

| Caminho | Observação |
|---------|------------|
| Central → Planejamento → Reservas | A tela completa. |
| Painel inicial → **Ir para reservas** | O card da home lista só as que estão em andamento. |

É preciso ter pelo menos uma **conta bancária**, **carteira** ou **investimento**. Cartão de crédito **não entra** em reserva.

---

## O que você cadastra

Cada reserva tem:

- um **nome** (único no espaço);
- **ícone** e **cor**;
- uma ou mais **contas** associadas;
- **valor alvo** e **data alvo**, se quiser acompanhar progresso (os dois são opcionais);
- a **moeda** em que o total e o alvo aparecem.

O dinheiro não muda de lugar quando você associa a conta. Se a corrente tem R$ 5.000 e o fundo tem R$ 10.000, e as duas entram na reserva “Viagem”, a reserva mostra R$ 15.000 — e as contas continuam com os mesmos saldos.

Uma conta pertence a **no máximo uma** reserva. Se ela já está em “Trocar de carro”, não dá para colocá-la também em “Viagem”.

---

## A tela

A lista abre nas reservas **em andamento**.

![Lista de reservas em andamento](Reservas%20-%20tela%20inicial.png)

De cima para baixo:

- o link **Como funcionam as reservas?**, se a ajuda contextual estiver ligada;
- as abas **Em andamento** e **Concluídas**;
- um **card por reserva**.

No card, como no exemplo “Trocar de carro”:

| Campo | Significado |
|-------|-------------|
| Nome e ícone | O objetivo. |
| **Meta: 20/11/2026** | Data alvo, se você cadastrou. |
| Valor grande (verde) | Total da reserva **hoje**. |
| Valor menor | Valor alvo, se houver. |
| **Progresso** | Total dividido pelo alvo. Só aparece quando existe valor alvo. |

O botão **+** cria uma reserva nova. O passo a passo está em [Como cadastrar uma reserva](ManageReserve.md).

Deslize o card para o lado para **editar**, **concluir** ou **excluir** — as mesmas ações da ficha de detalhes. Quem está no espaço só para visualizar vê a lista, sem esses gestos e sem o +.

Na aba **Concluídas**, o empty state diz “Nenhuma reserva concluída” quando a lista está vazia. Concluir **não apaga** a reserva: ela some de “Em andamento” e passa para a outra aba, com as contas ainda associadas.

---

## De onde vem o total

O total é a **soma dos saldos atuais** das contas associadas, convertidos para a moeda da reserva.

| Tipo de conta | Que saldo entra |
|---------------|-----------------|
| Bancária ou carteira | O saldo **de hoje** (só lançamentos efetivados ou reconciliados). Previstos não entram. |
| Investimento | O saldo da **última avaliação**. |

A conversão usa a taxa **do dia**. Se uma conta está em outra moeda, o app converte para a moeda da reserva. Sem taxa cadastrada, o cálculo pode falhar — no [painel inicial](../MainDashboard.md#reservas) aparece um aviso no total.

O progresso para em **100%** na barra, mesmo que o saldo já tenha passado do alvo. Sem valor alvo, não há barra.

---

## Detalhes da reserva

Toque no card.

![Detalhes da reserva, com total, alvo e contas associadas](Reservas%20-%20detalhes.png)

No topo, três ícones:

| Ícone | Ação |
|-------|------|
| Lápis | Edita nome, contas, alvo… |
| Caixa | **Conclui** (ou restaura, se já estiver concluída). |
| Lixeira | **Exclui** a reserva. O dinheiro **permanece** nas contas. |

Abaixo: nome, notas (se houver), **total da reserva**, **valor alvo**, **data alvo** e a barra de progresso.

**Contas associadas** lista cada conta com o saldo dela. Se a moeda da conta for diferente da moeda da reserva, aparecem os dois valores: o original e o convertido.

Pela **home**, essa ficha abre **sem** os três ícones: o painel só consulta.

---

## Concluir ou excluir

São coisas diferentes.

**Concluir** — o objetivo chegou (ou você desistiu de acompanhá-lo no dia a dia). A reserva vai para **Concluídas**. As contas continuam ligadas; o total ainda entra no “total reservado” da home. Dá para restaurar e voltar para **Em andamento**.

**Excluir** — a caixinha some. As contas ficam livres para entrar em outra reserva. Nada é lançado e nenhum saldo muda.

As duas ações pedem confirmação.

---

## No painel inicial

O card de reservas da [home](../MainDashboard.md#reservas) lista só as **em andamento**: nome, data alvo, valor juntado e barra.

No topo, na sua **moeda padrão**:

- **Total reservado** — soma de **todas** as reservas, em andamento e concluídas.
- **Objetivos concluídos** — no formato “2 de 5”.

Cada linha da lista aparece na **moeda daquela reserva**, que pode ser outra. Por isso o total de cima e os valores das linhas nem sempre “fecham” à vista — um está na sua moeda, o outro na moeda do objetivo.

Toque na reserva para o detalhe. **Ir para reservas** abre esta tela. Com os valores ocultos pelo olho, o toque no item fica desativado.

---

## Plano e espaço

No **Free**, o teto é de **1 reserva por espaço**. O Premium remove esse limite — veja [Conta de usuário](../UserAccount.md).

Cada espaço tem as suas reservas. Trocar de espaço na [conta](../UserAccount.md) troca a lista junto.

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| O saldo da conta não mudou depois de criar a reserva | É esperado. Reserva não transfere dinheiro. |
| Não consigo associar uma conta | Ela já está em outra reserva, ou é cartão de crédito. |
| Total diferente da soma que eu faço de cabeça | Contas em outra moeda são convertidas pela taxa de hoje. No painel, o total de cima usa a sua moeda padrão. |
| Aviso no total da home | Falta taxa de câmbio para converter alguma conta. Cadastre a taxa em Moedas. |
| Progresso não aparece | Cadastre um valor alvo. Só a data não gera barra. |
| Reserva sumiu da lista | Veja a aba **Concluídas**. |
| Número menor que o do banco | Só entra o saldo atual (efetivado/reconciliado). Previstos não contam. No investimento, vale a última avaliação. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
