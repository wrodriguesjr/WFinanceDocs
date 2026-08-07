# WFinance

WFinance é um aplicativo avançado de controle financeiro desenvolvido em Kotlin para Android, que oferece gestão financeira completa com **sincronização em tempo real** e **colaboração entre múltiplos usuários**. Projetado com arquitetura offline-first, o WFinance funciona perfeitamente sem internet e sincroniza automaticamente quando há conexão disponível.

## 🚀 Principais Características

- **Gestão Financeira Completa**
  - Transações (receitas, despesas, transferências)
  - Contas bancárias e carteiras
  - Cartões de crédito e faturas
  - Investimentos e rentabilidade
  - Categorização e etiquetas
  - Metas de gastos
  - Relatórios detalhados

- **Colaboração e Compartilhamento**
  - Espaços compartilhados para gestão colaborativa (familiar, empresarial)
  - Sistema de convites com códigos de 8 caracteres
  - Controle granular de permissões (Proprietário, Administrador, Membro, Somente Leitura)
  - Espaço pessoal privado para cada usuário
  - Sincronização automática entre dispositivos e usuários

- **Recursos Avançados**
  - Arquitetura offline-first: funciona 100% sem internet
  - Sincronização bidirecional em tempo real (~5-10 segundos)
  - Resolução automática de conflitos (Last-Write-Wins)
  - Suporte para múltiplas moedas e taxas de câmbio
  - Transações recorrentes e parceladas
  - Captura automática de transações via SMS e notificações bancárias
  - Captura automática de taxas de câmbio (Wise e outros)
  - Reconciliação bancária
  - Importação de extratos e faturas

## 💻 Requisitos

- Android API 31 ou superior
- Conta Google para autenticação e sincronização
- Conexão com internet para sincronização entre dispositivos (opcional - app funciona offline)

## 🛠️ Tecnologias

- **Linguagem**: Kotlin
- **Arquitetura**: MVVM (Model-View-ViewModel) com Clean Architecture
- **Principais Bibliotecas**:
  - Jetpack Components (LiveData, ViewModel, Room, Navigation, WorkManager)
  - Material Design Components
  - Firebase (Authentication, Firestore, Cloud Storage)
  - Hilt para injeção de dependência
  - Coroutines e Flow para programação assíncrona
  - ViewBinding para acesso a views

## 📱 Funcionalidades Detalhadas

### Espaços Compartilhados
- **Espaço Pessoal**: Privado e exclusivo para cada usuário
- **Espaços Colaborativos**: Compartilhe finanças com família ou equipe
- **Convites por Código**: Sistema de códigos de 8 caracteres para fácil compartilhamento
- **Permissões Granulares**: 4 níveis de acesso (Proprietário, Administrador, Membro, Somente Leitura)
- **Gestão de Membros**: Adicione, remova e gerencie permissões de participantes
- **Isolamento de Dados**: Cada espaço possui dados completamente independentes

### Sincronização com a Nuvem
- **Offline-First**: App funciona 100% sem conexão à internet
- **Sincronização Bidirecional**: Dados sincronizados automaticamente entre dispositivos
- **Tempo Real**: Latência de ~5-10 segundos para mudanças aparecerem em outros dispositivos
- **Resolução de Conflitos**: Sistema automático Last-Write-Wins
- **24 Entidades Sincronizadas**: Transações, contas, categorias, metas, investimentos e mais
- **Confiabilidade**: Fila persistente garante que nenhuma operação seja perdida

### Transações
- Criação e gerenciamento de transações financeiras
- Status: Prevista, Efetivada e Reconciliada
- Suporte para transações recorrentes e parceladas
- Captura automática de transações de notificações bancárias e SMS
- Importação facilitada de dados capturados
- Importação de extratos bancários (OFX)

### Organização
- Categorias e subcategorias personalizáveis
- Sistema de etiquetas (tags)
- Hierarquia de contas e carteiras
- Gestão de cartões de crédito e faturas
- Metas de gastos com acompanhamento de progresso

### Investimentos
- Controle de contas de investimento
- Cálculo de rentabilidade
- Suporte para múltiplas moedas
- Conversão automática de valores

### Relatórios
- Fluxo de caixa consolidado
- Análise por categoria e tag
- Desempenho de investimentos
- Relatórios personalizados por período

## 📖 Documentação

Para informações mais detalhadas sobre o funcionamento do sistema, consulte:

### Sincronização com a Nuvem
- [Visão Geral do Sistema de Sincronização](docs/cloudsync/00_VISAO_GERAL.md)
- [Fundamentos e Estruturas Básicas](docs/cloudsync/01_FUNDAMENTOS.md)
- [Fluxo de Sincronização (PUSH/PULL)](docs/cloudsync/02_FLUXO_SINCRONIZACAO.md)
- [Sincronização em Tempo Real](docs/cloudsync/03_TEMPO_REAL.md)
- [Estrutura do Firestore](docs/cloudsync/04_ESTRUTURA_FIRESTORE.md)
- [Como Adicionar Nova Entidade Sincronizável](docs/cloudsync/05_ADICIONAR_ENTIDADE.md)

### Espaços Compartilhados (Grupos)
- [Visão Geral de Espaços](docs/group/SPACES_OVERVIEW.md)
- [Sistema de Convites](docs/group/INVITATION_SYSTEM.md)
- [Sistema Offline-First e Sincronização](docs/group/OFFLINE_FIRST_SYNC.md)
- [Níveis de Permissões](docs/group/GROUP_PERMISSIONS.md)

### Transações
- [Conceitos de Transações](docs/transaction/TRANSACTIONS_CONCEPTS.md)
- [Regras de Transações](docs/transaction/TRANSACTION_RULES.md)
- [Regras de Status das Transações](docs/transaction/TRANSACTION_RULES_STATUS.md)
- [Modos de uso da TransactionsActivity](docs/transaction/TRANSACTIONS_ACTIVITY_MODES.md)

### Outros Recursos
- [Conceitos de Cartões de Crédito](docs/creditcard/CREDIT_CARD_CONCEPTS.md)
- [Captura de Transações via Notificações e SMS](docs/notifications/TRANSACTION_CAPTURE_NOTIFICATIONS.md)
- [Notificações de Post](docs/notifications/POST_NOTIFICATIONS.md)

### Documentação Técnica
- [Histórico de Implementação](docs/implementation_history/) - Detalhes técnicos de cada fase implementada
- [Regras de Segurança do Firestore](docs/firestore_rules/) - Security Rules (DEV e PRD)


## 👨‍💻 Desenvolvimento

O projeto está estruturado seguindo Clean Architecture e separação de responsabilidades:

```
app/
├── src/
│   ├── main/
│   │   ├── java/com/wrj/wfinance/
│   │   │   ├── data/                    # Camada de dados
│   │   │   │   ├── sync/                  # Sistema de sincronização
│   │   │   │   │   ├── core/                # SyncManager, EntitySyncRepository
│   │   │   │   │   ├── realtime/            # Sincronização em tempo real
│   │   │   │   │   ├── initial/             # Sincronização inicial
│   │   │   │   │   └── processing/          # Pós-processamento
│   │   │   │   ├── transactions/          # Transações
│   │   │   │   ├── groups/                # Espaços e membros
│   │   │   │   ├── capturedtransactions/  # Dados capturados
│   │   │   │   └── migrations/            # Migrações do banco
│   │   │   ├── firestore/               # Interface com Firestore
│   │   │   │   ├── CloudDataSource.kt       # Interface abstrata
│   │   │   │   ├── GenericCloudMapper.kt    # Mapper universal
│   │   │   │   └── FirestoreDataSource.kt   # Implementação
│   │   │   ├── usecases/                # Regras de negócio
│   │   │   │   ├── groups/                  # Lógica de espaços
│   │   │   │   ├── transactions/            # Lógica de transações
│   │   │   │   └── sync/                    # Lógica de sincronização
│   │   │   ├── screens/                 # Activities e UI
│   │   │   │   ├── groups/                  # Telas de gestão de espaços
│   │   │   │   ├── transactions/            # Telas de transações
│   │   │   │   └── ...
│   │   │   ├── services/                # Serviços em background
│   │   │   │   ├── transactioncapture/    # Captura de notificações
│   │   │   │   └── sms/                   # Captura via SMS
│   │   │   ├── workers/                 # WorkManager Workers
│   │   │   ├── utils/                   # Utilitários
│   │   │   └── notifications/           # Notificações ao usuário
│   │   └── res/                        # Recursos (layouts, strings, etc)
│   ├── test/                           # Testes unitários
│   └── androidTest/                    # Testes instrumentados
└── docs/                               # Documentação detalhada
```

