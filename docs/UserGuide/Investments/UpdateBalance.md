# Atualizar o saldo

O app só calcula rentabilidade depois que você informa quanto a conta vale. Aplicação e resgate movem o **capital**. Juros, dividendos, variação de cota e prejuízo entram na **avaliação de saldo**. Sem essa atualização, o resultado fica em zero e o saldo da tela continua igual à soma do que entrou e saiu.

Os outros guias estão em [Investimentos](Investments.md). O efeito dessa diferença no cálculo está em [Como a rentabilidade é calculada](Profitability.md).

---

## Com que frequência

O ritmo que faz o número de cada mês fazer sentido é **pelo menos uma avaliação por mês**, no fim do mês, com o valor que o banco ou a corretora mostra naquele dia. Se o intervalo for maior, o ganho de vários meses cai inteiro na data da avaliação seguinte. Os meses sem avaliação ficam com rentabilidade zero.

O aviso dos **30 dias** existe por isso. Ele aparece na conta **ativa** quando:

- nunca houve uma avaliação, ou
- a última foi há mais de 30 dias.

O saldo inicial do cadastro não conta como avaliação. Uma conta recém-criada já pode mostrar o ícone, mesmo com o saldo preenchido: ainda não há rendimento registrado. O aviso olha a data de **hoje**, mesmo que a [tela de investimentos](InvestmentScreen.md) esteja num mês antigo.

Conta inativa não mostra o ícone. Na lista, o nome dela fica mais claro.

Uma [reserva](../Reserves/Reserves.md) que inclui a conta usa o saldo da **última avaliação**.

---

## Onde lançar

1. Na [tela de investimentos](InvestmentScreen.md), toque no card da conta. Abre o extrato daquele mês.
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

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| Resultado zerado e saldo igual ao investido | Ainda não há avaliação, ou a última repetiu o saldo que o app já tinha. |
| Ícone de aviso numa conta nova | Esperado até a primeira avaliação. O saldo inicial não conta. |
| Saldo menor que o do banco | Vale o que foi lançado. Previsto não entra. Sem avaliação nova, o saldo não acompanha a cotação. |
| Vários meses de rendimento apareceram de uma vez | A avaliação cobre o intervalo desde a anterior. Avalie todo mês para o número cair no mês certo. |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
