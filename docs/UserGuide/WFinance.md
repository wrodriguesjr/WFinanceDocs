# WFinance

**Seu controle financeiro, do seu jeito.**

O WFinance é um aplicativo Android para organizar o dinheiro do dia a dia: receitas, despesas, transferências, cartões, investimentos e metas. Você decide se usa sozinho, com a família ou com um sócio — e o app continua funcionando mesmo sem internet.

Disponível na [Google Play](https://play.google.com/store/apps/details?id=com.wrj.wfinance).

Esta página apresenta o que o WFinance oferece. Para detalhes de uso, veja também:

- [Painel inicial](MainDashboard.md)
- [Transações](Transactions/Transactions.md)
- [Investimentos](Investments/Investments.md)
- [Captura de notificações bancárias](Capture/Capture.md)
- [Metas de gastos](Goals/Goals.md)
- [Reservas para objetivos](Reserves/Reserves.md)
- [Conta e espaços](AccountAndSpaces.md)
- [Termos de Uso](TermsOfUse.md)
- [Política de Privacidade](PrivacyPolice.md)

---

## Para quem é

O WFinance serve bem em situações como:

- **Uso pessoal** — acompanhar o próprio orçamento, contas e cartões.
- **Finanças da casa** — casal ou família registrando gastos no mesmo espaço, em tempo real.
- **Pequeno negócio** — sócios compartilhando o controle; o contador pode entrar só para visualizar.
- **Gestão delegada** — alguém cuida das contas de um familiar, com transparência para quem acompanha.
- **Vários aparelhos** — o mesmo espaço no celular, no tablet ou no aparelho do trabalho, sempre atualizado.

---


## O que você consegue fazer

### Painel inicial

A tela que abre depois do login reúne o mês corrente, contas, cartões, metas e reservas. Cards sem dado somem sozinhos; você escolhe quais blocos ver.

Leia o guia em [Painel inicial](MainDashboard.md).

### Transações

Registre **receitas**, **despesas** e **transferências** em contas bancárias, carteiras, cartões de crédito e investimentos.

Classifique por categoria, subcategoria e tags. Dá para parcelar, criar recorrência (salário, aluguel, assinaturas) e lançar valores em outra moeda.

Cada lançamento tem um status:

| Status           | Significado                                         |
|------------------|-----------------------------------------------------|
| **Previsto**     | Planejado. Ainda não entra no saldo real.           |
| **Efetivado**    | Já aconteceu. Entra no saldo e nos relatórios.      |
| **Reconciliado** | Conferido com extrato bancário ou fatura importada. |

O app também pode **captar lançamentos automaticamente** a partir de notificações e SMS de bancos — você só revisa e confirma.

Leia o guia em [Transações](Transactions/Transactions.md). O formulário, o estorno, o status, as listas e a conversão de moeda estão ligados a partir dessa página. A captura está em [Captura de notificações bancárias](Capture/Capture.md).

### Espaços

Todo mundo começa com um **espaço pessoal**, privado e criado automaticamente.

Depois, no plano com sincronização, você pode criar **espaços compartilhados**, convidar pessoas por um código e controlar juntos contas, cartões, transações, metas e relatórios.

Há quatro níveis de permissão:

| Nível               | O que pode                                              |
|---------------------|---------------------------------------------------------|
| **Proprietário**    | Controle total. Não sai do espaço (só pode encerrá-lo). |
| **Administrador**   | Gerencia membros e convites.                            |
| **Membro**          | Usa os dados financeiros normalmente.                   |
| **Somente leitura** | Só visualiza, sem alterar nada.                         |

Para criar ou participar de espaços compartilhados é necessário um plano com sincronização na nuvem.

Leia o guia em [Espaços](Spaces.md). Conta, perfil, bloqueio do app e exclusão: [Conta de usuário](UserAccount.md).

### Investimentos

Cada aplicação que você quer acompanhar (poupança, CDB, fundo, ação, tesouro) é uma **conta de investimento**, ligada à conta bancária de onde saem os aportes e para onde voltam os resgates.

De tempos em tempos você informa o saldo que a instituição está mostrando. O app separa esse saldo em duas partes que ainda estão na conta: o **investido** (o capital) e o **resultado** (o ganho ou a perda). Um resgate leva um pedaço de cada uma, na mesma proporção.

A tela de investimentos mostra o mês, o saldo da carteira, a rentabilidade e a evolução dos últimos 12 meses. Sem uma avaliação de saldo recente, aparece um aviso.

Leia o guia em [Investimentos](Investments/Investments.md). O cadastro, a tela, a atualização de saldo e o cálculo da rentabilidade estão ligados a partir dessa página.

### Metas

Defina um teto de gasto por categoria ou subcategoria, no mês ou no ano. O progresso usa só transações **efetivadas** e **reconciliadas**.

Na lista, cada categoria vira um **card**. Meta anual e metas mensais do mesmo recorte **somam** nesse card. Você escolhe olhar o **acumulado no ano** (janeiro até o mês escolhido), o **mês**, o **trimestre** ou o **ano inteiro**.

Todo o período do filtro conta no atingido — inclusive meses em que você não cadastrou limite. O app avisa quando uma meta chega a **80%** e a **100%**.

Leia o guia em [Metas de gastos](Goals/Goals.md). A lista, o cadastro e a projeção até dezembro estão ligados a partir dessa página.

### Reservas

Separe o dinheiro que já está nas contas para um **objetivo**: viagem, troca de carro, emergência. A reserva **não move saldo** e **não cria lançamento** — só soma as contas que você associar.

Uma conta entra em **no máximo uma** reserva. Cartão de crédito não entra. Valor alvo e data são opcionais; com alvo, o app mostra o progresso.

Leia o guia em [Reservas para objetivos](Reserves/Reserves.md). A lista e o cadastro estão ligados a partir dessa página.

### Várias moedas

Cada conta e cada cartão pode ter a **própria moeda**. Uma compra em dólar numa conta em reais é convertida com a taxa do dia.

Isso vale também para transferências entre contas de moedas diferentes — útil para quem usa Wise, Nomad ou tem conta no exterior. O exemplo de uma compra em dólar está em [Conversão de moeda](Transactions/CurrencyConversion.md).

Você pode cadastrar taxas diárias (ficam guardadas por 12 meses) e o app monta médias mensais para períodos mais antigos. Em Configurações → Moedas, escolha as moedas que usa com mais frequência para a lista ficar mais curta na hora de lançar.

### Sincronização e uso offline

O WFinance funciona **primeiro no aparelho**: você registra, edita e consulta sem internet.

No plano Premium, as alterações sobem para a nuvem em poucos segundos e chegam aos outros aparelhos e às outras pessoas do espaço. Se duas pessoas editarem a mesma coisa ao mesmo tempo, vale a **última alteração** que chegou à nuvem.

Ao entrar com a mesma conta Google num aparelho novo (plano com sincronização), o app baixa seus dados automaticamente.

---

## Contas financeiras

Além das transações, o WFinance organiza o dinheiro em quatro tipos de conta:

| Tipo                  | Para que serve                                |
|-----------------------|-----------------------------------------------|
| **Conta bancária**    | Extrato com saldo diário, previsto e efetivo. |
| **Carteira**          | Dinheiro em espécie do dia a dia.             |
| **Cartão de crédito** | Faturas, compras, pagamento e importação.     |
| **Investimento**      | Aportes, resgates e avaliação de saldo.       |

---

## Relatórios

Os relatórios ajudam a enxergar o conjunto, não só o lançamento isolado:

- **Fluxo de caixa** — entradas e saídas do período.
- **Por categoria** — para onde o dinheiro foi.
- **Por tag** — recortes que você mesmo criou (viagem, obra, projeto).
- **Investimentos** — rentabilidade e evolução.
- **Patrimônio** — visão consolidada dos saldos.
- **Faturas e extratos** — histórico de cartões e importações bancárias.

Ao abrir as transações de um relatório, a lista fica restrita àqueles lançamentos — sem adicionar novos itens, só para análise.

---

## Planos

No primeiro acesso você entra no **WFinance Free**, com as funções essenciais e limites de cadastro. Quando precisar de mais espaço, de vários aparelhos ou de espaços compartilhados, assine o **WFinance Premium**.

|                               | Free     | Premium            |
|-------------------------------|----------|--------------------|
| Uso no aparelho, sem internet | Sim      | Sim                |
| Sincronização entre aparelhos | Não      | Sim                |
| Espaços compartilhados        | Não      | Sim                |
| Quantidade de cadastros       | Limitada | Sem limite prático |

Limites atuais do plano Free (por espaço):

- 120 transações
- 2 contas bancárias
- 2 contas de investimento
- 1 carteira
- 1 cartão de crédito
- 5 metas
- 1 reserva

Itens arquivados ou inativos **continuam contando** no limite. A assinatura é cobrada pela Google Play e pode ser cancelada nas configurações da loja.

Detalhes de login, recuperação, bloqueio do app e exclusão estão em [Conta de usuário](UserAccount.md).

---

## Privacidade

Seus dados financeiros ficam no aparelho. No Premium, também vão para a nuvem só para sincronizar entre os seus dispositivos e os membros dos seus espaços.

O WFinance **não vende, não aluga e não compartilha** seus dados para propaganda.

Os textos completos estão em [Política de Privacidade](PrivacyPolice.md) e [Termos de Uso](TermsOfUse.md) (também na tela **Sobre** do app). Também é possível excluir os dados ou a conta inteira — veja [Conta de usuário](UserAccount.md).

---

## Requisitos

- Celular ou tablet Android (Android 12 ou superior).
- Conta Google para criar o acesso e, no Premium, para sincronizar.
- Internet só quando quiser sincronizar, recuperar a conta em outro aparelho ou assinar.

---

## Contato

- **E-mail:** [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com)
- **Google Play:** [Baixar o WFinance](https://play.google.com/store/apps/details?id=com.wrj.wfinance)
- **Documentação:** [wfinance.app.br](https://wfinance.app.br/UserGuide/WFinance)

Atualizações do app saem na [Google Play](https://play.google.com/store/apps/details?id=com.wrj.wfinance). Na tela **Sobre**, toque na versão para conferir se já está na última.