### Arquitetura de Sincronização

O sistema de sincronização é o coração do WFinance moderno:

**Componentes Principais:**
- **SyncManager**: Orquestrador que coordena sincronização de todas as entidades
- **EntitySyncRepository**: Lógica genérica reutilizável para qualquer entidade
- **GenericCloudMapper**: Conversor universal (eliminou ~3500 linhas de mappers específicos)
- **SyncOutbox**: Fila persistente de operações pendentes
- **RealtimeSyncCoordinator**: Coordena sincronização em tempo real

**Como Funciona:**

```
Dispositivo A (Usuário cria transação)
    ↓
1. Salva no Room Database local (offline)
    ↓
2. Enfileira na SyncOutbox
    ↓
3. OutboxMonitor detecta mudança (tempo real)
    ↓
4. SyncManager.push() → Firebase Firestore (3-10 segundos)
    ↓
Firebase Firestore (nuvem)
    ↓
5. FirestoreRealtimeListener detecta mudança
    ↓
6. SyncManager.pull() → Room Database local
    ↓
Dispositivo B (Usuário vê a transação - 5-10 segundos)
```

**Principais Decisões:**
- Offline-first para experiência sem interrupções
- Last-Write-Wins para resolução automática de conflitos
- Soft delete para rastreabilidade e sincronização de deleções
- Sincronização incremental para economia de rede
- Idempotência para garantir consistência em retries

## 🎯 Casos de Uso

### 1. Finanças Familiares
Casal gerencia orçamento doméstico de forma colaborativa:
- Ambos registram despesas e receitas em tempo real
- Veem relatórios consolidados instantaneamente
- Coordenam metas de gastos compartilhadas

### 2. Pequenos Negócios
Gestão financeira empresarial com múltiplos usuários:
- Sócios compartilham controle financeiro
- Contador tem acesso somente leitura
- Todos acessam de dispositivos diferentes

### 3. Gestão Delegada
Familiar gerencia finanças com transparência:
- Filho gerencia finanças dos pais
- Pais têm acesso para visualização
- Transparência total das movimentações

### 4. Múltiplos Dispositivos
Use o mesmo espaço em vários dispositivos:
- Celular pessoal, tablet e celular do trabalho
- Sincronização automática entre todos
- Dados sempre atualizados

## 🎓 Princípios do Sistema

### Offline-First
O aplicativo funciona 100% sem internet. Todas as operações são realizadas localmente primeiro e sincronizadas quando há conexão disponível.

### Colaboração em Tempo Real
Sincronização automática em ~5-10 segundos permite que múltiplos usuários vejam mudanças quase instantaneamente.

### Resolução Automática de Conflitos
Sistema Last-Write-Wins (LWW) resolve conflitos automaticamente sem intervenção do usuário. A última modificação sincronizada prevalece.

### Privacidade e Segurança
- Dados isolados por espaço
- Controle granular de permissões
- Auditoria completa de todas as operações
- Validação em múltiplas camadas (Client, UseCase, Firestore Rules)

### Confiabilidade
- Fila persistente garante que nenhuma operação seja perdida
- Soft delete permite rastreabilidade e recuperação
- Sincronização incremental economiza rede

## 📊 Estatísticas do Sistema

### Sincronização
- **24 entidades sincronizáveis** (19 GROUP-SCOPED + 5 USER-SCOPED)
- **Latência de sincronização**: ~5-10 segundos (antes: 30 minutos)
- **Melhoria de performance**: 95%+ na velocidade de sincronização
- **~2000 linhas de código** para sincronizar todas as entidades
- **Economia de código**: GenericCloudMapper eliminou ~3500 linhas de mappers específicos

### Espaços
- **4 níveis de permissão**: Proprietário, Administrador, Membro, Somente Leitura
- **Convites com código de 8 caracteres**: fácil compartilhamento
- **Validade do convite**: 7 dias
- **Sincronização automática** de membros e permissões
- **Membros ilimitados** por espaço (limitado pela assinatura)

## 📱 Screenshots

[Adicione screenshots do aplicativo aqui]

## 📞 Contato

- **Desenvolvedor**: Waldir Rodrigues Junior
- **Email**: waldir.rodrigues@gmail.com
- **GitHub**: https://github.com/wrodriguesjr

## 📄 Licença

[Adicione informações sobre a licença do projeto]
