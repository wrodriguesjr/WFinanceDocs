# Captura de notificações bancárias

A **captura** lê os avisos que o banco, o cartão ou a carteira digital já mandam para o celular e transforma cada um em um rascunho de lançamento. Você confere e confirma. Só então o valor entra no espaço.

Visão geral do app: [WFinance](../WFinance.md). O que é um lançamento: [Transações](../Transactions/Transactions.md). O formulário de confirmação: [Como lançar uma transação](../Transactions/ManageTransaction.md). O aviso na home: [Painel inicial](../MainDashboard.md).

---

## Em uma frase

O banco avisa. O WFinance entende a mensagem, guarda um rascunho e espera você importar.

A captura funciona com o app fechado. Ela cobre compras, PIX, pagamentos, transferências e, em alguns aplicativos, a cotação do câmbio.

---

## Para que serve

- Você deixa de digitar o que o banco já escreveu: valor, data, estabelecimento e, quando a mensagem traz, o cartão.
- O saldo só muda depois da sua confirmação. Um aviso lido pela metade não vira lançamento.
- Na próxima vez em que a mesma descrição (ou o mesmo cartão) aparecer, o app sugere a conta e a categoria que você usou antes.
- Se uma mensagem de um banco conhecido não for entendida, ela fica guardada. Você pode pedir para a equipe WFinance passar a reconhecê-la.
- Com a opção de câmbio ligada, a cotação que o aplicativo enviar entra sozinha, junto com a taxa inversa.

---

## Como funciona

1. O banco, o cartão ou o SMS avisa no celular.
2. Se o WFinance reconhecer o texto, grava um **rascunho** e pode avisar você.
3. Você abre a lista, confere conta, categoria, valor e sinal, e grava.
4. O rascunho sai da lista. O lançamento passa a valer no espaço que estiver ativo.

Enquanto o rascunho espera, ele **não entra** em saldo, resumo, meta nem relatório.

O rascunho fica neste aparelho. Outro celular com a mesma conta não mostra a lista de capturas. Depois de importar, o lançamento segue as regras normais do espaço — no Premium, sincroniza com os outros aparelhos.

Se o banco avisar pelo aplicativo e também por SMS, o WFinance guarda **um** rascunho.

Quem está no espaço só para visualizar não vê o aviso da tela inicial nem abre esta lista.

---

## Como chegar

| Caminho | O que abre |
|---------|------------|
| Painel inicial → **Transações aguardando importação** | Aba **Capturadas**. |
| Central → **Importação** → **Importar notificações bancárias** | Aba **Capturadas**. O número ao lado é a quantidade de rascunhos. |
| Central → **Importação** → **Notificações não reconhecidas** | Aba **Não reconhecidas**. |
| Toque no aviso do WFinance (“nova compra detectada”, “PIX recebido”…) | O formulário daquele rascunho, direto. |
| Painel inicial → **Ajustes recomendados** → **Permissões** | A tela de configurações, para ligar a captura. |
| Ícone de engrenagem → **Configurações** | As permissões e a opção de câmbio. |

As duas abas ficam na mesma tela, **Importação de notificações**. O número entre parênteses em **Capturadas** é a quantidade de rascunhos. Em **Não reconhecidas**, é a quantidade que ainda não foi enviada para análise.

---

## O que ligar

A captura é opcional. Dá para lançar tudo à mão. Se quiser usá-la, três acessos fazem diferença. Eles ficam em **Configurações**, no bloco **Acesso do sistema**.

Se ainda faltar algum, o painel inicial mostra **Ajustes recomendados**, com o atalho **Permissões**. Toque para ir à mesma tela. Dá para adiar esse lembrete por 30 dias (**Lembrar depois**). Conta e categoria continuam obrigatórias para o app funcionar; a captura, não.

![Aviso de permissões na tela inicial](Notificacoes%20-%20Aviso%20de%20permissao.png)

![Opções de leitura, SMS, envio de avisos e bateria](Notificacoes%20-%20Configuracoes.png)

| Opção | Para que serve |
|-------|----------------|
| **Leitura de notificações** | Lê o aviso do aplicativo do banco, do cartão, da carteira ou do app de SMS. É o acesso principal. |
| **Leitura de SMS** | Lê a mensagem de texto direto, quando o banco avisa por SMS e o celular esconde o conteúdo na notificação. |
| **Envio de notificações** | Permite que o WFinance avise você quando capturar um lançamento (e também nos avisos de meta). |
| **Otimização de Bateria** | Explica, no seu modelo de celular, como evitar que o sistema pare a captura com o app fechado. |

