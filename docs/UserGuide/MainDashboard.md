# Painel inicial

O **painel inicial** é a tela que abre depois do login. É um resumo do espaço ativo: o mês corrente, as contas, os cartões, as metas e as reservas — sem precisar entrar em cada lista.

Visão geral do app: [WFinance](WFinance.md). Conceitos de lançamento: [Transações](Transactions/Transactions.md). Perfil e espaços: [Conta de usuário](UserAccount.md).

---

## Em uma frase

Você olha o mês, decide o que merece atenção e toca no card para ir ao detalhe.

Nada é lançado aqui. O painel **mostra**. Para registrar uma movimentação, use o botão **+** na barra inferior.

---

## Primeira vez no app

Sem conta, sem categoria e sem lançamento, a tela fica assim: um aviso do que ainda falta e o atalho para personalizar o painel.

![Tela inicial vazia, no primeiro acesso](Screenshots/Tela%20inicial%20-%20vazia.png)

O card **O WFinance ainda não está pronto** lista o que é necessário para o app funcionar de verdade. Toque nele para ir ao checklist.

| Chip           | Por que aparece                                              | O que fazer                                                                                                  |
|----------------|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| **Conta**      | Não há conta bancária, carteira nem cartão no espaço.        | Cadastre pelo menos uma.                                                                                     |
| **Categoria**  | Não há categorias. Receita e despesa exigem classificação.   | Crie as suas ou use as categorias padrão do app.                                                             |
| **Permissões** | Notificações do app ou leitura de avisos de banco ainda não. | Opcional. Ajuda na [captura automática](Transactions/Transactions.md#captura-automática-notificações-e-sms). |

Conta e categoria são **obrigatórias**. Sem elas o resumo financeiro não aparece. Permissões são **recomendadas**; dá para adiar por 30 dias.

O card de baixo (**Quer configurar a sua tela inicial?**) abre as configurações do painel. Use quando quiser escolher quais blocos ver.

Quem está no espaço só para visualizar (permissão **somente leitura**) não vê esses avisos nem o resumo financeiro.

---

## Com dados

Depois de cadastrar contas e categorias, o painel passa a mostrar os cards que tiverem conteúdo. No exemplo abaixo, o mês está em **Fluxo de caixa** e as contas bancárias já têm saldo.

![Painel inicial com fluxo de caixa e contas bancárias](Screenshots/Tela%20inicial%20-%2001.png)

Só aparece o que existe **e** o que você marcou para exibir. Conta sem “mostrar na tela inicial”, meta inexistente no mês ou reserva inativa não ocupam espaço.

A ordem na tela é sempre a mesma:

1. Avisos (configuração pendente, capturas para importar, sincronização)
2. Resumo financeiro do mês
3. Contas bancárias
4. Carteiras
5. Cartões de crédito
6. Metas
7. Reservas
8. Atalho para configurar o painel

---

## Barra superior

- **Foto e nome** — abrem o [perfil](UserAccount.md#a-tela-editar-perfil). Lá você troca o **espaço ativo**. Tudo no painel é daquele espaço.
- **Ícone de olho** — esconde ou mostra os valores em todos os cards. Os números viram um placeholder; o restante da tela continua visível. Útil no ônibus ou na fila do banco.

Puxe a tela para baixo para atualizar saldos, faturas e totais.

No Premium, na primeira vez neste aparelho, um aviso no topo mostra o andamento da sincronização com a nuvem. Os cards vão preenchendo conforme os dados chegam.

---

## Avisos no topo

Além do checklist do primeiro uso, pode aparecer:

**Transações aguardando importação** — o app captou notificações ou SMS e ainda não virou lançamento. Toque para revisar e importar. Enquanto não confirmar, o valor **não entra** em saldo nem no resumo. Detalhes em [Captura automática](Transactions/Transactions.md#captura-automática-notificações-e-sms).

Esses avisos somem sozinhos quando não há mais o que fazer.

---

## Resumo financeiro

É o card do **mês corrente**, na sua moeda padrão. Só aparece se o espaço tiver pelo menos uma conta **e** categorias, e se você puder editar o espaço.

Há duas visões. A escolha fica gravada até você trocar.

| Visão              | O que conta                                      | Resultado                         | Quando usar                                      |
|--------------------|--------------------------------------------------|-----------------------------------|--------------------------------------------------|
| **Resultado**      | Receitas e despesas na **data do lançamento**.   | **Lucro** ou **Prejuízo**         | Entender o padrão de gasto e de renda do mês.    |
| **Fluxo de caixa** | Entradas e saídas quando o **dinheiro se move**. | **Superávit** ou **Déficit**      | Ver se o caixa do mês sobrou ou faltou.          |

A diferença mais comum: compra no cartão em março entra no **Resultado** de março; o pagamento da fatura em abril entra no **Fluxo de caixa** de abril.

O interruptor **Considerar previstas** vale para as duas visões:

- **Ligado** — inclui lançamentos ainda [previstos](Transactions/Transactions.md#status-previsto-efetivado-e-reconciliado) (salário que vai cair, conta que ainda não venceu).
- **Desligado** — só o que já foi efetivado ou reconciliado.

Toque nos valores para abrir o relatório correspondente (por categoria no Resultado, fluxo de caixa na outra visão), já com o mesmo critério de previstas.

Se a ajuda contextual estiver ligada, o link **O que é Resultado?** / **O que é visão de Fluxo de Caixa?** explica isso de novo dentro do app.

---

## Contas bancárias

Mostra as contas **ativas** marcadas para aparecer no painel.

No topo:

- **Saldo atual** — posição **hoje**, na sua moeda padrão.
- **Saldo futuro** — o que a conta tende a ter depois dos lançamentos futuros **já efetivados ou reconciliados**. A seta indica se o futuro está maior ou menor que o de hoje.

Previstos **não entram** nesses dois saldos. Para vê-los no mês, use **Considerar previstas** no resumo financeiro.

Em cada linha: nome, instituição, saldo atual e saldo futuro **na moeda da conta**. Toque na conta para abrir o extrato. O botão **Ir para contas bancárias** abre a lista completa, inclusive as que você ocultou daqui.

Se uma conta não aparece, confira se está ativa e com a opção de mostrar saldo na tela inicial.

---

## Carteiras

Mesma lógica das contas bancárias, para o dinheiro em espécie: saldo atual, saldo futuro, totais na sua moeda padrão.

Toque na carteira para o extrato. **Ir para carteiras** abre a lista de cadastro.

---

## Cartões de crédito

Para cada cartão, o painel destaca a fatura que importa **agora** no ciclo — em geral a atual e, se você pediu duas linhas, a anterior, a fechada ou a próxima.

Em cada fatura você vê:

- rótulo (atual, anterior, fechada, próxima);
- status (aberta, fechada, vencida, paga, sem movimento…);
- data de fechamento, vencimento ou pagamento;
- valor.

Toque na fatura para abrir as compras daquele ciclo.

Totais no topo do card, na sua moeda padrão:

| Total            | O que soma                                              |
|------------------|---------------------------------------------------------|
| **Vencido**      | Faturas vencidas e ainda não pagas.                     |
| **A vencer**     | Faturas abertas ou fechadas que ainda vão vencer.       |

Faturas já pagas e faturas futuras demais **não entram** nesses totais.

Nas configurações do painel você escolhe **uma ou duas faturas** por cartão. **Ir para cartões de crédito** abre a lista de cartões.

---

## Metas

Aparece quando há meta com progresso no **mês corrente**. Não lista todas: mostra as **três** com maior desvio, misturando percentual atingido e valor estourado. Meta anual entra pelo equivalente daquele mês.

No topo:

- **Maior desvio percentual** — a meta mais perto (ou além) do teto, em %.
- **Maior estouro em valor** — quanto passou do limite, na sua moeda padrão.

Toque numa meta para ver o detalhe. **Ir para metas** abre o acompanhamento completo (mês, trimestre ou ano).

Metas usam só transações **efetivadas** e **reconciliadas**.

---

## Reservas

Reservas são o dinheiro que você **separa para um objetivo** (viagem, entrada do imóvel, fundo de emergência). Elas **não mudam o saldo** das contas: só marcam quanto já está destinado.

O card lista as reservas **em andamento**: nome, data alvo (se houver), valor juntado e barra de progresso.

No topo:

- **Total reservado** — soma de **todas** as reservas (em andamento e concluídas), na sua moeda padrão.
- **Objetivos concluídos** — quantas já chegaram lá, no formato “2 de 5”.

Toque na reserva para o detalhe. **Ir para reservas** abre a tela completa. Com os valores ocultos pelo olho, o toque no item fica desativado.

---

## Personalizar o painel

Os seis cards (resumo, reservas, metas, contas, carteiras, cartões) podem ser ligados ou desligados.

Caminhos:

- o card **Quer configurar a sua tela inicial?**, no fim da página; ou
- o ícone da **Central** na barra inferior → configurações da tela inicial.

Lá você também define se cada cartão mostra uma ou duas faturas e se os textos de ajuda (**O que é…**) aparecem nos cards.

Desligar um card **não apaga dados**. Só tira aquele bloco da home.

---

## Barra inferior

O ícone de **casa** é este painel. Os outros atalhos levam a extratos, faturas, novo lançamento, investimentos, metas e à Central do app.

O **+** é o caminho mais rápido para [lançar uma transação](Transactions/ManageTransaction.md).

---

## Se algo não bate

| Situação                                         | O que conferir                                                                                          |
|--------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| Painel quase vazio depois do cadastro            | Falta categoria, ou o card está desligado nas configurações.                                            |
| Conta existe, mas não está na lista              | Precisa estar ativa e marcada para mostrar saldo na tela inicial.                                       |
| Números diferentes do banco                      | Saldos do painel ignoram previstos. Confira o status dos lançamentos.                                   |
| Resultado e fluxo de caixa não coincidem         | É esperado. Um olha a data da compra; o outro, a data em que o dinheiro saiu ou entrou.                 |
| Valores em `••••`                                | O olho da barra superior está ocultando os números. Toque de novo para revelar.                         |
| Ícone de alerta no total                         | Falta taxa de câmbio entre a moeda da conta e a sua moeda padrão. Cadastre a taxa em Moedas.            |
| Troquei de espaço e os números mudaram           | O painel é sempre do espaço ativo. Toque no nome, no topo, para conferir.                               |
| Capturas no aviso, mas o saldo não mudou         | Importar ainda não aconteceu. O rascunho não conta até você confirmar.                                  |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
