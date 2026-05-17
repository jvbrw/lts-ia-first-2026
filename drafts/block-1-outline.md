# Bloco 1: O Que Aprendemos Construindo Produto com IA em 2025
**Apresentador: JV**
**Duração: ~30 minutos**

---

## Objetivo

Compartilhar aprendizados práticos de quem construiu um produto que desenvolve produtos com IA. Responder à pergunta central:

> "O que 2025 nos ensinou, na prática, sobre desenvolver produto com IA no centro do processo?"

---

## Estrutura

### 1. Abertura: A realidade dos números (3min)
- **Setup do contexto global**: 88.3% de adoção vs 32.7% de aceitação de PRs de IA (LinearB 2026)
- **O paradoxo**: Todo mundo usando, poucos obtendo resultado
- **Nossa tese**: A ferramenta não é o problema. É como você estrutura o trabalho ao redor dela
- **💬 Interação**: "Aquela situação: usamos IA para fazer várias coisas do fluxo - e que foram mais rápidas - mas depois a gente viu que o tempo que ganhamos na hora de fazer agora estamos gastando na hora de revisar"

### 2. O desafio que nos levou a construir o AI Framework (4min)
- **Contexto BossaBox**: Empresa que desenvolve produtos para múltiplos clientes
- **O problema real**: Como incorporar o uso de IA em nossos projetos manter qualidade e velocidade com IA em nossos projetos?
- **4 problemas práticos que enfrentamos**:
  - Backlog represado (capacidade limitada)
  - Inconsistência (cada dev documenta diferente)
  - Contexto perdido (re-explicar tudo a cada interação com IA)
  - Desperdício de tempo (tarefas manuais vs descobrir valor)
- **A decisão**: Construir um framework próprio, não só usar ferramentas de IA genéricas

### 3. AI Framework: O que construímos (8min)
- **Definição**: Sistema de agentes especializados que amplifica produtividade em cada etapa do ciclo
- **5 capabilities integradas**:
  - **Context** → Levantamento estruturado (produto, processos, tech stack)
  - **Planning** → Decompõe iniciativa em user stories acionáveis
  - **Refinement** → Transforma stories em tarefas técnicas (BE/FE)
  - **Implementation** → Gera código com TDD, cria testes, prepara PRs
  - **QA Agent** → Cria cenários de teste e automações E2E
- **Principais features**:
  - Brownfield awareness (funciona também em produtos existentes)
  - Human-in-the-loop (validação humana entre etapas)
  - Spec-Driven Development (especificação primeiro, código depois)
  - No prompt engineering (contexto flui automaticamente)
- **Fluxo prático**: /initiative-start → /refine-tasks → /implement → /test
- **💬 Interação**: "Alguém já tentou algo parecido? Já usou algum produto que se propõe a fazer a mesma coisa?"

### 4. Casos reais: O que funcionou na prática (10min)

**Case 1: Squad enxuto, ciclo completo**
- **Desafio**: PM + 1 SWE executando framework completo
- **Feature**: Validação automatizada de CNPJ (média complexidade)
- **Resultado**: 4 user stories implementadas, 100% do workflow com IA
- **Métricas**: 3.3/4 output quality, 4/4 workflow usability, 3.6/4 speed
- **Aprendizado**: "Estamos confiantes como squad enxuto fazendo entregas end-to-end mantendo ou até superando as métricas anteriores de performance"

**Case 2: Velocidade em feature complexa**
- **Desafio**: Feature de alta complexidade mantendo eficiência
- **Solução**: Aproveitar código existente como referência (mostrando como as coisas boas se parecem)
- **Resultado**: Feature complexa em produção em menos de uma semana, operação estável confirmada
- **Métricas**: 4/4 speed execution (velocidade máxima mesmo com complexidade)
- **Aprendizado**: Framework mantém eficiência em cenários de alta complexidade, desde que tenha uma boa especificação e direção por parte dos orquestradores

**Case 3: Colaboração PM + TL com IA**
- **Desafio**: Geração eficiente de tarefas técnicas
- **Solução**: PM criando user stories com agentes + sub-agente customizado para code audit e refinamento técnico
- **Resultado**: O tempo gasto na geração de tarefas caiu pela metade, levando o time a ser mais estratégico
- **Métricas**: 3.3/4 output quality, 4/4 speed execution, 4 user stories
- **Inovação**: Primeiro sub-agente customizado
- **Aprendizado**: Colaboração humano-IA criando valor 

### 5. 3 Princípios que validamos (4min)

**Princípio 1: Context Engineering é a nova core skill**
- Contexto estruturado vs ad-hoc mostra diferença enorme de qualidade
- Warmup (carregar contexto uma vez) vs repetir tudo a cada prompt
- Repository + reference examples = output consistente
- **Evidência**: Diferença entre 32.7% e 80%+ de aceitação está no contexto

**Princípio 2: Responsabilidade aumenta, não diminui**
- IA não reduz carga cognitiva, redistribui
- De "escrever código" para "validar código + arquitetar contexto"
- Ownership se torna mais crítico (quem é dono do output de IA?)
- **Evidência**: PRs de IA são 2.6x maiores e levam 5.3x mais tempo de review (LinearB)

