# Transações

Uma **transação** é qualquer movimentação de dinheiro no WFinance: o salário que entrou, o almoço no cartão, o PIX para a poupança, o pagamento da fatura.

Esta página explica o que é uma transação, os tipos, os status e como usar as telas do dia a dia. Para o panorama do app, volte a [WFinance](WFinance.md).

---

## Em uma frase

Cada transação responde: **quanto**, **quando**, **em qual conta**, **de que tipo** e **em que situação** (prevista, feita ou já conferida).

---

## Os três tipos

### Receita

Dinheiro **entrando** na conta: salário, freelance, reembolso, rendimento creditado, presente.

Na lista, receitas entram nas **Entradas**.

### Despesa

Dinheiro **saindo** da conta: mercado, conta de luz, assinatura, compra no cartão.

Na lista, despesas entram nas **Saídas**.

### Transferência

Dinheiro **saindo de uma conta e entrando em outra**. Exemplos: PIX da conta corrente para a poupança, pagamento da fatura do cartão, aporte em investimento, saque para a carteira.

A transferência vira **dois lançamentos ligados**:

- um de saída na conta de origem;
- um de entrada na conta de destino.

Se você editar ou apagar um lado, o outro acompanha. Os dois sempre compartilham o mesmo status.

Quando as contas têm moedas diferentes (reais e dólares, por exemplo), cada lado guarda o valor na moeda daquela conta, com a taxa de câmbio do dia.

> Transferência **não** é receita nem despesa. Ela só muda o dinheiro de lugar. Por isso não deve entrar no “quanto gastei no mês” da mesma forma que uma compra.

---

## Status: previsto, efetivado e reconciliado

O status diz se o valor já vale para o saldo real.

| Status | O que significa | Entra no saldo? |
| --- | --- | --- |
| **Previsto** | Ainda vai acontecer (ou você está só planejando). | Não. Aparece só no saldo previsto. |
| **Efetivado** | Já aconteceu. | Sim. |
| **Reconciliado** | Conferido com extrato do banco ou fatura do cartão. | Sim. |

Regras práticas:

- Lançamentos **avulsos** costumam nascer **efetivados**.
- **Parcelas e recorrências** nascem **previstas**. Você confirma quando o dinheiro de fato sai ou entra.
- **Compras no cartão** já nascem **efetivadas**. Não existe “previsto” em fatura.
- Na **carteira** (dinheiro vivo), o ciclo é previsto ↔ efetivado. Reconciliado não se usa.

Só o que está **efetivado** ou **reconciliado** muda o saldo da conta, os totais da barra inferior e o progresso das metas.

---

## Em quais contas uma transação pode viver

| Conta | Como a lista se comporta |
| --- | --- |
| **Conta bancária** | Extrato do mês, com saldo de cada dia e opção de ver o previsto. |
| **Carteira** | Controle do dinheiro em espécie. |
| **Cartão de crédito** | Fatura do ciclo (não o mês civil). |
| **Investimento** | Aportes, resgates e avaliações de saldo. |

Uma transação também guarda:

- **descrição** (obrigatória);
- **categoria e subcategoria** (nas transferências podem ficar em branco);
- **observações** (opcional);
- **tags** (rótulos livres, como “viagem” ou “reforma”);
- **moeda e valor** — o valor original e, se for o caso, o valor já convertido para a moeda da conta.

---

## Como as listas funcionam

A tela de transações muda conforme o contexto. No topo, o ícone de informação explica o modo atual.

### Visão geral

Mostra lançamentos de **todas as contas** ao mesmo tempo. Serve para olhar o mês inteiro, o resultado de uma meta ou um filtro amplo.

Não há saldo diário. A barra de baixo mostra **entradas**, **saídas** e o **saldo do período** (só o que está na tela, sem puxar meses anteriores). Os totais usam a **moeda padrão do seu perfil**, convertendo quando preciso.

### Extrato bancário

É o extrato de **uma conta**. Os saldos andam dia a dia.

- O **saldo inicial** do mês vem do saldo final do mês anterior.
- A linha de **saldo diário** mostra quanto havia naquele dia.
- Você pode ligar os totais **previstos** para ver o caixa até o fim do mês, incluindo o que ainda não aconteceu.

Tudo aparece na **moeda da conta**, mesmo que o lançamento original esteja em outra moeda.

### Carteira

Funciona como um extrato simples do dinheiro vivo. O objetivo é refletir o que está no bolso agora — por isso o previsto aparece na lista, mas **não** altera o saldo.

### Fatura do cartão

A lista segue o **ciclo da fatura** (fechamento e vencimento), não o mês do calendário.

No cabeçalho você encontra:

