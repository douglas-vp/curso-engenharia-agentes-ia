# Criando seu Primeiro Agente de IA

> Cobrindo desde os fundamentos até exemplos práticos com agentes reais.

---

## Sumário

1. [O que é um Agente de IA?](#o-que-é-um-agente-de-ia)
2. [Os 7 Pilares de um Bom Prompt](#os-7-pilares-de-um-bom-prompt)
3. [Criando seu Primeiro Agente (passo a passo)](#criando-seu-primeiro-agente-passo-a-passo)
4. [Engenharia de Prompt Avançada](#engenharia-de-prompt-avançada)
5. [Exemplos Práticos de Agentes Reais](#exemplos-práticos-de-agentes-reais)
6. [Erros Comuns e Como Evitá-los](#erros-comuns-e-como-evitá-los)
7. [Recursos Adicionais](#recursos-adicionais)

---

## O que é um Agente de IA?

Um **Agente de IA** é uma instância de um modelo de linguagem (como o ChatGPT) configurada com um conjunto de instruções personalizadas para se comportar de uma forma específica — como se fosse um profissional especializado que você contratou para uma função.

Ao invés de fazer perguntas genéricas para a IA, você define:

- **Quem ela é** (papel/persona)
- **Como ela se comunica** (tom)
- **O que ela deve fazer** (instruções)
- **Qual o resultado esperado** (saída)

Isso transforma uma ferramenta genérica em um colaborador especializado.

---

## Os 7 Pilares de um Bom Prompt

Todo agente bem construído é sustentado por estes elementos:

| # | Elemento | Descrição |
|---|----------|-----------|
| 1 | **PAPEL** | Quem é a IA? Qual a sua especialização? |
| 2 | **TOM** | Como ela deve se comunicar? (formal, casual, técnico...) |
| 3 | **INSTRUÇÕES** | O que ela deve fazer, passo a passo |
| 4 | **SER ESPECÍFICO** | Quanto mais detalhado, melhor o resultado |
| 5 | **SER REPETITIVO COM ASPECTOS CRUCIAIS** | Reforce as regras mais importantes |
| 6 | **SAÍDA ESPERADA** | Como deve ser o formato e conteúdo da resposta |
| 7 | **EXEMPLOS** | Demonstre o que você espera com amostras reais |

> 💡 **Dica:** A qualidade do seu agente é diretamente proporcional à qualidade do seu prompt. Um prompt vago gera respostas vagas.

---

## Criando seu Primeiro Agente (passo a passo)

### Passo 1 — Defina o Papel

Comece dizendo explicitamente **quem é** a IA. Seja específico sobre a área de atuação e o nível de expertise.

```
❌ Fraco:
"Você é um assistente de marketing."

✅ Forte:
"Você é um copywriter sênior com 10 anos de experiência,
especializado na criação de Reels para criadores de conteúdo
de fitness no Instagram."
```

---

### Passo 2 — Defina o Tom

O tom determina a personalidade da comunicação. Pense no público-alvo do seu agente.

```
Exemplos de tons:
- "Use uma linguagem técnica e objetiva, sem rodeios."
- "Seja entusiasta e motivacional, como um personal trainer."
- "Adote um tom acadêmico, citando fontes sempre que possível."
- "Escreva de forma casual e descontraída, como se fosse uma conversa entre amigos."
```

---

### Passo 3 — Escreva as Instruções

Aqui você define o **fluxo de trabalho** do seu agente. Use uma sequência numerada quando houver etapas a seguir.

```
Quando solicitado a escrever um roteiro, siga esta ordem:

1. Pesquise na internet fatos curiosos sobre o tema.
2. Apresente um relatório para o usuário e aguarde aprovação.
3. Sugira no mínimo 10 hooks diferentes.
4. Com base no hook escolhido, escreva o roteiro final.
```

---

### Passo 4 — Defina a Saída Esperada

Especifique o **formato**, o **tamanho** e o **estilo** da resposta.

```
O relatório deve:
- Ter entre 150 e 250 palavras
- Ser formatado em Markdown
- Incluir links de referência para cada informação
- Ter no mínimo 10 sugestões de hooks
```

---

### Passo 5 — Adicione Exemplos

Exemplos são o ingrediente mais poderoso de qualquer prompt. Eles mostram na prática o que palavras muitas vezes não conseguem descrever.

```
Abaixo estão 3 exemplos do estilo de escrita que você deve imitar:

[EXEMPLO 1]
"The calves are the hardest muscle to grow.
But scientists have recently discovered three solutions..."

[EXEMPLO 2]
"Your triceps will never reach their full potential
if you only do these exercises..."
```

---

## Engenharia de Prompt Avançada

### Repetição Estratégica

Para regras críticas que o agente não pode ignorar, **repita-as em diferentes partes do prompt**. Isso aumenta o peso daquela instrução no processamento.

```
[No início do prompt]
"Nunca invente informações. Sempre cite fontes."

[No meio, nas instruções de pesquisa]
"IMPORTANTE: Inclua os links de referência junto de cada informação."

[No final, no formato de saída]
"Lembre-se: seu relatório DEVE conter referências com links para cada fato."
```

---

### Checkpoints de Aprovação

Para tarefas complexas com múltiplas etapas, instrua o agente a **pausar e aguardar aprovação** antes de avançar. Isso evita retrabalho.

```
"Apresente seu relatório para o usuário e verifique por possíveis
alterações ANTES de avançar para a próxima etapa."
```

---

### Restrições Negativas

Dizer o que o agente **não deve fazer** é tão importante quanto dizer o que ele deve.

```
Exemplos de restrições:
- "Evite informações óbvias. Foque em fatos curiosos e contraintuitivos."
- "Não use linguagem de propaganda ou tom publicitário."
- "Não gere imagens com estilo de estúdio fotográfico ou CGI."
- "Evite poses exageradas ou voltadas diretamente para a câmera."
```

---

## Exemplos Práticos de Agentes Reais

### Agente 1 — Copywriter (estilo Jeff Nippard)

**Objetivo:** Criar roteiros de Reels de fitness imitando o estilo de um criador específico.

**Prompt completo:**

```
PAPEL:
Você é um copywriter sênior, especializado na criação de Reels
modelando um criador de conteúdo chamado Jeff Nippard.

TOM:
Seus roteiros combinam frases curtas e impactantes com explicações
científicas. Linguagem acessível, mas baseada em evidências.

INSTRUÇÕES:
1. Ao receber um tema, pesquise na web fatos curiosos e dados
   científicos sobre o assunto.
2. Apresente um relatório em Markdown com referências e links.
   Aguarde aprovação antes de continuar.
3. Sugira no mínimo 10 hooks diferentes para o Reels.
4. Com base no hook escolhido, escreva o roteiro final.

SAÍDA ESPERADA:
- Roteiro entre 150 e 250 palavras
- Imite o comprimento das frases do Jeff Nippard
- Use o vocabulário e tom dele
- Baseie-se apenas em informações verificadas

EXEMPLOS DE HOOKS:
- "What's the least amount of work you can do and still make gains?"
- "The calves are the hardest muscle to grow."
- "Your triceps will never reach their full potential if you only
  do these exercises."

EXEMPLO DE ROTEIRO:
He always trains his calves using a full range of motion.
And he only does the top half.
Who do you think will grow bigger calves? Well, a new study tested this.
[...]
```

---

### Agente 2 — Fotógrafo UGC (User Generated Content)

**Objetivo:** Gerar prompts para imagens realistas de produtos em contextos cotidianos.

**Prompt completo:**

```
PAPEL:
Você é um fotógrafo profissional de produtos lifestyle,
especializado em imagens UGC (User Generated Content)
ultra-realistas.

TOM:
Técnico e detalhado. Cada instrução deve maximizar o realismo
e evitar qualquer aparência artificial ou publicitária.

INSTRUÇÕES:
Dado uma imagem de produto, gere uma foto realista de uma pessoa
usando o produto naturalmente no cotidiano.

CÂMERA E ESTILO:
- Simule fotografia com smartphone (iPhone 14 Pro, Samsung Galaxy S23)
- Lente equivalente a 24mm, perspectiva levemente ampla
- Profundidade de campo natural, leve desfoque de movimento ocasional
- Textura natural de pele, detalhes reais de tecido e superfície

AMBIENTES:
- Residenciais: cozinha, sala com sofá, quarto, home office
- Ao ar livre: café na rua, parque, calçada, praça
- Objetos de cena: xícaras, livros, laptops, plantas, notebooks

ATORES:
- Pessoas comuns, não modelos
- Textura de pele natural, pequenas imperfeições
- Etnias diversas, roupas casuais (camiseta, jeans, moletom)
- Expressões espontâneas: rindo, concentrado, caminhando

RESTRIÇÕES:
❌ Nunca: iluminação de estúdio, produto centralizado perfeitamente,
   look CGI, poses promocionais exageradas
✅ Sempre: enquadramento levemente torto, foco impreciso sutil,
   objetos parcialmente cortados, mãos cobrindo partes do produto
```

---

### Estrutura Visual Comparativa

```
PROMPT FRACO                    PROMPT FORTE
─────────────────               ──────────────────────────────────
"Você é um fotógrafo"    →      "Você é fotógrafo profissional de
                                 lifestyle UGC, especializado em
                                 simular fotos de smartphone com
                                 imperfeições naturais..."

"Faça uma foto realista" →      "Simule iPhone 14 Pro, lente 24mm,
                                 luz de janela de apartamento,
                                 grão sutil, enquadramento levemente
                                 torto, pele com textura real..."

"Não use estúdio"        →      "❌ Evite: iluminação de estúdio,
                                 produto centralizado, look HDR,
                                 poses diretamente para câmera,
                                 maquiagem de modelo"
```

---

## Erros Comuns e Como Evitá-los

### ❌ Erro 1: Ser vago no papel

```
Errado:  "Você é um especialista em marketing."
Certo:   "Você é um estrategista de conteúdo para Instagram,
          com foco em criadores de fitness com 50k–500k seguidores."
```

---

### ❌ Erro 2: Não dar exemplos

Sem exemplos, a IA interpreta as instruções à sua maneira. Com exemplos, ela tem um modelo concreto para seguir.

---

### ❌ Erro 3: Não definir restrições

Dizer apenas o que quer não é suficiente. Diga também o que você **não** quer.

---

### ❌ Erro 4: Esquecer o formato da saída

Se você não especificar o formato, a IA escolherá por conta própria — e raramente será o formato ideal para o seu caso de uso.

---

### ❌ Erro 5: Não iterar

Agentes raramente ficam perfeitos na primeira versão. Teste, observe onde ele erra, e refine as instruções com base nos resultados reais.

---

## Recursos Adicionais

- 📖 **Prompt Engineering Guide** (com versão em português):  
  [https://www.promptingguide.ai/pt](https://www.promptingguide.ai/pt)  
  Uma das referências mais completas sobre engenharia de prompts disponíveis gratuitamente.

- 🔁 **Quando um agente não se comportar como esperado:**  
  Consulte o guia acima e revise os 7 pilares desta documentação. Na maioria dos casos, o problema está na falta de especificidade ou na ausência de exemplos.

---

> **Resumo rápido:** Um bom agente de IA = Papel claro + Tom definido + Instruções detalhadas + Restrições explícitas + Exemplos concretos + Formato de saída especificado.  
> Quanto mais você investe no prompt, menos retrabalho você terá nos resultados.