**Princípio 3: Conhecimento técnico (produto ou engenharia) permanece fundamental e necessário**
- Entender arquitetura é necessário para prompting efetivo
- Inglês vira "linguagem de programação" mas profundidade técnica é mandatória 
- Não é substituição, é amplificação de quem já sabe
- **Evidência**: Times com melhor performance técnica têm melhores resultados com IA

**💬 Interação**: "Qual desses 3 princípios está mais presente no dia a dia de vocês?"

### 6. Conexão com tendências de 2026 (1min)
- **O que estamos vendo**: Adoção ampla de AI Agents como colaboradores (OpenAI Enterprise 2025)
- **Shift de papel**: Desenvolvedores e pessoas de produto virando curadores/orquestradores (não só implementadores)
- **IA como infraestrutura**: Não é experimento, é parte do produto (31.8% redução em tempo de review) que precisa de um fluxo de trabalho adequado
- **Análise Anthropic**: 500k+ interações mostram que automação domina sobre assistência (casos de uso de IA em automações)
- **Implicação**: Isso exige redesenho de times, preocupação com o fluxo de trabalho e não só adoção de ferramentas

### 7. Transição para Bloco 2 (1min)
- **O que mostramos**: Estrutura de trabalho (AI Framework) funciona quando bem desenhada, levando em consideração toda a fábrica de desenvolvimento de produto
- **O que falta responder**: Como redesenhar times para operar dessa forma?
- **Setup**: Bassan vai abordar o que isso exige de liderança e desenho organizacional em 2026 

---

## Pontos-Chave a Enfatizar

1. **Casos reais, não teoria** - 4 projetos diferentes (Cubo, Piwi, Enforce, BossaBox) com contextos e desafios únicos
2. **Números que importam** - De 32.7% para 80%+ aceitação, média 3.5/4.0 em todas métricas, ~2 dias economizados por sprint
3. **Problemas concretos resolvidos** - Backlog represado, inconsistência, contexto perdido, desperdício de tempo
4. **Context engineering como diferencial** - Brownfield awareness, warmup, spec-driven, human-in-the-loop
5. **Validação externa** - LinearB 2026 confirma: adoção alta ≠ resultado alto, contexto é o gargalo
6. **Desenvolvemos o que pregamos** - AI Framework é produto interno em uso real, não slide

---

## Conexões com Referências Estratégicas (para preparar Bloco 2)

**OpenAI Enterprise 2025**:
- Uso corporativo cresceu substancialmente em fluxos multi-etapa
- Nossa evidência: AI Framework valida isso com casos reais em produção

**Anthropic Research - Software Development Impact**:
- 500k+ interações mostram automação dominando sobre assistência
- Nossa evidência: Cases mostram automação de workflows completos (PM → QA)

**GitHub Octoverse 2025**:
- Nova identidade do desenvolvedor na era AI
- Nossa evidência: Papel de PM, TL e Dev mudou nos 4 casos (curador/orquestrador)

**Redução tempo de review (31.8%)**:
- Paper 2025 sobre ganhos de produtividade com IA bem integrada
- Nossa evidência: De 32.7% para 80%+ quando contexto é estruturado

---

## Materiais de Apoio

**Documentos internos**:
- Cases AI Framework PDF (10 slides com métricas detalhadas)
- AI Framework PDF (8 slides explicando capabilities e features)
- Demos em vídeo dos 4 agentes

**Dados externos**:
- LinearB 2026 Software Engineering Benchmarks Report
- OpenAI State of Enterprise AI 2025
- Anthropic Research (Impact on Software Development)
- GitHub Octoverse 2025

---

## Oportunidades de Evolução (mencionar rapidamente)

Aprendemos também com o que **não** funcionou perfeitamente:
1. **Agente QA**: Bugs não detectados geraram tarefas extras (já melhorado)
2. **Frameworks legados**: Agentes tentavam código moderno em Vue 2 (resolvido com warmup de versão)
3. **Padrões de plataforma**: Nem sempre seguidos automaticamente (adicionados ao warmup + checklist)

→ Transparência sobre desafios reforça credibilidade e mostra processo de melhoria contínua

---

## Notas de Apresentação

**Tom e abordagem**:
- Tom conversacional e prático: "o que descobrimos fazendo"
- Usar "nós" e "nossa experiência" - é trabalho de time
- Ser direto sobre desafios enfrentados (oportunidades de evolução)
- Cases são protagonistas, não conceitos abstratos

**Ritmo e interação**:
- Abrir cada seção com pergunta para audiência
- Não se apressar nos cases - são a substância da apresentação
- Pausar para perguntas após AI Framework e após os 3 Princípios
- Conectar cada case com um aprendizado específico

**Transição para Bloco 2**:
- Deixar claro: "Mostramos que funciona quando estruturado"
- Setup natural: "Mas como redesenhar times para operar assim?"
- Bassan pega daqui para falar de liderança e organização

**Mensagem de encerramento do Bloco 1**:
> "Construímos produto com IA no centro. Funciona. Mas não é mágica - é estrutura, disciplina e contexto bem arquitetado. E isso tem implicações profundas para como times devem ser desenhados."