- total da fatura, valor pago e o que ainda falta;
- datas de fechamento, vencimento e último pagamento;
- **Pagar fatura** — quitação total ou parcial, gerando o lançamento na conta que você escolher;
- **Importar fatura** — conferência com o arquivo do cartão;
- **Criar fatura** — se o ciclo ainda não existir;
- **Retirada em dinheiro** — saque no cartão (quando fizer sentido);
- **Recalcular datas** — se você mudou o dia de fechamento ou vencimento do cartão.

Parcelas caem automaticamente na fatura certa. Não existe saldo diário: o foco é o ciclo.

### Extrato de investimentos

Mostra o que entrou e saiu daquele ativo.

Pelo cabeçalho você:

- **Avalia o saldo** — informa quanto vale hoje; o app registra o rendimento ou a perda;
- **Aplica** — transfere da conta bancária para o investimento;
- **Resgata** — traz o valor de volta para a conta bancária.

Os números (investido, saldo, resultado e rentabilidade) ficam na moeda da conta de investimento. Sem avaliação recente, aparece um aviso.

### Modo relatório

Quando você vem de um relatório, a lista mostra **somente** os lançamentos daquele recorte. Não dá para incluir novos itens nem mudar o período — o objetivo é analisar.

---

## Criar, editar, copiar e importar

O botão de adicionar abre o formulário. Você também chega nele ao editar, copiar ou confirmar um lançamento capturado de notificação.

### Campos do lançamento

1. **Tipo** — receita, despesa ou transferência.
2. **Descrição** — o nome que você vai reconhecer na lista.
3. **Valor e moeda** — o valor da operação. Se a moeda for diferente da conta, o app pede a taxa e mostra o valor convertido.
4. **Data**.
5. **Conta** — ou, na transferência, **origem** e **destino**.
6. **Categoria e subcategoria** — para receitas e despesas.
7. **Fatura** — obrigatória quando a conta é um cartão. O app sugere o ciclo pela data da compra; você pode trocar.
8. **Observações** e **tags**.
9. **Recorrência ou parcelamento**, se for o caso.

Na hora de sair sem gravar, o app pergunta se você quer descartar.

### Gestos na lista

Deslize o lançamento:

- **para um lado** — marcar como efetivado (ou voltar para previsto) e editar;
- **para o outro** — excluir.

Quem está no espaço só como leitor não vê essas ações.

Toque no item para abrir os detalhes (conta, categoria, tags, moeda, origem do lançamento).

Puxe a lista para baixo para atualizar.

---

## Parcelas e recorrência

### Parcelamento

O valor total é dividido em N parcelas iguais (a primeira pode receber o ajuste dos centavos). Todas as parcelas são criadas de uma vez, com status **previsto**, cada uma na data certa.

Útil para: compra em 10 vezes, inscrição anual dividida, reforma paga em etapas.

### Recorrência fixa

O mesmo valor se repete a cada período, até o limite da série. Também nasce **previsto**.

Útil para: salário, aluguel, escola, streaming, contribuição mensal.

Frequências disponíveis:

Diária, semanal, quinzenal, mensal, bimestral, trimestral, semestral, anual — e intervalos próximos (bi-semanal, bi-anual).

O app limita o tamanho da série para não criar lançamentos demais de uma vez (por exemplo, cerca de 1 ano no diário e alguns anos no mensal).

### Ao editar ou apagar uma série

Você escolhe o alcance:

| Opção | Efeito |
| --- | --- |
| **Só esta** | Altera ou apaga apenas o lançamento aberto. Os outros da série continuam. |
| **Esta e as futuras** | A partir desta data, inclusive. O passado fica como está. |
| **Toda a série** | Todas as ocorrências. |

Uma ocorrência editada sozinha vira uma **exceção**: o restante da série não muda.

---

## Várias moedas no lançamento

Há dois valores possíveis:

- o valor **da transação** (o que você pagou ou recebeu, na moeda da operação);
- o valor **na conta** (o mesmo movimento já convertido para a moeda da conta).

Se as moedas forem iguais, os dois coincidem. Se forem diferentes, o app usa a taxa do dia (ou a que você informar).

Exemplo: compra de US$ 100 numa conta em reais, com taxa 5,00 → a conta registra R$ 500.

Na transferência entre contas de moedas diferentes, cada lado usa a moeda da própria conta. A taxa fica registrada com a data da cotação.

No formulário, o botão de atualizar busca a taxa daquela data. Cadastre suas moedas mais usadas em Configurações → Moedas.

---

## Filtros e ordem

Na lista você pode filtrar por:

- texto da descrição;
- categorias de despesa ou de receita;
- contas;
- tipo (receita, despesa, transferência);
- status;
- intervalo de datas ou de valores;
- tags;
- mostrar ou esconder os previstos.

Dá para ordenar por data, valor ou descrição.

---

## Captura automática (notificações e SMS)

Com a permissão ativada, o WFinance lê notificações e SMS de bancos e cartões e identifica compras, PIX, pagamentos e, em alguns apps (como o Wise), taxas de câmbio.

O fluxo é:

1. A mensagem chega no celular, mesmo com o app fechado.
2. Se o WFinance reconhecer o formato, guarda um **rascunho**.
3. Você abre a lista de capturas, confere conta, categoria e valor, e importa.
4. Só então vira uma transação de verdade no seu espaço.

Enquanto não importar, o rascunho não pertence a ninguém. No aparelho só uma pessoa fica logada por vez: quem importar fica com o lançamento, e o rascunho some para não ser usado de novo.

A captura **não cria lançamento sozinha**. Sempre há a etapa de confirmação.

---

## Importação de extrato e fatura

Além das notificações, você pode importar:

- **extrato bancário** (arquivo OFX, por exemplo) para conferir a conta e marcar lançamentos como reconciliados;
- **fatura do cartão**, para cruzar as compras com o arquivo oficial.

A reconciliação é a forma de dizer: “isto bate com o banco”. Lançamentos já reconciliados não devem ser importados de novo.

---

## Lançamentos que o próprio app cria

Alguns itens não nascem do botão “adicionar”. Eles existem para manter saldos e faturas coerentes.

| Origem | Quando aparece | Pode editar? |
| --- | --- | --- |
| **Manual** | Você criou. | Sim. |
| **Notificação de app** | Importou de uma captura. | Sim, em geral. |
| **Reconciliação / importação** | Veio de extrato ou fatura. | Com cuidado — já foi conferido. |
| **Saldo inicial** | Valor que a conta já tinha ao ser cadastrada. | Só em investimento. Nas outras contas, apague e faça um ajuste de saldo. |
| **Ajuste de saldo** | Correção pontual do saldo da conta. | Não. Apague e crie outro. |
| **Pagamento de cartão** | Você pagou a fatura. | Não edite. Se errou, exclua e pague de novo. |
| **Previsão de pagamento** | O app estima o pagamento futuro da fatura. | Não. Some sozinha quando o pagamento real é lançado. |
| **Saldo da fatura anterior** | O que não foi pago e passou para o ciclo seguinte. | Não. Some se a fatura anterior for paga no valor exato. |
| **Importação de fatura** | Compra vinda do arquivo do cartão. | Conforme as regras da fatura. |
| **Avaliação de saldo** | Você informou o valor atual do investimento. | Sempre efetivada; não mude o status. |
| **Aporte direto** | Entrada no investimento sem passar por outra conta. | Sem cópia. |
| **Imposto** | Lançamento de imposto ligado ao investimento. | Sem cópia. |

Se o app recusar a edição, em geral a mensagem explica o caminho certo (excluir e refazer, ou deixar o automático cuidar).

---

## Excluir transações

- Lançamento **único**: some só ele. Se for transferência, os dois lados saem juntos.
- **Série**: escolha se apaga só esta, as futuras ou todas.
- Tags daquele lançamento saem junto.
- Os saldos são recalculados na hora.
- Apagar um **pagamento de fatura** desfaz o pagamento na fatura.

Algumas origens automáticas (previsão de pagamento, saldo rolado) **não** podem ser apagadas à mão.

---

## O que entra e o que não entra no saldo

Pense assim:

- **Saldo real** = efetivados + reconciliados.
- **Saldo previsto** = real + o que ainda está previsto.
- **Metas** = só efetivados e reconciliados.
- **Estorno** (valor negativo) continua sendo receita ou despesa — só o sinal inverte.

Na visão geral, transferências aparecem nos dois lados (saiu daqui, entrou ali). No extrato de uma conta, você vê só a perna daquela conta.

---

## Dicas rápidas

- Use **previsto** para o que ainda não saiu da conta (boleto do mês que vem, parcela futura). O saldo real continua limpo.
- Prefira **transferência** em vez de “despesa + receita” quando o dinheiro só mudou de conta.
- Categorias boas deixam relatórios e metas úteis. Tags resolvem recortes que atravessam várias categorias.
- Ative a captura de notificações se você já recebe alerta de PIX e compra no celular.
- No cartão, olhe a **fatura**, não o mês do calendário.
- No investimento, avalie o saldo com alguma frequência para a rentabilidade não ficar parada.
- No plano Free há limite de transações por espaço. O Premium remove esse teto — veja [Conta de usuário](UserAccount.md).
