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
Sincronização automática em ~10-15 segundos permite que múltiplos usuários vejam mudanças quase instantaneamente.

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

### Espaços
- **4 níveis de permissão**: Proprietário, Administrador, Membro, Somente Leitura
- **Convites com código**: fácil compartilhamento
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
