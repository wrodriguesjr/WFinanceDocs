# Como cadastrar uma conta de investimento

Uma **conta de investimento** é o cadastro de uma aplicação que você quer acompanhar: um CDB, a poupança, um fundo, um conjunto de ações, o FGTS. Ela guarda o histórico de aportes, resgates e avaliações de saldo. Os números da tela de investimentos saem desse histórico.

Os outros guias estão em [Investimentos](Investments.md). O que a tela mostra está em [A tela de investimentos](InvestmentScreen.md). A rentabilidade está em [Como a rentabilidade é calculada](Profitability.md). Visão geral do app: [WFinance](../WFinance.md).

---

## Em uma frase

A conta de investimento responde: **“este pedaço do meu patrimônio, quanto eu coloquei e quanto ele rendeu?”**

Ela não é uma conta corrente. Receita e despesa do dia a dia não caem aqui. O dinheiro entra por **aplicação** (sai da conta bancária associada) ou por **aporte direto**, e sai por **resgate** (volta para essa mesma conta bancária). O rendimento entra quando você **avalia o saldo**.

Uma conta é uma posição que você escolhe seguir. Dois CDBs em bancos diferentes são duas contas. Na corretora, você pode ter uma conta só (e avaliar o saldo total) ou separar ações, FIIs e tesouro em contas diferentes, se quiser a rentabilidade de cada um. O tipo (CDB, ação, fundo) organiza filtros e relatórios; **não muda a fórmula**.

---

## Como chegar

| Ação | De onde |
|------|---------|
| **Criar** | Central → **Estrutura financeira** → **Investimentos** → botão **+**. A tela se chama **Minhas contas**, já na aba Investimentos. |
| **Abrir a lista** | O mesmo caminho. No topo dá para alternar **Bancos**, **Carteiras**, **Investimentos** e **Cartões**. |
| **Editar** | Toque na conta → lápis. Ou deslize o card para editar. |
| **Ver os lançamentos** | Toque na conta → **Ver transações da conta**. Na [tela de investimentos](InvestmentScreen.md), o toque no card abre o mesmo extrato. |

Quem está no espaço só para visualizar vê a lista, sem **+**, sem deslizar e sem gravar o formulário.

Se você sair sem gravar, o app pergunta se quer descartar.

---

## A lista

A lista abre nas contas **ativas**. A outra aba é **Inativas**.

Em cada linha: logo, nome, tipo e o saldo. Toque na linha para a ficha:

- **Ver transações da conta**, no mês que está indicado;
- **conta vinculada** (o banco associado);
- **saldo total**, **total investido** e **rendimentos** (com o percentual);
- tags e o selo de ativa ou inativa.

No topo da ficha: editar, arquivar (ou reativar) e excluir. As mesmas ações estão no deslize do card.

---

## O que esta tela pede

O título é **Criar conta de investimento** ou **Editar conta de investimento**.

### Dados da conta

**Nome** — até 40 caracteres. Único neste espaço. “Tesouro Selic” e “CDB do banco” convivem; dois com o mesmo nome, não.

**Logo** — obrigatório. Toque em **Selecione o logo** e escolha o da instituição.

### Tipo de investimento

Dois campos, nessa ordem:

1. **Grupo** — a família (renda fixa, fundos, cripto…).
2. **Tipo** — o produto dentro do grupo. A lista de tipos muda quando o grupo muda.

O grupo **Liquidez restrita** (FGTS e previdência privada) usa o mesmo cálculo das outras contas. No relatório de patrimônio, essas contas aparecem em **Investimentos restritos**. No fluxo de caixa, o filtro **Considerar investimentos restritos no fluxo** decide se a aplicação e o resgate delas entram na conta.

| Grupo | Tipos |
|-------|--------|
| Renda fixa — governo | Tesouro Direto |
| Renda fixa — crédito privado | CDB, LCI/LCA, Letra de Câmbio, Letra Financeira, Debêntures, Debêntures incentivadas, CRI, CRA, FIDC |
| Renda variável | Ações, BDRs, ETFs, Fundos imobiliários (FIIs) |
| Fundos | Fundos de investimento |
| Estruturados e derivativos | COE, Derivativos |
| Alternativos | Ouro e metais, Câmbio, Empréstimo P2P, Crowdfunding |
| Cripto | Criptomoedas |
| Caixa e equivalentes | Poupança, Conta remunerada |
| Liquidez restrita | Previdência privada, FGTS |

