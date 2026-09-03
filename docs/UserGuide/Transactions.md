# Transações

Uma **transação** é qualquer movimentação de dinheiro no WFinance: o salário que entrou, o almoço no cartão, o PIX para a poupança, o pagamento da fatura.

Esta página explica o que é uma transação, os tipos, os sinais (incluindo estornos), os status e como as listas funcionam. Para o passo a passo do formulário de lançamento, veja [Como lançar uma transação](ManageTransaction.md). Visão geral do app: [WFinance](WFinance.md).

---

## Em uma frase

Cada transação responde: **quanto**, **quando**, **em qual conta**, **de que tipo** e **em que situação** (prevista, feita ou já conferida).

O app trata **três tipos**: receita, despesa e transferência. Aplicação e resgate de investimento são transferências especiais. O mesmo formulário serve para criar, editar, copiar ou importar.

---

## Os três tipos

### Receita

Dinheiro **entrando** na conta: salário, freelance, aluguel recebido, rendimento creditado.

- Exige **conta** e **categoria**.
- Pode ir para conta bancária, carteira ou cartão de crédito.
- Aceita **recorrência fixa** (salário, pensão) e **parcelamento**, quando fizer sentido.
- Na lista, entra nas **Entradas**.

O sinal normal da receita é **positivo (+)**. Um sinal invertido registra um **estorno** — por exemplo, devolver parte de um valor que você tinha recebido.

### Despesa

Dinheiro **saindo** da conta: mercado, luz, assinatura, compra no cartão.

- Exige **conta** e **categoria**.
- Pode sair de conta bancária, carteira ou cartão de crédito.
- Aceita **parcelamento** (muito comum no cartão) e **recorrência fixa** (aluguel, escola, streaming).
- Na lista, entra nas **Saídas**.

O sinal normal da despesa é **negativo (−)**. Um sinal invertido registra um **estorno** — reembolso do plano de saúde, devolução da loja, crédito na fatura.

### Transferência

Dinheiro **saindo de uma conta e entrando em outra**, no mesmo espaço. Exemplos: PIX da corrente para a poupança, pagamento da fatura, aplicação em investimento, saque para a carteira.

