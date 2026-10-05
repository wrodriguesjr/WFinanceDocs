# Investimentos

A tela de **Investimentos** responde, no mês que você está olhando: quanto as contas valem, quanto desse valor ainda é dinheiro que você colocou e quanto ainda é ganho ou perda.

Esta página explica os números, os filtros, o gráfico, por que o saldo precisa ser atualizado e o jeito como o app calcula a rentabilidade. Para criar a conta, escolher o tipo e ligar o banco de onde sai o dinheiro, veja [Como cadastrar uma conta de investimento](ManageInvestmentAccount.md). O extrato de cada conta (aplicar, resgatar, avaliar) está em [Transações](../Transactions/Transactions.md#extrato-de-investimentos). Visão geral do app: [WFinance](../WFinance.md).

---

## Em uma frase

Você informa o que entrou, o que saiu e, de tempos em tempos, **quanto a conta vale**. O app separa esse saldo em duas partes que continuam lá dentro:

- **Investido** — o capital que você colocou e que ainda não foi retirado.
- **Resultado** — o ganho ou a perda que ainda está na conta.

**Saldo = investido + resultado.** A rentabilidade em percentual é o resultado dividido pelo investido.

O app não busca cotação na corretora. Os números nascem dos lançamentos que você registra.

---

## Como chegar

| Caminho | Observação |
|---------|------------|
| Ícone de **investimentos** na barra inferior | Esta tela, aberta no mês atual. |
| Toque numa conta desta lista | Abre o extrato daquela conta, no mesmo mês. |

Para cadastrar a conta em si: Central → **Estrutura financeira** → **Investimentos**. O passo a passo está em [Como cadastrar uma conta de investimento](ManageInvestmentAccount.md).

---

## A tela

A lista abre no **mês atual**, no modo **resultado acumulado** (o histórico inteiro até o fim daquele mês, não só o que aconteceu nele).

![Tela de investimentos em outubro, com saldo, rentabilidade e a linha dos últimos 12 meses](Investimentos%20-%20geral%20com%20grafico.png)

De cima para baixo:

- o filtro de mês (setas, atalhos de início e fim, e o calendário);
- o link **Como funciona a gestão de investimentos?**, se a ajuda contextual estiver ligada;
- **Filtros** (contas, tipos, tags, resultado acumulado, contas inativas);
- os chips das tags que já estão em uso;
- o card de **totais**, com o gráfico dos últimos 12 meses;
- um **card por conta** de investimento.

Se não houver conta no recorte, a tela mostra: “Nenhuma conta de investimento encontrada para o período selecionado”.

As contas aparecem da que tem **maior saldo** para a que tem menor.

---

## Os números do topo

O card grande junta **todas as contas** que passaram pelos filtros, já na **moeda padrão** do seu perfil.

| Campo | Significado |
|-------|-------------|
| **Saldo total** | Soma do saldo de cada conta no **fim do mês** selecionado. |
| **Investido** | Soma do capital que ainda está em cada conta nesse fim de mês. |
| **Resultado** | Soma do ganho ou da perda que ainda está em cada conta. Com o modo acumulado desligado, passa a ser a rentabilidade **daquele mês**. |
| **Rentabilidade** | Resultado dividido pelo investido, em %. |

O saldo total leva o símbolo da moeda (`R$`). Investido, resultado e rentabilidade estão na mesma moeda, sem repetir o símbolo.

O percentual do topo é o da **carteira junta**. Uma conta em +10% e outra em +2% não viram “6% no meio”: cada uma pesa pelo tamanho do capital dela.

Verde é ganho. Vermelho é perda.

---

## Dois jeitos de olhar o mesmo mês

O interruptor **Resultado acumulado**, dentro de Filtros, muda a pergunta. Ele começa **ligado**.

| | Ligado (padrão) | Desligado |
|--|-----------------|-----------|
| Pergunta | Quanto dessa conta, até o fim deste mês, ainda é capital e quanto ainda é rendimento? | Neste mês, o saldo mudou por causa de dinheiro que entrou ou saiu, ou porque o investimento rendeu? |
| No card | Saldo total, total investido, resultado acumulado e o % acumulado | Saldo total, saldo inicial, aportes líquidos, rentabilidade do mês e o % do mês |
| No topo, **Resultado** | O resultado que ainda está nas contas | A soma da rentabilidade daquele mês |
| No topo, **Rentabilidade** | Resultado ÷ investido | Também resultado do mês ÷ investido |

Com o interruptor desligado, o **% de cada card** usa outra base: saldo inicial do mês mais os aportes líquidos. Por isso o percentual do topo e o percentual do card podem ser diferentes. Os dois estão certos para a pergunta de cada um.

O campo **Investido** do topo não muda de significado: continua sendo o capital que ainda está nas contas no fim do mês.

### O que cada linha do card quer dizer

**No modo acumulado** (o card começa fechado; a seta abre o resto):

| Campo | Significado |
|-------|-------------|
| **Saldo total** | Quanto a conta vale no fim do mês. |
| **Total investido** | Capital que ainda está nela. |
| **Resultado acumulado** | Ganho ou perda que ainda está nela. |
| **Result. acum. (%)** | Resultado acumulado ÷ total investido. |

**No modo do mês:**

| Campo | Significado |
|-------|-------------|
| **Saldo total** | Quanto a conta vale no fim do mês. |
| **Saldo inicial** | Quanto ela valia no fim do mês anterior. No primeiro mês da conta, o saldo de abertura entra aqui. |
| **Aportes líquidos** | Aplicações e aportes do mês, menos os resgates. Positivo: entrou mais do que saiu. |
| **Rentabilidade** | Saldo final − saldo inicial − aportes líquidos. |
| **Rent. (%)** | Essa rentabilidade ÷ (saldo inicial + aportes líquidos). |

Exemplo do mês. A conta começou abril com R$ 9.200, você aplicou R$ 800 e, no fim, avaliou o saldo em R$ 10.100.

- Aportes líquidos = R$ 800
- Rentabilidade = 10.100 − 9.200 − 800 = **R$ 100**
- Percentual = 100 ÷ (9.200 + 800) = **1%**

Os R$ 800 não são rendimento. Só os R$ 100 que apareceram além do dinheiro novo.

No **primeiro mês** da conta, o valor com que você a abriu aparece no saldo inicial, não em aportes líquidos. Assim a abertura não parece lucro.

---

## O card da conta

No card fechado dá para ver o nome, o tipo (CDB, fundo, tesouro…) e os dois valores principais. A seta abre o restante, inclusive as **tags** da conta.

Toque no card (fora da seta e do ícone de aviso) para abrir o **extrato** daquela conta, no mês que a tela está mostrando. Lá ficam **Avaliar**, **Aplicar**, **Resgatar** e **Outros**.

### Ícone de aviso

O ícone ao lado do nome pede uma **atualização de saldo**. Quando ele aparece, o que fazer e por que a rentabilidade depende disso está em [Atualizar o saldo](#atualizar-o-saldo).

O toque no ícone só explica o aviso. Para lançar a avaliação, abra o extrato da conta.

Conta inativa aparece com o nome mais claro e não mostra o ícone.

---

## O gráfico

A linha dentro do card de totais é o **saldo total** mês a mês: o mês selecionado e os **11 anteriores**.

- O último ponto é o mesmo **saldo total** do topo.
- Meses anteriores ao primeiro saldo somem da linha.
- Um mês sem movimento novo repete o saldo anterior.
- Os filtros de conta, tipo, tag e inativas valem para a linha também.
- A linha não dá zoom nem abre detalhe; a rolagem da tela continua normal.

Se ainda não há saldo para desenhar, o gráfico fica oculto.

---

## Filtros

Toque em **Filtros** para abrir. O número ao lado, quando aparece, conta o que está diferente do padrão.

| Filtro | Padrão | Efeito |
|--------|--------|--------|
| **Contas de investimento** | Todas | Restringe a lista e os totais às contas marcadas. |
| **Tipos de investimento** | Todos | Só CDB, só tesouro, só o que você marcar. |
| **Tags** | Nenhuma | Contas que tenham **pelo menos uma** das tags marcadas. |
| **Resultado acumulado** | Ligado | Desligar troca o card e o resultado do topo para a visão do mês. |
| **Considerar contas inativas** | Ligado | Desligar esconde contas arquivadas. |

Os chips logo abaixo dos filtros são as mesmas tags. Marcar um chip ou marcar a tag dentro de Filtros é a mesma escolha. Uma tag usada só por conta inativa só aparece no chip quando **Considerar contas inativas** está ligado.

“Nenhum filtro” no chip da linha significa que aquela lista está aberta para todos.

Os totais do topo são **refeitos** com as contas que sobraram. Esconder uma conta tira o saldo dela do gráfico e da soma.

---

## Atualizar o saldo

O app só calcula rentabilidade depois que você informa quanto a conta vale. Aplicação e resgate movem o **capital**. Juros, dividendos, variação de cota e prejuízo entram na **avaliação de saldo**. Sem essa atualização, o resultado fica em zero e o saldo da tela continua igual à soma do que entrou e saiu.

O ritmo que faz o número de cada mês fazer sentido é **pelo menos uma avaliação por mês**, no fim do mês, com o valor que o banco ou a corretora mostra naquele dia. Se o intervalo for maior, o ganho de vários meses cai inteiro na data da avaliação seguinte. Os meses sem avaliação ficam com rentabilidade zero.

O aviso dos **30 dias** existe por isso. Ele aparece na conta **ativa** quando:

- nunca houve uma avaliação, ou
- a última foi há mais de 30 dias.

O saldo inicial do cadastro não conta como avaliação. Uma conta recém-criada já pode mostrar o ícone, mesmo com o saldo preenchido: ainda não há rendimento registrado. O aviso olha a data de **hoje**, mesmo que a tela esteja num mês antigo.

### Onde lançar

1. Na tela de investimentos, toque no card da conta. Abre o extrato daquele mês.
2. No cabeçalho do extrato, toque em **Avaliar**.

A folha **Avaliação de saldo** abre por cima do extrato. O subtítulo é “Ajuste o saldo final após ganhos ou perdas”.

![Avaliação de saldo da previdência, com a diferença entre o saldo do app e o novo saldo](Investimentos%20-%20avaliacao%20de%20saldo.png)

| Campo | O que é |
|-------|---------|
| **Conta de investimento** | A conta do extrato. Não se troca nesta folha. |
| **Data da avaliação** | No mês atual, vem o dia de hoje — o rótulo **Hoje** aparece ao lado. Em outro mês, vem o dia 1º daquele mês. Dá para alterar. |
| **Saldo atual** | O valor que o app já tem para essa conta. |
| **Novo saldo** | O valor que a instituição está mostrando. |
| **Diferença a lançar** | Novo saldo menos o saldo atual. Esse valor entra no **resultado**. O investido não muda. |
| **Notas** | Opcional. |

Na captura, a previdência está em R$ 5.702,13 no app e o novo saldo é R$ 6.000,00. A diferença de **R$ 297,87** é o rendimento dessa atualização.

**Salvar** grava a avaliação no extrato e atualiza saldo, resultado e rentabilidade. **Cancelar** descarta.

Para corrigir uma avaliação já lançada, edite esse lançamento no extrato. A mesma folha abre de novo.

| Recado | Por quê |
|--------|---------|
| Selecione uma data para a avaliação | A data é obrigatória. |
| A data da avaliação não pode ser futura | A avaliação registra um saldo que já existe. |
| Digite o novo saldo avaliado | O campo novo saldo está vazio. |
| O saldo avaliado não pode ser negativo | O saldo da conta fica em zero ou acima. |
| O novo saldo deve ser diferente do saldo atual | Diferença zero não é rendimento nem perda. |

Quem está no espaço só para visualizar vê o extrato, sem **Avaliar**.

---

## Como o app calcula a rentabilidade

O investido e o resultado acumulado não saem de uma conta de menos no fim do mês. O app **refaz o histórico**, lançamento por lançamento, na ordem da data. No mesmo dia, vale a ordem em que você lançou.

Esse método se chama **replay cronológico**. A cada passo ele atualiza duas gavetas:

- a do **capital** (o que a tela chama de investido);
- a do **rendimento** (o que a tela chama de resultado).

O saldo da conta é a soma das duas.

### O que cada lançamento faz

| Lançamento | Onde se registra | Efeito |
|------------|------------------|--------|
| **Saldo inicial** | No cadastro da conta, ou em **Outros** no extrato | Entra inteiro no investido. Resultado continua zero. |
| **Aplicação** | **Aplicar** no extrato: sai da conta bancária associada | Aumenta o investido. A conta bancária diminui no mesmo valor. |
| **Aporte direto** | **Outros** no extrato | Aumenta o investido, sem mexer em outra conta do app. Serve para dinheiro que já estava no investimento, ou que veio de fora. |
| **Avaliação de saldo** | **Avaliar** no extrato | Você informa quanto a conta vale. A **diferença** para o saldo que o app já tinha vai toda para o resultado. Pode ser positiva ou negativa. O investido não muda. |
| **IOF ou IR** | **Outros** no extrato | Reduz o resultado. Se o resultado não cobre o imposto, ele zera e o que faltar sai do investido. |
| **Resgate** | **Resgatar** no extrato: volta para a conta bancária associada | Leva uma **fatia** do investido e uma fatia do resultado, na mesma proporção do saldo naquele momento. |

Só entram lançamentos **efetivados** ou **reconciliados**. Previsto fica de fora até mudar de status.

A avaliação é o único lugar do rendimento. Juros, dividendos, variação de cota e prejuízo aparecem quando você diz qual é o saldo novo. Se você nunca avalia, o resultado permanece zero e o saldo fica igual ao que entrou e saiu.

### Um exemplo, do zero até o resgate

Imagine um CDB.

**1. Abertura, R$ 10.000.**  
Investido 10.000 · resultado 0 · saldo 10.000 · rentabilidade 0%.

**2. No fim do mês o banco mostra R$ 10.200.** Você avalia esse valor.  
Os R$ 200 são rendimento. Investido continua 10.000 · resultado 200 · saldo 10.200 · rentabilidade 2%.

**3. Você aplica mais R$ 1.000.**  
Investido 11.000 · resultado continua 200 · saldo 11.200.  
A rentabilidade cai para cerca de **1,82%** (200 ÷ 11.000). O ganho em reais é o mesmo; a base ficou maior porque entrou dinheiro que ainda não rendeu.

**4. Nova avaliação: o saldo está R$ 11.500.**  
A diferença é 11.500 − 11.200 = R$ 300, somados ao resultado.  
Investido 11.000 · resultado 500 · saldo 11.500 · rentabilidade cerca de **4,55%** (500 ÷ 11.000).

**5. Você resgata R$ 2.300.**  
Na hora do resgate o saldo é 11.500, sendo 11.000 de capital (cerca de 95,7%) e 500 de rendimento (cerca de 4,3%). O resgate leva as duas partes nessa mistura:

- do investido saem R$ 2.200;
- do resultado saem R$ 100.

Ficam investido 8.800 · resultado 400 · saldo 9.200. A rentabilidade continua cerca de **4,55%**: o resgate diminuiu o tamanho, e levou capital e ganho na mesma proporção.

O resultado acumulado é o ganho **que ainda está na conta**. Os R$ 100 que saíram no resgate já foram para a conta bancária; eles deixam de aparecer como resultado do investimento.

**6. Resgate do que restou (R$ 9.200).**  
Investido, resultado e saldo vão a **zero**. Uma conta zerada não fica com “lucro pendurado” nem com valor investido negativo.

### Imposto

Com resultado de R$ 200, um IR de R$ 50 deixa o resultado em R$ 150. O investido não muda, então o percentual cai.

Se o imposto for maior do que o resultado, o resultado zera e a diferença diminui o investido. Imposto não é resgate: ele não volta para a conta bancária como transferência. Você lança o valor em **Outros**.

### O que este cálculo é

É a leitura do **que você lançou** no WFinance. Ele serve para acompanhar a carteira dentro do app, no mesmo espaço das contas e das reservas.

O rendimento de cada mês depende da [atualização de saldo](#atualizar-o-saldo). Lance também o IOF e o IR quando a instituição descontar: o imposto sai do resultado.

---

## Moeda

Cada conta tem a própria moeda. Nesta tela, os **valores** são convertidos para a moeda padrão do seu perfil, com a taxa do **último dia do mês** selecionado.

O **percentual de cada card** é o da moeda da conta: converter para real não altera esse %. O percentual do **topo** já é calculado com os valores convertidos, então ele descreve a carteira na sua moeda.

Sem taxa cadastrada para aquela moeda e aquela data, o relatório avisa, em vez de mostrar um total convertido pela metade. As taxas ficam em Central → Estrutura financeira → **Taxas de câmbio**. No gráfico, um mês antigo sem taxa reaproveita a taxa do mês selecionado.

---

## Plano e espaço

No **Free**, o teto é de **2 contas de investimento por espaço**. Arquivar não libera vaga: conta inativa continua contando. O Premium remove esse limite — veja [Conta de usuário](../UserAccount.md).

Quem está no espaço só para visualizar vê a lista e os números, sem criar conta nem lançar aplicação, resgate ou avaliação.

Trocar de espaço na [conta](../UserAccount.md) troca os investimentos junto. Cada espaço tem os seus.

Uma conta de investimento pode entrar numa [reserva](../Reserves/Reserves.md). O valor que a reserva usa é o saldo da **última avaliação**.

Contas do grupo **Liquidez restrita** (FGTS e previdência privada) usam o mesmo cálculo desta tela. No relatório de patrimônio elas aparecem separadas das contas de resgate mais livre.

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| Resultado zerado e saldo igual ao investido | Ainda não há avaliação de saldo, ou a última avaliação repetiu o saldo que o app já tinha. Use **Avaliar** no extrato. |
| Ícone de aviso numa conta nova | Esperado até a primeira avaliação. O saldo inicial não conta como avaliação. |
| Apliquei e a rentabilidade em % caiu | O dinheiro novo entrou no investido e ainda não rendeu. O resultado em reais só muda na próxima avaliação. |
| Resgatei e o resultado diminuiu | Esperado. O resgate leva uma parte do ganho junto com o capital. O que saiu está na conta bancária. |
| Conta zerada ainda mostra lucro ou investido negativo | Confira se o resgate foi do saldo inteiro e se está efetivado. No replay, zerar a conta zera investido e resultado. |
| Rentabilidade do mês alta demais depois de um depósito | O depósito precisa ser **aplicação** ou **aporte direto**. Se ele só aparecer dentro da avaliação, a diferença inteira vira rendimento. |
| % do topo diferente do % do card | No modo do mês, o card usa saldo inicial + aportes. O topo divide pelo investido. No modo acumulado, o topo é a carteira inteira, não a média dos cards. |
| Saldo menor que o do banco | Vale o que foi lançado. Previsto não entra. Sem avaliação nova, o saldo não acompanha a cotação. |
| Lista vazia | Filtro de conta, tipo ou tag pode ter escondido tudo. Ou **Considerar contas inativas** está desligado e a conta foi arquivada. |
| Conta em dólar com valores estranhos em real | Falta a taxa do fim daquele mês, ou a taxa usada não é a que você esperava. |
| Não consigo aplicar nem avaliar | Papel de somente leitura neste espaço. Conta inativa também some da lista de contas na hora de lançar uma transferência. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