Ao ligar o interruptor, o Android pede a permissão:

- **Leitura de notificações** abre a tela do sistema em que você autoriza o WFinance a acessar notificações. Procure o WFinance na lista e ative.
- **Leitura de SMS** e **Envio de notificações** pedem confirmação na hora.

Depois de concedida, a opção fica ligada. Para retirar o acesso, use as configurações do Android (aplicativos → WFinance, ou acesso às notificações).

**Saiba mais**, em cada linha, explica o que aquele acesso faz.

No aplicativo do banco, os avisos de compra, PIX e pagamento também precisam estar ligados. Sem o aviso do banco, não há o que capturar.

### Leitura de notificações e SMS

Na maior parte dos celulares, a **leitura de notificações** já alcança o aviso do app de mensagens (Mensagens do Google, Mensagens da Samsung e outros). Use a **leitura de SMS** quando o banco manda SMS e, mesmo com a leitura de notificações ligada, a compra não aparece.

Alguns aparelhos escondem o texto quando as **notificações aprimoradas** do Android estão ligadas. Se a captura falhar com as permissões já concedidas:

1. Abra as configurações do Android.
2. Vá em **Notificações** → **Notificações aprimoradas**.
3. Desligue essa opção.

O mesmo caminho está no **Saiba mais** da leitura de notificações.

### Bateria

Com o app fechado, alguns celulares encerram a captura depois de alguns minutos. Xiaomi, Redmi, POCO, Huawei, Honor, Oppo, Realme e OnePlus fazem isso com mais frequência. Samsung costuma ser mais brando.

Toque em **Otimização de Bateria**. O WFinance mostra o passo a passo do fabricante do seu aparelho. Os nomes dos menus mudam conforme a marca e a versão do sistema. Em geral, o caminho é deixar o WFinance **sem restrições** de bateria e, quando existir, permitir **inicialização automática** e execução em segundo plano.

O app não altera essa configuração sozinho. Se você preferir não mexer, os lançamentos continuam podendo ser feitos à mão.

Depois de reiniciar o celular, desbloqueie a tela uma vez. A captura volta a valer a partir daí.

---

## Aviso na tela inicial

Quando existe rascunho esperando, o painel mostra **Transações aguardando importação** e a quantidade.

![Alerta de transações capturadas na tela inicial](Notificacoes%20-%20Alerta%20na%20tela%20inicial.png)

Toque no aviso para abrir a lista. Ele some quando não houver mais rascunho, ou se você estiver num espaço só para visualizar.

Esse aviso fala das mensagens **já entendidas**. As que o app recebeu e não soube ler ficam na outra aba, sem card na home.

---

## Aviso do WFinance

Com o **envio de notificações** ligado, cada rascunho novo gera um aviso do próprio WFinance: compra, PIX, boleto, transferência, saque, depósito, tarifa ou pagamento de cartão.

O texto traz valor, descrição e, quando a mensagem tiver, cartão e local. **Toque para processar esta transação** abre o formulário daquele item.

Se o envio estiver desligado, o rascunho continua na lista e no aviso da tela inicial. Só deixa de aparecer na barra de notificações do Android.

Uma mensagem repetida não gera um segundo aviso.

---

## Transações capturadas

A aba **Capturadas** lista o que já foi entendido e ainda não virou lançamento.

![Lista de notificações capturadas aguardando importação](Notificacoes%20-%20Lista%20notificacoes%20capturadas.png)

Em cada card:

- a descrição (em geral o estabelecimento ou a pessoa);
- a data;
- o cartão, quando a mensagem informa;
- o tipo (Compra, Pix enviado, Pix recebido, pagamento, transferência, saque, depósito, tarifa e outros);
- o valor, com o sinal. Saída aparece na cor de despesa. Entrada (PIX recebido, depósito, recompensa) aparece na cor de receita.

Toque no card para importar.

Deslize para a **direita**:

- **importar** — abre o formulário;
- **reprocessar** — lê a mensagem de novo. Use quando o texto foi entendido pela metade e o app já tiver aprendido o formato certo;
- **ver a mensagem** — mostra o título e o texto originais.

Deslize para a **esquerda** para excluir aquele rascunho.

**Excluir tudo** apaga a lista inteira, depois de uma confirmação. Isso não apaga lançamentos que você já importou.

Se a lista estiver vazia, a tela diz que não há notificação disponível.

