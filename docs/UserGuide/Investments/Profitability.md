# Como a rentabilidade é calculada

O investido e o resultado acumulado não saem de uma conta de menos no fim do mês. O app **refaz o histórico**, lançamento por lançamento, na ordem da data. No mesmo dia, vale a ordem em que você lançou.

Os outros guias estão em [Investimentos](Investments.md). O rendimento só entra nessa conta quando você [atualiza o saldo](UpdateBalance.md).

---

## Duas gavetas

Esse método se chama **replay cronológico**. A cada passo ele atualiza duas gavetas:

- a do **capital** (o que a tela chama de investido);
- a do **rendimento** (o que a tela chama de resultado).

O saldo da conta é a soma das duas. A rentabilidade em percentual é o resultado dividido pelo investido.

---

## O que cada lançamento faz

| Lançamento | Onde se registra | Efeito |
|------------|------------------|--------|
| **Saldo inicial** | No [cadastro da conta](ManageInvestmentAccount.md), ou em **Outros** no extrato | Entra inteiro no investido. Resultado continua zero. |
| **Aplicação** | **Aplicar** no extrato: sai da conta bancária associada | Aumenta o investido. A conta bancária diminui no mesmo valor. |
| **Aporte direto** | **Outros** no extrato | Aumenta o investido, sem mexer em outra conta do app. Serve para dinheiro que já estava no investimento, ou que veio de fora. |
| **Avaliação de saldo** | **Avaliar** no extrato | Você informa quanto a conta vale. A **diferença** para o saldo que o app já tinha vai toda para o resultado. Pode ser positiva ou negativa. O investido não muda. |
| **IOF ou IR** | **Outros** no extrato | Reduz o resultado. Se o resultado não cobre o imposto, ele zera e o que faltar sai do investido. |
| **Resgate** | **Resgatar** no extrato: volta para a conta bancária associada | Leva uma **fatia** do investido e uma fatia do resultado, na mesma proporção do saldo naquele momento. |

Só entram lançamentos **efetivados** ou **reconciliados**. Previsto fica de fora até mudar de status.

A avaliação é o único lugar do rendimento. Juros, dividendos, variação de cota e prejuízo aparecem quando você diz qual é o saldo novo. Se você nunca avalia, o resultado permanece zero e o saldo fica igual ao que entrou e saiu.

Na [tela de investimentos](InvestmentScreen.md), com o resultado acumulado desligado, a rentabilidade **do mês** é outra conta: saldo final − saldo inicial − aportes líquidos. Ela responde o que mudou naquele mês, além do dinheiro que entrou ou saiu.

---

## Um exemplo, do zero até o resgate

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
Investido, resultado e saldo vão a **zero**. Uma conta zerada não fica com lucro pendurado nem com valor investido negativo.

---

## Imposto

Com resultado de R$ 200, um IR de R$ 50 deixa o resultado em R$ 150. O investido não muda, então o percentual cai.

Se o imposto for maior do que o resultado, o resultado zera e a diferença diminui o investido. Imposto não é resgate: ele não volta para a conta bancária como transferência. Você lança o valor em **Outros**.

---

## O que este cálculo é

É a leitura do **que você lançou** no WFinance. Ele serve para acompanhar a carteira dentro do app, no mesmo espaço das contas e das reservas.

O rendimento de cada mês depende da [atualização de saldo](UpdateBalance.md). Lance também o IOF e o IR quando a instituição descontar: o imposto sai do resultado.

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| Apliquei e a rentabilidade em % caiu | O dinheiro novo entrou no investido e ainda não rendeu. O resultado em reais só muda na próxima avaliação. |
| Resgatei e o resultado diminuiu | Esperado. O resgate leva uma parte do ganho junto com o capital. O que saiu está na conta bancária. |
| Conta zerada ainda mostra lucro ou investido negativo | Confira se o resgate foi do saldo inteiro e se está efetivado. Zerar a conta zera investido e resultado. |
| Rentabilidade do mês alta demais depois de um depósito | O depósito precisa ser **aplicação** ou **aporte direto**. Se ele só aparecer dentro da avaliação, a diferença inteira vira rendimento. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