- Exige **conta origem** e **conta destino**.
- **Não tem categoria**: só muda o dinheiro de lugar, sem entrar no “quanto gastei” como uma compra.
- Vira **dois lançamentos ligados**. Se você editar ou apagar um lado, o outro acompanha. Os dois compartilham o mesmo status.
- Aceita contas de moedas diferentes, com conversão.
- Cartão de crédito **não entra** em transferência (compras e estornos de compra ficam como despesa ou receita no próprio cartão).
- Conta de investimento **só** aparece em transferência — é assim que se faz [aplicação e resgate](#aplicação-e-resgate).

O sinal normal é **negativo (−)** na origem (saiu daqui, entrou ali). O sinal invertido desfaz a transferência.

---

## Sinais e estornos

Toda transação tem um **sinal**. Ele não muda o tipo: um reembolso médico continua sendo **despesa** de Saúde, só que com o sinal trocado.

| Tipo              | Sinal normal                         | Estorno (sinal invertido)              | Exemplo                                             |
|-------------------|--------------------------------------|----------------------------------------|-----------------------------------------------------|
| **Despesa**       | − dinheiro saindo                    | + reembolso, devolução, crédito        | Consulta R$ 200 (−); plano devolve R$ 150 (+)       |
| **Receita**       | + dinheiro entrando                  | − devolução do que você tinha recebido | Cliente pagou R$ 1.000 (+); você devolve R$ 200 (−) |
| **Transferência** | − saiu da origem e entrou no destino | + desfaz o movimento                   | Poupança → corrente; depois você reverte            |

Por que isso importa:

- o reembolso **não vira receita** — a categoria continua correta;
- relatórios mostram o gasto bruto e o líquido daquela categoria;
- o histórico reflete o que aconteceu, sem maquiar a natureza do lançamento.

Na lista, estorno de despesa entra nas **Entradas** e estorno de receita nas **Saídas**, porque o dinheiro andou no sentido contrário. O tipo (despesa/receita) permanece.

---

## Status: previsto, efetivado e reconciliado

O status diz se o valor já vale para o saldo real.

| Status           | O que significa                                                               | Entra no saldo?                    |
|------------------|-------------------------------------------------------------------------------|------------------------------------|
| **Previsto**     | Ainda vai acontecer (ou você está só planejando).                             | Não. Aparece só no saldo previsto. |
| **Efetivado**    | Já aconteceu.                                                                 | Sim.                               |
| **Reconciliado** | Conferido com extrato bancário ou fatura importada. Maior nível de confiança. | Sim.                               |

Regras práticas:

- Lançamentos **avulsos** costumam nascer **efetivados**.
- **Parcelas e recorrências** nascem **previstas**. Você confirma quando o dinheiro de fato sai ou entra.
- **Compras no cartão** já nascem **efetivadas**. Não existe “previsto” em fatura.
- Na **carteira** (dinheiro vivo), o ciclo é previsto ↔ efetivado. Reconciliado não se usa.
- Os dois lados de uma transferência **sempre** têm o mesmo status.

Só o que está **efetivado** ou **reconciliado** muda o saldo da conta, os totais da barra inferior e o progresso das metas.

---

## Em quais contas uma transação pode viver

| Conta                 | Receita / despesa | Transferência          | Como a lista se comporta                                         |
|-----------------------|-------------------|------------------------|------------------------------------------------------------------|
| **Conta bancária**    | Sim               | Sim                    | Extrato do mês, com saldo de cada dia e opção de ver o previsto. |
| **Carteira**          | Sim               | Sim                    | Controle do dinheiro em espécie.                                 |
| **Cartão de crédito** | Sim               | Não                    | Fatura do ciclo (não o mês civil).                               |
| **Investimento**      | Não               | Só aplicação e resgate | Aportes, resgates e avaliações de saldo.                         |

Uma transação também guarda:

- **descrição** (obrigatória);
- **categoria e subcategoria** (obrigatórias em receita e despesa; transferências ficam sem);
- **observações** (opcional);
- **tags** (rótulos livres, como “viagem” ou “reforma”), para recortes nos relatórios;
- **moeda e valor** — o valor original e, se for o caso, o valor já convertido para a moeda da conta.

---

## Aplicação e resgate

São transferências, não receitas nem despesas.

**Aplicação (aporte)** — conta bancária → investimento. Aumenta o valor investido.

**Resgate** — investimento → conta bancária. Diminui o valor investido.

A conta bancária precisa ser a **mesma associada** àquele investimento no cadastro do ativo. Se a conta não bater, o app não conclui o lançamento.

Rendimento, perda e imposto **não** se lançam como aplicação. Use a **avaliação de saldo** no extrato do investimento.

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

O botão de adicionar abre o [formulário de lançamento](ManageTransaction.md). Você também chega nele ao editar, copiar ou confirmar um lançamento capturado de notificação.

**Copiar** preenche todos os campos com o lançamento original. Ajuste o que for diferente e grave. Alguns tipos automáticos (pagamento de fatura, avaliação de saldo, ajuste) não podem ser copiados.

**Importar** preenche com o que veio da notificação ou do SMS. Confira conta, categoria e valor antes de confirmar. A captura sozinha **não** cria o lançamento.

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

Recorrência fixa e parcelamento são **mutuamente exclusivos**: no mesmo lançamento você escolhe um ou nenhum.

### Parcelamento

O valor total é dividido em N parcelas iguais (a primeira pode receber o ajuste dos centavos). Todas as parcelas são criadas de uma vez, com status **previsto**, cada uma na data certa.

No cartão, cada parcela cai na **fatura correspondente**.

Útil para: compra em 10 vezes, inscrição anual dividida, financiamento.

Cada parcela pode ser ajustada depois, sozinha.

### Recorrência fixa

O mesmo valor se repete a cada período, até o limite da série. Também nasce **previsto**.

Útil para: salário, aluguel, escola, streaming, pensão.

Frequências: diária, semanal, bi-semanal, quinzenal, mensal, bimestral, trimestral, semestral, anual e bi-anual.

O app limita o tamanho da série para não criar lançamentos demais de uma vez (por exemplo, cerca de 1 ano no diário e alguns anos no mensal).

### Ao editar ou apagar uma série

Você escolhe o alcance:

| Opção                 | Efeito                                                                                                                         |
|-----------------------|--------------------------------------------------------------------------------------------------------------------------------|
| **Só esta**           | Altera ou apaga apenas o lançamento aberto. Os outros da série continuam.                                                      |
| **Esta e as futuras** | A partir desta data, inclusive. **Substitui** ajustes que você tinha feito à mão nessas ocorrências. O passado fica como está. |
| **Toda a série**      | Todas as ocorrências, inclusive as passadas. Também **substitui** ajustes individuais.                                         |

Uma ocorrência editada sozinha vira uma **exceção**: o restante da série não muda — até você escolher “futuras” ou “todas”.

---

## Várias moedas no lançamento

Há dois valores possíveis:

- o valor **da transação** (o que você pagou ou recebeu, na moeda da operação);
- o valor **na conta** (o mesmo movimento já convertido para a moeda da conta).

Se as moedas forem iguais, os dois coincidem. Se forem diferentes, o app usa a taxa do dia (ou a que você informar).

**Receita ou despesa** — a conversão aparece quando a moeda do lançamento é diferente da moeda da conta (compra em euro numa conta em reais).

**Transferência** — a conversão aparece quando origem e destino têm moedas diferentes. A moeda da transação é sempre a da **conta origem**. Cada lado guarda o valor na moeda daquela conta.

Exemplo: compra de US$ 100 numa conta em reais, com taxa 5,00 → a conta registra R$ 500.

No formulário:

- **Recarregar taxa** busca a cotação da data da transação (ou de hoje, se a data estiver vazia);
- **Editar** libera taxa, data da cotação e valor já convertido;
- o valor na moeda da conta é calculado sozinho a partir da taxa.

Cadastre suas moedas mais usadas em Configurações → Moedas.

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

| Origem                         | Quando aparece                                      | Pode editar?                                                             |
|--------------------------------|-----------------------------------------------------|--------------------------------------------------------------------------|
| **Manual**                     | Você criou.                                         | Sim.                                                                     |
| **Notificação de app**         | Importou de uma captura.                            | Sim, em geral.                                                           |
| **Reconciliação / importação** | Veio de extrato ou fatura.                          | Com cuidado — já foi conferido.                                          |
| **Saldo inicial**              | Valor que a conta já tinha ao ser cadastrada.       | Só em investimento. Nas outras contas, apague e faça um ajuste de saldo. |
| **Ajuste de saldo**            | Correção pontual do saldo da conta.                 | Não. Apague e crie outro.                                                |
| **Pagamento de cartão**        | Você pagou a fatura.                                | Não edite. Se errou, exclua e pague de novo.                             |
| **Previsão de pagamento**      | O app estima o pagamento futuro da fatura.          | Não. Some sozinha quando o pagamento real é lançado.                     |
| **Saldo da fatura anterior**   | O que não foi pago e passou para o ciclo seguinte.  | Não. Some se a fatura anterior for paga no valor exato.                  |
| **Importação de fatura**       | Compra vinda do arquivo do cartão.                  | Conforme as regras da fatura.                                            |
| **Avaliação de saldo**         | Você informou o valor atual do investimento.        | Sempre efetivada; não mude o status.                                     |
| **Aporte direto**              | Entrada no investimento sem passar por outra conta. | Sem cópia.                                                               |
| **Imposto**                    | Lançamento de imposto ligado ao investimento.       | Sem cópia.                                                               |

Se o app recusar a edição, em geral a mensagem explica o caminho certo (excluir e refazer, ou deixar o automático cuidar).

---

## Excluir transações

- Lançamento **único**: some só ele. Se for transferência, os dois lados saem juntos.
- **Série**: escolha se apaga só esta, as futuras ou todas.
- Tags daquele lançamento saem junto.
- Os saldos são recalculados na hora (criação, edição, exclusão ou mudança de status).
- Apagar um **pagamento de fatura** desfaz o pagamento na fatura.

Algumas origens automáticas (previsão de pagamento, saldo rolado) **não** podem ser apagadas à mão.

---

## O que entra e o que não entra no saldo

Pense assim:

- **Saldo real** = efetivados + reconciliados.
- **Saldo previsto** = real + o que ainda está previsto.
- **Metas** = só efetivados e reconciliados.
- **Estorno** continua sendo receita, despesa ou transferência — só o sinal inverte.
- **Saldo do período** (visão geral) soma entradas e saídas da lista, sem puxar meses anteriores.
- **Saldo inicial e final** (uma conta bancária ou carteira) consideram o que veio do mês passado.

Na visão geral, transferências aparecem nos dois lados (saiu daqui, entrou ali). No extrato de uma conta, você vê só a perna daquela conta.

---

## Dicas rápidas

- Use **previsto** para o que ainda não saiu da conta. O saldo real continua limpo.
- Prefira **transferência** em vez de “despesa + receita” quando o dinheiro só mudou de conta.
- Reembolso é **estorno de despesa**, não receita nova.
- Categorias boas deixam relatórios e metas úteis. Tags resolvem recortes que atravessam várias categorias.
- Ative a captura de notificações se você já recebe alerta de PIX e compra no celular.
- No cartão, olhe a **fatura**, não o mês do calendário.
- No investimento, avalie o saldo com alguma frequência para a rentabilidade não ficar parada.
- O passo a passo dos campos está em [Como lançar uma transação](ManageTransaction.md).
- No plano Free há limite de transações por espaço. O Premium remove esse teto — veja [Conta de usuário](UserAccount.md).
