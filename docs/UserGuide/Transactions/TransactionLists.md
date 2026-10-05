# As listas

A tela de transações muda conforme o contexto. No topo, o ícone de informação explica o modo atual.

Os outros guias estão em [Transações](Transactions.md). Criar um lançamento: [Como lançar uma transação](ManageTransaction.md).

---

## Visão geral

Mostra lançamentos de **todas as contas** ao mesmo tempo. Serve para olhar o mês inteiro, o resultado de uma meta ou um filtro amplo.

Não há saldo diário. A barra de baixo mostra **entradas**, **saídas** e o **saldo do período** (só o que está na tela, sem puxar meses anteriores). Os totais usam a **moeda padrão do seu perfil**, convertendo quando preciso.

---

## Extrato bancário

É o extrato de **uma conta**. Os saldos andam dia a dia.

- O **saldo inicial** do mês vem do saldo final do mês anterior.
- A linha de **saldo diário** mostra quanto havia naquele dia.
- Você pode ligar os totais **previstos** para ver o caixa até o fim do mês, incluindo o que ainda não aconteceu.

Tudo aparece na **moeda da conta**, mesmo que o lançamento original esteja em outra moeda. A conversão está em [Conversão de moeda](CurrencyConversion.md).

---

## Carteira

Funciona como um extrato simples do dinheiro vivo. O objetivo é refletir o que está no bolso agora — por isso o previsto aparece na lista, mas o saldo usa só o que já foi efetivado. Reconciliado não se usa na carteira. Os status estão em [Status](TransactionStatus.md).

---

## Fatura do cartão

A lista segue o **ciclo da fatura** (fechamento e vencimento), não o mês do calendário.

No cabeçalho você encontra:

- total da fatura, valor pago e o que ainda falta;
- datas de fechamento, vencimento e último pagamento;
- **Pagar fatura** — quitação total ou parcial, gerando o lançamento na conta que você escolher;
- **Importar fatura** — conferência com o arquivo do cartão;
- **Criar fatura** — se o ciclo ainda não existir;
- **Retirada em dinheiro** — saque no cartão, quando fizer sentido;
- **Recalcular datas** — se você mudou o dia de fechamento ou vencimento do cartão.

Parcelas caem automaticamente na fatura certa. Não existe saldo diário: o foco é o ciclo.

---

## Extrato de investimentos

Mostra o que entrou e saiu daquele ativo.

Pelo cabeçalho você:

- **Avalia o saldo** — informa quanto a conta vale. Sem isso, a rentabilidade não anda. O passo a passo está em [Atualizar o saldo](../Investments/UpdateBalance.md);
- **Aplica** — transfere da conta bancária para o investimento;
- **Resgata** — traz o valor de volta para a conta bancária.

Os números (investido, saldo, resultado e rentabilidade) ficam na moeda da conta de investimento. Sem avaliação recente, aparece um aviso. O que cada um significa na carteira inteira está em [A tela de investimentos](../Investments/InvestmentScreen.md).

---

## Modo relatório

Quando você vem de um relatório ou de uma meta, a lista mostra **somente** os lançamentos daquele recorte. Não dá para incluir novos itens nem mudar o período. O objetivo é analisar.

---

## Gestos

Deslize o lançamento:

- **para um lado** — marcar como efetivado (ou voltar para previsto) e editar;
- **para o outro** — excluir.

Quem está no espaço só como leitor não vê essas ações.

Toque no item para abrir os detalhes (conta, categoria, tags, moeda, origem do lançamento).

Puxe a lista para baixo para atualizar.

O que não pode ser apagado à mão está em [Lançamentos que o app cria](SpecialTransactions.md).

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

## Contato

Dúvidas de uso: [wfinance.suporte@gmail.com](mailto:wfinance.suporte@gmail.com).
