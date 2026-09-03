# Como lançar uma transação

Esta página é o passo a passo da tela que **cria, edita, copia e importa** lançamentos. Os conceitos (tipos, status, estornos, saldos) estão em [Transações](Transactions.md).

Você chega aqui pelo botão de adicionar, ao deslizar um item para editar, ao copiar, ou ao confirmar uma notificação capturada.

---

## O que esta tela faz

Um único formulário cobre:

- receita, despesa e transferência;
- aplicação e resgate de investimento (são transferências);
- conta bancária, carteira ou cartão;
- lançamento simples, parcelado ou recorrente;
- categoria, subcategoria e tags;
- moeda diferente da conta, com taxa de conversão.

O título da tela muda conforme o modo: criar, editar, copiar ou importar. Os campos são os mesmos; o que muda é o que já vem preenchido.

Se você sair sem gravar, o app pergunta se quer descartar.

---

## Campos, na ordem em que aparecem

### Tipo

Escolha **despesa**, **receita** ou **transferência**. Isso libera ou esconde o restante:

| Tipo               | Conta            | Categoria   | Quem pode ser a conta                               |
|--------------------|------------------|-------------|-----------------------------------------------------|
| Despesa ou receita | Uma conta        | Obrigatória | Bancária, carteira ou cartão. **Não** investimento. |
| Transferência      | Origem e destino | Não existe  | Bancária, carteira ou investimento. **Não** cartão. |

Aplicação = bancária → investimento. Resgate = investimento → bancária. A bancária precisa ser a **conta associada** àquele investimento.

### Descrição

Nome que você vai reconhecer na lista. Em importação, já vem o texto da notificação — ajuste se quiser.

### Valor, sinal e moeda

Informe o valor e a moeda da operação.

Os botões **+** e **−** definem o [sinal](Transactions.md#sinais-e-estornos):

- despesa normal: **−**
- receita normal: **+**
- transferência normal: **−**
- estorno: o contrário do normal

Não troque o tipo para registrar um reembolso. Mantenha “despesa” (ou “receita”) e inverta o sinal.

### Data

Data em que o dinheiro saiu, entrou ou foi transferido. No cartão, essa data também ajuda o app a sugerir a fatura.

### Conta (ou origem e destino)

Toque para escolher. A lista já filtra o que vale para o tipo atual.

Na transferência, preencha os dois lados. Se as moedas forem diferentes, a área de câmbio aparece.

### Categoria e subcategoria

Obrigatórias em receita e despesa. A subcategoria é opcional se você quiser só o grupo maior.

Em transferência esses campos não aparecem.

### Fatura (só cartão)

Ao escolher um cartão, surge o seletor de **mês e ano da fatura**. O app sugere o ciclo pela data da compra e pelos dias de fechamento do cartão. Você pode trocar se a compra cair na fatura seguinte ou anterior.

Compras parceladas geram uma parcela em cada fatura futura.

### Observações e tags

Livres. Tags servem para recortes nos relatórios (viagem, obra, projeto) sem misturar com a categoria.

### Recorrência ou parcelamento

Três opções, **uma só**:

- **Nenhuma** — um lançamento único.
- **Recorrência fixa** — o mesmo valor se repete (salário, aluguel). Você escolhe a frequência.
- **Parcelamento** — o total vira N parcelas. Você informa quantidade e frequência.

Não dá para ligar recorrência e parcela ao mesmo tempo.

Ao **editar** um item de série, o app pergunta o alcance:

- **Somente esta** — só o lançamento aberto.
- **Esta e futuras** — a partir desta data; **apaga ajustes manuais** feitos nessas ocorrências.
- **Todas** — a série inteira, inclusive o passado; também substitui exceções.

---

## Quando a conversão de moeda aparece

A faixa de câmbio só entra se for necessária:

- receita ou despesa cuja moeda é diferente da moeda da conta;
- transferência entre contas de moedas diferentes (a moeda do lançamento é a da origem).

Nessa faixa você pode:

- **Recarregar** — busca a taxa da data da transação (ou de hoje, se a data estiver vazia);
- **Editar** — informa taxa, data da cotação e o valor já convertido.

O valor na moeda da conta é calculado a partir da taxa. Detalhes e exemplos: [Transações — várias moedas](Transactions.md#várias-moedas-no-lançamento).

---

## Copiar

Todos os campos vêm da transação original. Mude o que for diferente (data, valor, conta) e grave.

Não é possível copiar pagamento de fatura, previsão de pagamento, saldo rolado, avaliação de investimento, saldo inicial, ajuste de saldo, aporte direto nem imposto.

---

## Importar de notificação

Os campos vêm do rascunho capturado (descrição, valor, data, às vezes cartão). Confira a conta e a categoria — a captura nem sempre acerta — e grave.

Depois de importar, o rascunho some para não ser usado de novo.

---

## O que esta tela não faz

- Não muda o **status** (previsto / efetivado). Isso se faz na lista, deslizando o item.
- Não paga fatura, não avalia investimento e não importa extrato OFX. Essas ações ficam nos cabeçalhos das listas.
- Não cria lançamentos automáticos (saldo inicial, pagamento de cartão, carry-over). O app gera esses sozinho.

---

## Se o app recusar gravar

Mensagens comuns:

- falta conta, categoria, origem ou destino;
- investimento escolhido em receita ou despesa — use transferência;
- cartão escolhido em transferência — use despesa ou receita no cartão;
- conta bancária diferente da associada ao investimento;
- recorrência e parcela ligadas ao mesmo tempo;
- tentativa de editar um lançamento que o app controla sozinho.

A mensagem na tela costuma indicar o caminho. A tabela completa está em [Transações — lançamentos que o próprio app cria](Transactions.md#lançamentos-que-o-próprio-app-cria).