O link **Como funciona a importação de transações?** (quando a ajuda contextual está ligada) explica a tela e lista as fontes que o app reconhece no momento, com atalho para o aplicativo na Play Store.

### Confirmar o lançamento

O formulário abre preenchido com descrição, valor, data, moeda e o tipo (despesa ou receita). O sinal já vem coerente com a mensagem: compra e PIX enviado saem; PIX recebido, depósito e recompensa entram. Estorno vem com o sinal invertido — confira se o dinheiro voltou.

Conta e categoria precisam da sua confirmação. Se você já lançou aquela descrição, ou se o nome do cartão já foi associado a uma conta, o app traz a sugestão. Ajuste o que estiver diferente e grave.

O passo a passo dos campos está em [Como lançar uma transação](../Transactions/ManageTransaction.md#importar-de-notificação).

Antes de abrir o formulário, e de novo ao gravar, pode aparecer **Possível duplicidade**: já existe um lançamento com o **mesmo valor e o mesmo sinal** na mesma data ou um dia antes ou depois. O aviso mostra a descrição, o valor, a data e a conta. **Criar transação** segue em frente. Voltar deixa o rascunho onde está.

Despesa e receita do mesmo valor não se misturam. Estorno também não conta como duplicata da compra original.

Ao gravar, o rascunho é apagado para não ser importado outra vez. Quem está logado neste aparelho é quem fica com o lançamento, no espaço ativo.

---

## Notificações não reconhecidas

A aba **Não reconhecidas** guarda mensagens de aplicativos que o WFinance já conhece, mas cujo texto ele ainda não soube transformar em lançamento. Pode ser um aviso novo do banco, um formato que mudou, ou um SMS.

Mensagem de um aplicativo que o WFinance não acompanha é ignorada. Ela não aparece nesta lista.

![Lista de notificações recebidas e não reconhecidas](Notificacoes%20-%20Lista%20notificacoes%20nao%20reconhecidas.png)

Cada card mostra a origem (o banco ou o app de SMS), a data, o título e o texto.

**Exibir somente notificações com valores** começa ligado. Assim, avisos sem número (publicidade, dica de segurança, saldo sem movimentação) ficam de fora. Desligue para ver tudo o que foi guardado.

Toque no card para ler o texto completo.

Deslize para a **direita**:

- **reprocessar** — tira o item da lista e tenta ler de novo. Se o app já tiver aprendido aquele texto, surge um rascunho na aba **Capturadas** ou, no caso de cotação, a taxa é gravada. Se continuar sem leitura, o item volta para cá;
- **enviar para análise** — manda aquela mensagem para a equipe WFinance.

Deslize para a **esquerda** para excluir.

**Excluir tudo** apaga a lista, com confirmação.

Itens com mais de **3 semanas** saem sozinhos. A aba **Capturadas** não tem esse prazo: o rascunho fica até você importar ou apagar.

O link **O que são as notificações pendentes?** resume essas ações e lista os aplicativos reconhecidos.

### Enviar para análise

O envio pede confirmação e mostra a origem, o título e a mensagem que serão encaminhados. Só segue o que você confirmar.

A mesma mensagem não é enviada duas vezes.

Depois do envio, um ícone no canto do card indica o andamento:

| Ícone | Significado |
|-------|-------------|
| Seta de envio | A equipe ainda não respondeu. |
| Círculo com visto | A análise foi concluída. |
| Círculo com X | A análise foi cancelada. |

Toque no card para ver o texto e, quando a equipe escrever, o retorno. A resposta chega quando o celular sincroniza. É preciso internet.

O número da aba conta só o que **ainda não** foi enviado. O card enviado continua na lista até você apagar, reprocessar ou completar as 3 semanas.

Quando a equipe passar a reconhecer aquele texto, volte ao item e **reprocesse**. O rascunho, se a leitura der certo, aparece em **Capturadas** para você importar.

---

## Taxas de câmbio

Em **Configurações**, no bloco **Funcionalidades e segurança**, a opção **Importar taxas de câmbio** grava a cotação que alguns aplicativos enviam por notificação.

Como usar:

1. Ligue **Importar taxas de câmbio**.
2. No aplicativo (por exemplo, o que você usa para conta em outra moeda), ligue o alerta de atualização de taxa.
3. Mantenha a **leitura de notificações** ativa.

A taxa entra direto, sem passar pela lista de rascunhos. A cotação inversa é gravada junto. **Saiba mais** mostra quais aplicativos estão cobertos no momento.

Com a opção desligada, o WFinance pode até reconhecer o aviso, mas não atualiza as suas taxas.

SMS não traz cotação. Esse caminho é só de notificação de aplicativo.

---

## O que a captura entende

O conjunto de bancos, cartões, carteiras e apps de SMS cresce com o tempo, sem depender só de uma atualização na Play Store. A lista vigente está no **Saiba mais** da própria tela de importação e no **Saiba mais** das taxas de câmbio.

Mensagens típicas: compra no cartão, PIX enviado ou recebido, boleto, pagamento agendado, pagamento de fatura, transferência, saque, depósito, tarifa e recompensa.

Três destinos possíveis:

| O que aconteceu | Onde fica |
|-----------------|-----------|
| O texto foi entendido como movimentação | Aba **Capturadas**, até você importar. |
| O texto foi entendido como cotação, com a opção ligada | Nas taxas de câmbio, na hora. |
| O aplicativo é conhecido e o texto não foi entendido | Aba **Não reconhecidas**. |
| O aplicativo não é acompanhado | A mensagem é deixada de lado. |

Pagamento agendado pode vir com data futura. Confira no formulário. Se o dinheiro ainda não saiu, grave e, na lista de transações, deixe o lançamento como [previsto](../Transactions/Transactions.md#status-previsto-efetivado-e-reconciliado).

---

## Privacidade

A leitura acontece no aparelho, para achar movimentação e cotação. O WFinance não usa esses avisos para propaganda.

O rascunho e a lista de não reconhecidas ficam só neste celular. Eles não sobem para a nuvem e não passam para outra pessoa do espaço. O lançamento importado, sim, entra no espaço ativo.

No envio para análise, seguem a origem, o título e o texto daquela mensagem — os mesmos que a confirmação mostra na tela. Nada mais da sua lista é enviado junto.

Só uma pessoa fica logada por vez neste aparelho. Quem importar o rascunho fica com o lançamento.

---

## Dicas

- Ligue a leitura de notificações e o envio de notificações. Deixe o SMS para o caso em que o banco avisa por mensagem de texto e a notificação chega vazia.
- No app do banco, mantenha os alertas de compra e de PIX ligados.
- Importe com alguma frequência. A aba de capturadas não se limpa sozinha.
- Confira conta e categoria na primeira vez de cada loja ou cartão. Nas seguintes, a sugestão costuma acertar.
- Se o valor já estiver lançado (você digitou antes, ou importou a fatura), o aviso de duplicidade evita o dobro.
- Uma mensagem que você não quer vira lançamento: deslize para excluir, ou use **Excluir tudo**.
- Mensagem estranha de um banco que você usa: envie para análise e, depois da atualização, reprocesse.
- Se a captura morre com o app fechado, abra **Otimização de Bateria** e siga o passo do seu celular.
- O filtro **somente notificações com valores** esconde aviso sem número. Desligue se estiver procurando um texto específico.

---

## Se a captura não aparecer

| Situação | O que conferir |
|----------|----------------|
| Nenhum aviso vira rascunho | Leitura de notificações ligada, e o WFinance autorizado na tela de acesso a notificações do Android. |
| SMS do banco não entra | Leitura de SMS ligada. Se a notificação do app de mensagens chegar com o texto oculto, desligue as notificações aprimoradas do Android. |
| Funciona uns minutos e para | **Otimização de Bateria**, sobretudo em Xiaomi, Huawei, Oppo e similares. Desbloqueie o celular uma vez depois de reiniciar. |
| O aviso do WFinance não aparece | **Envio de notificações**. O rascunho pode estar na lista mesmo assim. |
| A compra está na outra aba | O texto ainda não é reconhecido. Envie para análise ou reprocesse depois de uma atualização. |
| Não está em aba nenhuma | O aplicativo daquele aviso ainda não é acompanhado, ou o banco não enviou notificação. |
| Conta ou categoria vieram vazias | É a primeira vez daquela descrição ou daquele cartão. Preencha e grave; a próxima sugestão usa essa escolha. |
| Possível duplicidade | Já existe lançamento com o mesmo valor e o mesmo sinal naquela data ou num dia vizinho. |
| Não vejo o card na tela inicial | Não há rascunho, ou você está só visualizando este espaço. As não reconhecidas não aparecem nesse card. |
| Reprocessei e nada mudou | O formato ainda não foi aprendido. A mensagem volta para **Não reconhecidas**. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
