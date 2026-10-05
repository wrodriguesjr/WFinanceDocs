# A tela de investimentos

A tela de **Investimentos** mostra, no mês que você está olhando, quanto as contas valem, quanto desse valor ainda é dinheiro que você colocou e quanto ainda é ganho ou perda.

O conceito e os outros guias estão em [Investimentos](Investments.md). Criar a conta: [Como cadastrar uma conta de investimento](ManageInvestmentAccount.md).

---

## Como chegar

O ícone de **investimentos** na barra inferior abre esta tela no mês atual.

Toque num card para abrir o extrato daquela conta, no mesmo mês. Lá ficam **Avaliar**, **Aplicar**, **Resgatar** e **Outros**.

---

## A tela

A lista abre no **mês atual**, no modo **resultado acumulado**: o histórico inteiro até o fim daquele mês.

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

De onde vêm investido e resultado: [Como a rentabilidade é calculada](Profitability.md).

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

Toque no card (fora da seta e do ícone de aviso) para abrir o **extrato** daquela conta, no mês que a tela está mostrando.

### Ícone de aviso

O ícone ao lado do nome pede uma **atualização de saldo**. Quando ele aparece e como lançar a avaliação está em [Atualizar o saldo](UpdateBalance.md).

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

## Moeda

Cada conta tem a própria moeda. Nesta tela, os **valores** são convertidos para a moeda padrão do seu perfil, com a taxa do **último dia do mês** selecionado.

O **percentual de cada card** é o da moeda da conta: converter para real não altera esse %. O percentual do **topo** já é calculado com os valores convertidos, então ele descreve a carteira na sua moeda.

Sem taxa cadastrada para aquela moeda e aquela data, o relatório avisa, em vez de mostrar um total convertido pela metade. As taxas ficam em Central → Estrutura financeira → **Taxas de câmbio**. No gráfico, um mês antigo sem taxa reaproveita a taxa do mês selecionado.

---

## Quem pode ver

Quem está no espaço só para visualizar vê a lista e os números, sem criar conta nem lançar aplicação, resgate ou avaliação. O limite de contas do plano Free está em [Como cadastrar uma conta de investimento](ManageInvestmentAccount.md#o-que-o-app-não-deixa-gravar).

---

## Se algo não bate

| Situação | O que conferir |
|----------|----------------|
| % do topo diferente do % do card | No modo do mês, o card usa saldo inicial + aportes. O topo divide pelo investido. No modo acumulado, o topo é a carteira inteira, não a média dos cards. |
| Lista vazia | Filtro de conta, tipo ou tag pode ter escondido tudo. Ou **Considerar contas inativas** está desligado e a conta foi arquivada. |
| Conta em dólar com valores estranhos em real | Falta a taxa do fim daquele mês, ou a taxa usada não é a que você esperava. |
| Não consigo aplicar nem avaliar | Papel de somente leitura neste espaço. Conta inativa também some da lista de contas na hora de lançar uma transferência. |
| Resultado zerado, com o ícone de aviso | Falta [atualizar o saldo](UpdateBalance.md). |
| O resgate ou o percentual não fecham com a conta de cabeça | Veja [como a rentabilidade é calculada](Profitability.md). |

---

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
