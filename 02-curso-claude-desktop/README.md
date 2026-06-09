# Claude Desktop — Automatize Tarefas do Dia a Dia

---

## Sumário

1. [Visão Geral do Curso](#visão-geral-do-curso)
2. [Onboarding](#onboarding)
   - [Apresentação — Claude Desktop](#1-apresentação--claude-desktop)
   - [O que é o Claude Desktop?](#2-o-que-é-o-claude-desktop)
   - [Por que o Claude vai mudar sua forma de trabalhar](#3-por-que-o-claude-vai-mudar-sua-forma-de-trabalhar)
3. [Dominando o Claude Cowork](#dominando-o-claude-cowork-1)
   - [Dominando o Claude Cowork](#4-dominando-o-claude-cowork)
   - [Projeto Prático: Analista de Contratos](#5-projeto-prático-analista-de-contratos)
   - [Automação: Briefing de E-mails e Agenda](#6-automação-briefing-de-e-mails-e-agenda)
   - [Projeto Prático: Analista de Dados (Detecção de Fraude)](#7-projeto-prático-analista-de-dados--detecção-de-fraude)
4. [Integrações do Claude](#integrações-do-claude)
   - [Diferença entre Cowork e Claude como extensão](#8-diferença-entre-cowork-e-claude-como-extensão)
   - [Claude para Excel: principais aplicações](#9-claude-para-excel-principais-aplicações)
   - [Projeto Prático: Dashboard Comercial](#10-projeto-prático-dashboard-comercial)
   - [Claude para PowerPoint: criando apresentações](#11-claude-para-powerpoint-criando-apresentações)
   - [Claude como extensão do Google Chrome](#12-claude-como-extensão-do-google-chrome)

---

## Visão Geral do Curso

O curso é estruturado em três grandes blocos:

| Seção | Aulas | Foco |
|---|---|---|
| **Onboarding** | 1–3 | Instalação, conceitos e impacto do Claude |
| **Dominando o Claude Cowork** | 4–7 | Automação de tarefas via Cowork (desktop) |
| **Integrações do Claude** | 8–11 | Excel, PowerPoint, Chrome e extensões |

---

## Onboarding

### 1. Apresentação — Claude Desktop

Apresentação do curso, metodologia e o que o aluno aprenderá ao longo das aulas. Visão geral da ferramenta Claude Desktop e como ela se encaixa no ecossistema de produtividade pessoal e profissional.

---

### 2. O que é o Claude Desktop?

O **Claude Desktop** é uma aplicação de inteligência artificial instalada diretamente no computador (Windows ou macOS), que permite ao usuário interagir com modelos de IA de forma local, sem depender exclusivamente de servidores externos para cada ação.

**Principais características:**

- **Privacidade e controle de dados** — ao contrário de plataformas web, os dados são processados em ambiente local do usuário, com maior segurança.
- **Interface intuitiva** — acessível mesmo para quem não possui experiência técnica com IA.
- **Capacidade offline** — permite operar com menor dependência de conexão contínua à internet.
- **Alta personalização** — adapta-se a diferentes casos de uso: análise de dados, automação de processos, desenvolvimento de aplicativos inteligentes.

#### Instalação no Windows

1. Acesse [https://claude.com/download](https://claude.com/download)
2. Clique em **Download** na opção Windows
3. Execute o arquivo `Claude Setup.exe` baixado
4. A instalação ocorre automaticamente
5. Ao abrir, clique em **Get started**
6. Faça login via **Continue with Google** ou outra opção
7. Autorize a abertura clicando em **Open Claude** quando solicitado no navegador
8. Configure atalhos de teclado e clique em **Continue**
9. ✅ Claude Desktop está pronto para uso no Windows

#### Instalação no macOS

1. Acesse [https://claude.com/download](https://claude.com/download)
2. Clique em **Download** na opção macOS
3. Abra o arquivo `Claude.dmg` baixado
4. **Arraste o ícone do Claude para a pasta Applications**
5. Aguarde a cópia finalizar
6. Abra o Claude na pasta Aplicativos
7. Se aparecer aviso de segurança, clique em **Open**
8. Clique em **Get started** e faça login com **Continue with Google**
9. Autorize o acesso e clique em **Continue** nas configurações iniciais
10. ✅ Claude Desktop está pronto para uso no macOS

---

### 3. Por que o Claude vai mudar sua forma de trabalhar

Nesta aula é apresentado o argumento central do curso: a IA não substitui o profissional, mas multiplica sua capacidade de execução. O Claude funciona como um assistente que entende contexto, lida com documentos complexos, e pode ser direcionado via prompts para entregar resultados concretos — rascunhos, análises, revisões de contratos, relatórios de dados — em fração do tempo manual.

---

## Dominando o Claude Cowork

### 4. Dominando o Claude Cowork

O **Claude Cowork** é a interface desktop do Claude que permite integração direta com arquivos locais do computador. Diferente do Claude Web (navegador), o Cowork acessa pastas, lê documentos, processa planilhas e gera novos arquivos diretamente no sistema de arquivos do usuário.

**Capacidades principais do Cowork:**

- Leitura e escrita de arquivos locais (PDF, DOCX, CSV, etc.)
- Acesso a diretórios configurados pelo usuário
- Execução de fluxos de trabalho encadeados (ler → processar → gerar saída)
- Integração com ferramentas como Excel e PowerPoint
- Operação via prompts em linguagem natural, sem necessidade de código

---

### 5. Projeto Prático: Analista de Contratos

#### Objetivo

Usar o Claude Desktop/Cowork para revisar um contrato de prestação de serviços, protegendo os interesses da empresa contratante (pequeno porte, orçamento limitado). O Claude gera uma versão revisada com **marcações de controle de alterações (redline)**, sinalizando riscos e propondo cláusulas mais favoráveis.

#### Arquivos utilizados

| Arquivo | Tipo | Descrição |
|---|---|---|
| `Contrato-Lockbreak_Digitalizado_1.pdf` | PDF | Contrato original escaneado (documento base) |
| `Prompt.md` | Markdown | Instrução enviada ao Claude |
| `Contrato-Lockbreak_Revisado_Redline.docx` | DOCX | Saída gerada pelo Claude com redline |

#### O Prompt utilizado

```
Estou revisando um contrato de serviços com um fornecedor. Somos uma empresa de 
pequeno porte com flexibilidade orçamentária limitada.

Crie uma versão revisada e com marcações que nos proteja de ficarmos presos a algo 
do qual não podemos sair, garanta que mantenhamos a propriedade de nossos dados e 
de qualquer trabalho pelo qual pagamos, e nos dê flexibilidade para ajustar ou 
desistir se as coisas não derem certo.

Crie um novo arquivo que seja uma cópia exata do contrato com o recurso de controle 
de alterações ativado. As linhas vermelhas devem mostrar as exclusões (texto 
riscado em vermelho) e as inserções (texto sublinhado colorido). Use um script para 
criar comentários ou sugestões nas margens do documento para cada edição, explicando 
o problema. Sinalize qualquer coisa que possa nos causar problemas mais tarde.
```

#### Passo a Passo do Projeto

**Passo 1 — Prepare os arquivos**

Crie uma pasta local com o contrato a ser analisado. No exemplo do curso, a estrutura é:
```
Claude Desktop/
└── contrato_fornecedor/
    ├── Contrato-Lockbreak_Digitalizado_1.pdf   ← contrato original
    └── Prompt.md                                ← instrução para o Claude
```

**Passo 2 — Forneça acesso ao diretório no Cowork**

No Claude Cowork, autorize o acesso à pasta `contrato_fornecedor`. O Claude passa a enxergar todos os arquivos dentro dela.

**Passo 3 — Execute o prompt**

Cole ou referencie o conteúdo do `Prompt.md` no chat do Cowork. O Claude irá:
1. Ler o PDF do contrato original
2. Identificar cláusulas problemáticas para uma pequena empresa
3. Propor alterações protetoras
4. Gerar o arquivo `Contrato-Lockbreak_Revisado_Redline.docx` com controle de alterações

**Passo 4 — Interprete o arquivo redline gerado**

O documento de saída `Contrato-Lockbreak_Revisado_Redline.docx` contém:

- **Texto riscado em vermelho** → trechos removidos ou problemáticos
- **Texto sublinhado colorido** → novas cláusulas inseridas para proteção
- **Comentários nas margens** → explicações do Claude sobre cada intervenção

#### Contrato analisado: principais pontos revisados

O contrato original era entre **MM Comércio e Locação de Eletro Eletrônicos Ltda (Locbreak)** e **Chip7 de Informática e Eletro-Eletrônicos Ltda ME**, envolvendo locação e manutenção de equipamentos (nobreaks e estabilizadores). O Claude identificou e revisou áreas críticas:

| Cláusula | Risco original | Proteção inserida |
|---|---|---|
| Rescisão contratual | Prazo excessivo de aviso prévio | Redução do prazo ou cláusula de saída antecipada |
| Propriedade intelectual | Ausência de cláusula explícita | Inserção de cláusula garantindo propriedade dos dados ao contratante |
| Reajuste de preços | Sem teto de reajuste definido | Limitador de reajuste indexado ao IPCA ou similar |
| SLA de manutenção | Penalidades indefinidas | Reforço dos descontos já previstos (5% por chamado não atendido, até 20% do valor mensal) |
| Responsabilidade civil | Cláusula ampla em favor do fornecedor | Limitação de responsabilidade proporcional |

#### Resultado esperado

Ao final, o aluno terá um contrato revisado profissionalmente em minutos, com rastreabilidade completa de todas as alterações sugeridas e justificativas em linguagem clara — tarefa que normalmente exigiria horas de trabalho manual ou consulta jurídica especializada.

---

### 6. Automação: Briefing de E-mails e Agenda

Nesta aula é demonstrado como usar o Claude Cowork para automatizar a criação de **briefings diários**, integrando:

- Resumo de e-mails importantes recebidos
- Leitura da agenda do dia
- Geração de um documento consolidado de prioridades

O Claude acessa as informações fornecidas pelo usuário (ou via integração com ferramentas de e-mail/calendário configuradas no Cowork) e produz um briefing executivo estruturado, economizando o tempo gasto na triagem manual de informações no início do dia.

---

### 7. Projeto Prático: Analista de Dados — Detecção de Fraude

#### Objetivo

Utilizar o Claude Desktop/Cowork para realizar análise exploratória de um dataset de transações bancárias, identificar padrões suspeitos e gerar um **relatório executivo de detecção de fraude** automaticamente.

#### Arquivos utilizados

| Arquivo | Tipo | Descrição |
|---|---|---|
| `Transacoes_Bancarias_Fraude.csv` | CSV | Dataset com 2.512 transações bancárias |
| `Transacoes_Bancarias_Fraude_Descricao.md` | Markdown | Dicionário de dados e contexto do dataset |
| `Relatorio_Analise_Fraude.pdf` | PDF | Relatório gerado pelo Claude como saída |

#### Sobre o Dataset

O arquivo `Transacoes_Bancarias_Fraude.csv` contém **2.512 amostras** de transações bancárias do período **02/01/2023 a 01/01/2024**, distribuídas entre **495 contas únicas**.

**Colunas do dataset:**

| Coluna | Tipo | Descrição |
|---|---|---|
| `TransactionID` | String | Identificador único da transação |
| `AccountID` | String | Identificador da conta (múltiplas transações por conta) |
| `TransactionAmount` | Float | Valor monetário da transação |
| `TransactionDate` | Datetime | Data e hora da transação |
| `TransactionType` | Categórico | `Credit` ou `Debit` |
| `Location` | String | Cidade (EUA) onde ocorreu a transação |
| `DeviceID` | String | Identificador do dispositivo utilizado |
| `IP Address` | String | Endereço IPv4 da transação |
| `MerchantID` | String | Identificador do comerciante |
| `AccountBalance` | Float | Saldo após a transação |
| `PreviousTransactionDate` | Datetime | Data da última transação da conta |
| `Channel` | Categórico | `Online`, `ATM` ou `Branch` (Agência) |
| `CustomerAge` | Inteiro | Idade do titular da conta |
| `CustomerOccupation` | Categórico | `Doctor`, `Engineer`, `Student`, `Retired` |
| `TransactionDuration` | Inteiro | Duração da transação em segundos |
| `LoginAttempts` | Inteiro | Tentativas de login antes da transação |

#### Passo a Passo do Projeto

**Passo 1 — Organize os arquivos**

Crie uma pasta local com os arquivos do dataset:
```
Transacoes_Bancarias/
├── Transacoes_Bancarias_Fraude.csv
└── Transacoes_Bancarias_Fraude_Descricao.md
```

**Passo 2 — Conceda acesso ao Cowork**

No Claude Cowork, aponte para a pasta `Transacoes_Bancarias`. O Claude passará a enxergar o CSV e o dicionário de dados.

**Passo 3 — Envie o prompt de análise**

Exemplo de prompt:
```
Leia o arquivo Transacoes_Bancarias_Fraude.csv e o dicionário de dados 
Transacoes_Bancarias_Fraude_Descricao.md.

Realize uma análise exploratória completa focada em detecção de fraude. 
Identifique padrões suspeitos, outliers e comportamentos anômalos.

Gere um relatório executivo em PDF com: sumário executivo, perfil geral 
das transações, padrões temporais, indicadores de risco, análise geográfica, 
rastreamento de dispositivos/IPs e recomendações estratégicas.
```

**Passo 4 — Interprete o relatório gerado**

O Claude processa o CSV, calcula estatísticas, identifica anomalias e gera o `Relatorio_Analise_Fraude.pdf` com as seguintes seções:

#### Resultados do Relatório Gerado

**Métricas gerais do dataset:**

| Indicador | Valor |
|---|---|
| Total de transações | 2.512 |
| Contas únicas | 495 |
| Período analisado | 02/01/2023 a 01/01/2024 |
| Valor mínimo | R$ 0,26 |
| Valor médio | R$ 297,59 |
| Valor mediano | R$ 211,14 |
| Valor máximo | R$ 1.919,11 |
| Desvio padrão | R$ 291,95 |
| Saldo médio das contas | R$ 5.114,30 |
| Duração média das transações | 119,6 segundos |

**Distribuição por canal:**

| Canal | Participação |
|---|---|
| Agência (Branch) | 34,5% |
| ATM | 33,1% |
| Online | 32,3% |

**Indicadores de risco identificados:**

| Indicador | Quantidade | Percentual | Nível |
|---|---|---|---|
| Transações com 3+ tentativas de login | 95 | 3,8% | 🔴 ALTO |
| Transações que consomem >50% do saldo | 228 | 9,1% | 🔴 ALTO |
| Transações acima do P90 (R$ 701,31) | 252 | 10,0% | 🟡 MÉDIO |
| IPs associados a 10+ contas distintas | 3 IPs | — | 🔴 CRÍTICO |
| Dispositivos vinculados a 7–9 contas | 7 dispositivos | — | 🟡 MÉDIO |

**Padrões temporais:**

| Hora | Volume | Valor médio | Tx. Suspeitas |
|---|---|---|---|
| 16h | 1.316 | R$ 300,48 | 47 |
| 17h | 819 | R$ 301,92 | 31 |
| 18h | 377 | R$ 278,12 | 17 |

> Segunda-feira concentra **42,6%** das transações semanais. Terças-feiras apresentam valor médio superior (R$ 327,56).

**Caso crítico identificado:**

> O IP `200.136.146.93` está associado a **13 contas distintas** — comportamento típico de infraestrutura fraudulenta centralizada. Recomenda-se bloqueio imediato e investigação forense dos acessos originados deste endereço.

**Recomendações estratégicas geradas pelo Claude:**

1. **Sistema de Pontuação de Risco em Tempo Real** — implementar score combinando tentativas de login, razão valor/saldo, histórico de IP e dispositivo.
2. **Autenticação Multifator (MFA)** — exigir segundo fator para transações com 2+ falhas de login ou valor acima do P75.
3. **Monitoramento de Infraestrutura Compartilhada** — alertas automáticos para dispositivos/IPs associados a mais de 3 contas distintas.
4. **Regras de Limite por Sessão** — bloquear transações que consumam mais de 60% do saldo em sessões com comportamento anômalo.
5. **Análise de Velocidade** — monitorar frequência de transações por conta (contas com 12+ transações no período merecem revisão).
6. **Modelo de Machine Learning** — treinar modelo supervisionado usando as variáveis: `LoginAttempts`, `AmountToBalanceRatio`, `Channel`, `DeviceID` e `IP Address`.

#### Resultado esperado

Em minutos, o Claude transforma um CSV bruto em um relatório executivo profissional de 12 páginas — completo com análise estatística, tabelas, identificação de anomalias e recomendações acionáveis — tarefa que normalmente levaria horas de trabalho em Python/Pandas ou ferramentas de BI.

---

## Integrações do Claude

### 8. Diferença entre Cowork e Claude como extensão

Nesta aula é explicada a distinção entre dois modos de uso do Claude:

| Característica | Claude Cowork (Desktop) | Claude como Extensão |
|---|---|---|
| **Acesso a arquivos locais** | ✅ Sim | ❌ Limitado |
| **Integração com apps** | Via MCP (Model Context Protocol) | Via API do navegador/app |
| **Uso típico** | Automações complexas, análise de documentos | Tarefas pontuais em apps específicos |
| **Interface** | App desktop standalone | Extensão/plugin dentro de outro app |
| **Exemplos** | Analisar CSV, revisar contratos | Auxiliar no Excel, criar slides no PowerPoint |

---

### 9. Claude para Excel: principais aplicações

Demonstração de como o Claude integrado ao Excel (via plugin) pode:

- Gerar fórmulas complexas a partir de descrições em linguagem natural
- Analisar dados em planilhas e gerar insights
- Criar tabelas dinâmicas e gráficos automaticamente
- Limpar e transformar dados sujos
- Explicar fórmulas existentes em linguagem simples

---

### 10. Projeto Prático: Dashboard Comercial

#### Objetivo

Usar o Claude para criar um **dashboard comercial interativo** a partir de dados reais de e-commerce, integrando múltiplas tabelas e gerando visualizações de KPIs de negócio.

#### Arquivos utilizados

```
31_claude_dashboard/
├── dataset/
│   ├── monthly_revenue.csv      ← receita mensal (2020–2026)
│   ├── orders.csv               ← histórico de pedidos
│   ├── customers.csv            ← dados de clientes
│   └── product_summary.csv      ← resumo por produto/categoria
└── design-system/
    └── index.html               ← design system de referência visual
```

#### Sobre os Datasets

**`monthly_revenue.csv`** — 75 meses de dados (Jan/2020 a Mar/2026):

| Coluna | Descrição |
|---|---|
| `year`, `month`, `quarter` | Período |
| `orders` | Total de pedidos no mês |
| `revenue_usd` | Receita bruta (USD) |
| `avg_order_value` | Ticket médio |
| `avg_discount_pct` | Desconto médio aplicado (%) |
| `return_rate` | Taxa de devoluções (%) |
| `unique_customers` | Clientes únicos no mês |
| `new_customers` | Novos clientes no mês |

**`orders.csv`** — histórico completo de pedidos com colunas:
`order_id`, `customer_id`, `order_date`, `product_name`, `category`, `unit_price_usd`, `quantity`, `total_amount_usd`, `payment_method`, `device_used`, `delivery_days`, `order_status`, `returned`, `customer_rating`

**`customers.csv`** — perfil de cada cliente com:
`customer_id`, `country`, `age`, `gender`, `membership_tier`, `total_orders`, `total_spend_usd`, `preferred_category`, `preferred_payment_method`, `acquisition_channel`, `churned`

**`product_summary.csv`** — resumo por produto com:
`category`, `product_name`, `total_orders`, `total_revenue_usd`, `avg_price`, `avg_rating`, `return_rate`, `avg_discount_pct`, `avg_delivery_days`

#### Passo a Passo do Projeto

**Passo 1 — Organize a pasta do projeto**

Certifique-se que a estrutura de arquivos está correta com os quatro CSVs na pasta `dataset/` e o arquivo `index.html` do design system na pasta `design-system/`.

**Passo 2 — Conceda acesso ao Cowork**

No Claude Cowork, aponte para a pasta `31_claude_dashboard`. O Claude enxergará os datasets e o design system de referência.

**Passo 3 — Analise os dados antes de construir**

Solicite ao Claude uma exploração inicial:
```
Leia os quatro arquivos CSV na pasta dataset/. 
Descreva a estrutura de cada um, o período de dados disponível,
e sugira os KPIs mais relevantes para um dashboard comercial.
```

**Passo 4 — Referencie o Design System**

Forneça o design system como guia visual:
```
Use o arquivo design-system/index.html como referência de estilos 
(cores, tipografia, componentes) para o dashboard que iremos criar.
```

**Passo 5 — Solicite a construção do dashboard**

Exemplo de prompt para geração do dashboard:
```
Com base nos dados dos quatro CSVs e usando o design system como guia visual,
crie um dashboard comercial em HTML com:

1. KPIs principais: receita total, ticket médio, taxa de novos clientes, taxa de devolução
2. Gráfico de receita mensal (série temporal 2020–2026)
3. Top categorias de produtos por receita
4. Distribuição por canal de pagamento
5. Mapa de calor: receita por mês e ano (comparativo anual)
6. Filtros por ano e quarter
```

**Passo 6 — Itere sobre o resultado**

O Claude gera o arquivo HTML do dashboard. A partir daí, é possível:
- Pedir ajustes visuais ("mude as cores do gráfico para o padrão do design system")
- Adicionar novos gráficos ("adicione um gráfico de retenção de clientes")
- Criar versão para Excel ("exporte este dashboard como planilha com gráficos")

#### Insights esperados dos dados

Com o dataset disponível (2020–2026), alguns insights que o Claude pode destacar:

- **Tendência de crescimento**: receita de ~$35K/mês em 2020 para picos de ~$44K em 2026
- **Sazonalidade**: meses de junho e outubro/novembro consistentemente com maiores receitas
- **Ticket médio**: crescimento de ~$120–130 em 2020 para $140–152 em 2026
- **Aquisição de clientes**: base estável de ~260–310 clientes únicos por mês

#### Resultado esperado

Um dashboard comercial completo e interativo em HTML, pronto para ser aberto no navegador ou integrado a um relatório, gerado automaticamente a partir de arquivos CSV brutos — sem necessidade de ferramentas de BI como Power BI ou Tableau.

---

### 11. Claude para PowerPoint: criando apresentações

Demonstração de como usar o Claude integrado ao PowerPoint para:

- Gerar slides a partir de um texto ou briefing
- Criar estrutura de apresentação (narrativa, fluxo de slides)
- Sugerir layout e design baseado no conteúdo
- Converter relatórios em apresentações executivas

---

### 12. Claude como extensão do Google Chrome

Nesta aula é apresentado o **Claude como extensão do Chrome**, que permite:

- Resumir páginas web com um clique
- Fazer perguntas sobre o conteúdo da página atual
- Extrair informações de sites (tabelas, listas, dados)
- Redigir e-mails e formulários diretamente no navegador
- Pesquisar e sintetizar informações de múltiplas páginas

**Diferença chave:** enquanto o Cowork trabalha com arquivos locais, a extensão do Chrome trabalha com o conteúdo da web em tempo real, tornando-os complementares.

---

## Conclusão

O curso cobre um espectro completo de automação com Claude: desde a instalação e primeiros passos, passando por projetos práticos com contratos, análise de fraude e dashboards comerciais, até integrações com as ferramentas do dia a dia (Excel, PowerPoint, Chrome). A proposta central é que qualquer profissional — independente de background técnico — consiga multiplicar sua produtividade usando IA de forma prática e imediata.