Dá para trocar grupo e tipo depois, mesmo com lançamentos. Isso só reclassifica a conta.

### Saldo inicial

Só na **criação**.

**Valor inicial** — quanto a conta já vale no dia em que você começa a acompanhá-la. Pode ser zero: a conta nasce vazia e o primeiro dinheiro entra por uma aplicação.

Se o valor for maior que zero, o app grava um lançamento de **saldo inicial** na data que você escolher. Esse valor entra inteiro no **investido**. O resultado começa em zero, até a primeira avaliação que mostre um saldo diferente.

**Data do lançamento** — o dia desse saldo. O padrão é hoje.

Na edição, este bloco some. Para corrigir a abertura, edite o lançamento de saldo inicial no extrato.

### Moeda

A moeda da conta. Na criação, o padrão é o real, entre as moedas que você marcou no perfil.

Aplicações, resgates, avaliações e os números do extrato ficam nessa moeda. Na [tela de investimentos](InvestmentScreen.md#moeda), os totais são convertidos para a moeda padrão do perfil.

Depois do primeiro lançamento, a moeda fica travada. O campo avisa: “Não é possível mudar a moeda de uma conta que possui lançamentos”.

### Conta bancária associada

Obrigatória. É de lá que saem as aplicações e para lá que voltam os resgates. O app só conclui a transferência se a conta bancária for **esta**.

Toque na linha para escolher uma conta que já existe, ou em **Adicionar nova conta** para cadastrar o banco na hora.

Cartão de crédito e carteira não entram aqui: a associada é uma **conta bancária**.

Depois do primeiro lançamento, a conta associada também fica travada. Se a conta ainda não tem nenhum lançamento, dá para trocar a moeda e o banco.

### Tags

Opcional. Digite e escolha uma tag já usada em contas de investimento, ou crie uma nova na hora. Toque no x do chip para tirar.

As tags aparecem no card expandido da [tela de investimentos](InvestmentScreen.md) e servem de filtro lá. Uma conta pode ter várias. No filtro, ela entra se tiver **qualquer uma** das tags selecionadas.

### Conta ativa

O interruptor começa ligado. Desligar arquiva: a conta sai da aba **Ativas** e deixa de aparecer quando você escolhe uma conta para um lançamento novo. O histórico permanece. Com **Considerar contas inativas** ligado na tela de investimentos, ela ainda entra nos totais.

---

## Depois de salvar

A lista atualiza sozinha. Com saldo inicial maior que zero, o extrato já mostra esse lançamento na data escolhida.

O próximo passo, para a rentabilidade existir, é abrir o extrato e usar **Avaliar**. O ideal é repetir isso ao menos uma vez por mês. Sem essa avaliação, a [tela de investimentos](InvestmentScreen.md) mostra resultado zero e o ícone de aviso — o saldo inicial não conta como avaliação. O passo a passo da folha está em [Atualizar o saldo](UpdateBalance.md).

Para colocar dinheiro novo que sai do banco, use **Aplicar**. Para tirar, **Resgatar**. Para um valor que não passa por outra conta do app, use **Outros** → aporte. IOF e IR também ficam em **Outros**.

---

## Arquivar ou excluir

São coisas diferentes. As duas pedem confirmação.

**Arquivar** — a conta vai para **Inativas**. Lançamentos, saldo e rentabilidade continuam disponíveis quando o relatório inclui inativas. Dá para reativar.

**Excluir** — a conta some. Se já existem lançamentos, o app avisa que eles serão apagados junto e sugere arquivar. A exclusão não volta atrás.

Arquivar pela ficha, pelo deslize ou pelo interruptor **Conta ativa** mexe na mesma situação: ativa ou inativa.

---

## O que o app não deixa gravar

| Recado | Por quê |
|--------|---------|
| Selecione um logo para a conta de investimento | O logo identifica a instituição na lista. |
| Selecione uma conta bancária antes de salvar | Aplicação e resgate precisam de um banco associado. |
| Insira um nome para a conta | O nome é obrigatório. |
| Já existe uma conta com esse nome | O nome é único no espaço. |
| Não é possível mudar a moeda de uma conta que possui lançamentos | A moeda dos lançamentos já gravados ficaria inconsistente. |
| Você não tem permissão para editar contas de investimento neste grupo | Papel de somente leitura neste espaço. |

No plano **Free** há limite de **2 contas de investimento por espaço**. Conta inativa continua na conta do limite. O Premium remove esse teto — veja [Conta de usuário](../UserAccount.md).

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
