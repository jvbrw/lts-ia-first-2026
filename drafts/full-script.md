# Desenvolvimento de Produto IA-First: O Que Muda no Desenho dos Times
*Leading Tech Sessions - BossaBox*

---

## Abertura (JV - 2min)

**"Antes de começar, uma pergunta rápida: quem aqui já ouviu que IA vai aumentar 10x a produtividade do time - e depois viu o resultado não bater com a expectativa? Manda um 'sim' no chat!"**

### O contexto de 2026

- **Adoção explodiu**: de 71.6% para 88.3% de times usando IA no último ano (LinearB 2026)
- **Mas os resultados não seguiram**: PRs gerados por IA têm 2.6x mais linhas e demoram 5.3x mais para serem revisados
- **A taxa de aceitação conta a história**: 32.7% para PRs com IA vs 84.4% para PRs manuais
- **45% das empresas não medem impacto de IA** - operam no escuro

> "A ferramenta não é o mais importante. É como a empresa se organiza para usar as ferramentas disponíveis."

**Hoje vamos compartilhar o que aprendemos na prática em 2025 e o que isso exige de quem lidera times de produto e tecnologia em 2026.**

---

# BLOCO 1: O Que Aprendemos Construindo Produto com IA em 2025
**Apresentador: JV**
**Duração: ~30 minutos**

---

## 1.1 Onde IA Funcionou Bem (e Por Quê)

### O padrão que identificamos: IA funciona quando há contexto estruturado e lógica de captura de valor em cada etapa

> IA como fluxo de trabalho ao invés de trabalho atomizado

**Casos que deram certo:**

#### Caso 1: POCs de viabilidade técnica
- **Situação**: Feature complexa com incerteza técnica alta
- **Com IA**: POC em 2-3 dias identificou limitação antes de 2 meses de desenvolvimento
- **Por que funcionou**: Escopo limitado, feedback rápido, decisão binária (viável/inviável)
- **O padrão**: Contexto claro + critério de sucesso definido + ciclo curto de feedback

#### Caso 2: Features de baixa-média complexidade
- **Situação**: Implementação de features com escopo bem definido
- **Com IA**: Ciclo completo (spec → refinement → implementação → QA) com IA em cada etapa
- **Por que funcionou**: Cada etapa alimenta a próxima com contexto estruturado
- **O padrão**: IA como fluxo contínuo, não como ferramenta pontual

**💬 "Onde funcionou pra vocês? Mandem no chat um caso."**

---

## 1.2 Onde IA Quebrou Expectativas (e Por Quê)

### O anti-padrão: "delegar sem estrutura"

**Casos que não deram certo:**

#### Caso 1: "Cria uma feature pra mim"
- **O que aconteceu**: PM delegou criação de spec inteira para IA sem contexto estruturado
- **Resultado**: Feature foi desenvolvida, ninguém usou - e nem validou se fazia sentido
- **Aprendizado**: IA amplifica decisões - boas e ruins

#### Caso 2: O problema do AI PR na prática
- **O que aconteceu**: Dev usou IA para gerar código sem contexto do sistema
- **Resultado**: PR 3x maior que necessário, 5x mais tempo de review, overwork no time
- **Dados do mercado**: 32.7% de aceitação de AI PRs vs 84.4% manuais (LinearB 2026)
- **Aprendizado**: **Contexto é o gargalo**, não a capacidade de geração

#### Caso 3: Excesso de agentes sem clareza de valor
- **O que aconteceu**: Time criou múltiplos agentes de IA para automatizar tudo
- **Resultado**: Mais complexidade, mais manutenção, ROI negativo
- **Aprendizado**: IA por conveniência ≠ IA com valor claro

**💬 "Alguém já passou por situação parecida? Onde a expectativa não bateu com realidade?"**

---

## 1.3 O Framework que Desenvolvemos: AI Framework

### Nossa resposta prática para os problemas que encontramos

**O que é**: Framework de agentes especializados que automatizam o ciclo de desenvolvimento de produto

**Por que criamos**: Precisávamos estruturar o contexto de forma que IA pudesse operar com consistência

### As 5 capabilities principais

| Role | O que faz | Por que importa |
|------|-----------|-----------------|
| **Product Management** | PRDs, User Stories, refinamento | Garante contexto de negócio estruturado |
| **Tech Lead** | Specs técnicas, decisões arquiteturais | Conecta visão de produto com realidade técnica |
| **Software Engineering** | Implementação baseada em tasks refinadas | Executa com contexto completo |
| **QA** | Test cases E2E, validação | Fecha o loop de qualidade |
| **Refinement** | Quebra US em tasks técnicas | Garante granularidade adequada |

### O fluxo na prática

```
1. /initiative-start → Classifica iniciativa + gera User Stories
2. /refinement → Quebra US em tasks técnicas (DoR)
3. /implement → Implementa com TDAID (Test-Driven AI Development)
4. /qa-test → Valida implementação
```

### TDAID: Test-Driven AI Development

**O insight**: Se IA vai gerar código, ela precisa de critérios claros de sucesso

1. **Planning**: Analisa plano e define estrutura
2. **Red**: Escreve testes ANTES do código (devem falhar)
3. **Green**: Implementa código para testes passarem
4. **Validate**: Executa validações de qualidade

**Resultado**: Saímos de 32% de aceitação para +80% em PRs gerados pelo framework

**💬 "Isso faz sentido? Mandem dúvidas no chat sobre como estruturamos o framework."**

---

## 1.4 Os 3 Princípios que Validamos em 2025

### Princípio 1: Context Engineering é a Nova Core Skill

> "IA só é boa quanto o contexto que você dá"

**Na prática significa:**
- Product Spec não é mais "nice to have" - é infraestrutura crítica
- Documentação técnica vira input, não output
- Quem domina contexto, domina o resultado

**Exemplo concreto**: Nosso Product Spec estruturado reduziu retrabalho em PRDs em 80%

### Princípio 2: Human-in-the-Loop Muda de Lugar, Não Desaparece

> "A responsabilidade aumenta, não diminui"

**O shift:**
- **De**: Humano executa, IA assiste
- **Para**: IA executa, humano valida e orquestra

**Implicação**: PM que "só valida" sem entender o que está validando cria mais problemas

### Princípio 3: Repertório Importa Mais que Prompt

> "Show it what great looks like"

**O que descobrimos:**
- Biblioteca de 50 specs exemplares > prompt genérico
- IA aprende com seus melhores exemplos, não com documentação abstrata
- Tempo investido em curadoria tem retorno exponencial

**💬 "Qual desses princípios ressoa mais com a realidade de vocês? Mandem no chat."**

---

## 1.5 Dados de Mercado: O Contexto de 2026

### O estado atual (LinearB 2026 Benchmarks)

| Métrica | Valor | Implicação |
|---------|-------|------------|
| Adoção de IA em times | 88.3% | Todos estão usando |
| Taxa de aceitação AI PRs | 32.7% | Mas resultados são ruins |
| Taxa de aceitação PRs manuais | 84.4% | Gap de 2.5x |
| Empresas sem métricas de IA | 45% | Operando no escuro |
| Maior barreira para AI PRs | Contexto | Não é a ferramenta |

### O que os dados mostram

1. **Adoção alta ≠ resultado alto** - O gap entre usar e usar bem é enorme
2. **Contexto é o gargalo** - Não falta capacidade de geração, falta estrutura
3. **Medição é rara** - Maioria não sabe se IA está ajudando ou atrapalhando

**💬 "Vocês medem o impacto de IA no time? Mandem 'sim' ou 'não' no chat."**

---

## Transição para Bloco 2

**"O que esses aprendizados nos mostram é que a ferramenta não é o mais importante. O que importa é como a empresa se organiza para usar as ferramentas disponíveis.**

**No próximo bloco, o Bassan vai explorar o que isso exige de quem lidera times em 2026 - como redesenhar ownership, responsabilidades e contexto."**

---

# BLOCO 2: O Que Esses Aprendizados Exigem do Desenho dos Times em 2026
**Apresentador: Gustavo Bassan**
**Duração: ~30 minutos**

---

## 2.1 O Shift Fundamental: De Systems of Record para Systems of Intelligence

### O modelo mental que precisa mudar

**Systems of Record (SOR)** - Como software funcionou por 40 anos:
- Dashboards estáticos
- UIs rígidas
- Human-in-the-loop em tudo
- Software que informa, não age

**Systems of Intelligence (SOI)** - O que 2026 exige:
- Inteligência em tempo real
- Plataformas headless com interação multi-modal
- Human-on-the-loop (supervisão, não execução)
- Software que age autonomamente

| De (SOR) | Para (SOI) |
|----------|------------|
| Dashboards estáticos | Inteligência em tempo real |
| Human-in-the-loop | Human-on-the-loop |
| Human middleware | Autonomous outcomes |
| Software não-inteligente | AI agent colleagues com memória |

**💬 "Onde o time de vocês está nessa transição? SOR ou já caminhando para SOI?"**

---

## 2.2 Redesenhando Ownership em Times IA-First

### O problema: Ownership tradicional não funciona com IA

**Modelo tradicional:**
- PM é dono do "quê"
- Tech Lead é dono do "como"
- Dev é dono da execução
- Linhas claras, handoffs definidos

**O que IA quebra:**
- Quem é "dono" de um output gerado por IA?
- Quem valida se o contexto estava certo?
- Quem é responsável quando IA amplifica um erro de premissa?

### O novo modelo: Ownership de Contexto + Outcome

**3 novas responsabilidades que não existiam:**

#### 1. Context Owner
- **Quem**: Geralmente PM ou Tech Lead
- **O quê**: Garantir que IA tem informação suficiente para operar
- **Métrica**: Qualidade do input → Qualidade do output

#### 2. Validation Owner
- **Quem**: Quem tem expertise no domínio (varia por contexto)
- **O quê**: Validar outputs antes de virarem decisões
- **Métrica**: Taxa de aceitação, tempo de review

#### 3. Feedback Owner
- **Quem**: Pode ser distribuído
- **O quê**: Capturar aprendizados e melhorar o sistema
- **Métrica**: Evolução da qualidade ao longo do tempo

**💬 "Como ownership funciona no time de vocês hoje? Mandem no chat."**

---

## 2.3 Context Engineering como Disciplina

### Por que contexto virou disciplina, não tarefa

**O insight do JV no Bloco 1**: Taxa de aceitação de AI PRs é 32.7% vs 84.4% manual.

**A causa raiz**: Falta de contexto estruturado, não falta de capacidade de IA.

### O que significa tratar contexto como disciplina

#### 1. Product Spec como Infraestrutura

**Antes**: Documento opcional, "nice to have"
**Agora**: Pré-requisito para qualquer geração de IA

**Estrutura que funciona:**
- Problema de negócio (não solução)
- Constraints técnicas conhecidas
- Exemplos de sucesso (repertório)
- Critérios de validação claros

#### 2. Warmup como Prática Padrão

**O que é**: Processo de carregar contexto antes de pedir output

**Exemplo do AI Framework:**
- `warmup-tech.md` - Contexto técnico do projeto
- `warmup-project.md` - Contexto de negócio
- Carregados antes de qualquer comando

**Resultado**: IA não "adivinha" - ela opera com informação real

#### 3. Documentação como Input, Não Output

**Shift de mindset:**
- **Antes**: Documentamos depois de fazer
- **Agora**: Documentamos para IA poder fazer

**Implicação prática**: Qualidade da documentação vira gargalo de produtividade

**💬 "Vocês tratam documentação como input ou output? Mandem no chat."**

---

## 2.4 Evitando IA por Conveniência

### O anti-padrão mais comum em 2025

**Sintomas:**
- "Vamos criar um agente pra isso"
- "IA pode fazer isso mais rápido"
- "Todo mundo está usando"

**O problema**: IA sem clareza de valor = complexidade sem retorno

### Framework de decisão: Quando usar IA

| Critério | Usar IA | Não usar IA |
|----------|---------|-------------|
| Contexto disponível? | Estruturado e acessível | Implícito ou disperso |
| Critério de sucesso? | Claro e mensurável | Subjetivo ou vago |
| Volume/Escala? | Alto ou repetitivo | Único ou raro |
| Expertise necessária? | Pode ser validada | Requer julgamento profundo |

### Perguntas antes de implementar IA

1. **Qual o valor esperado?** (não "seria legal", mas ROI concreto)
2. **Quem vai validar o output?** (e essa pessoa tem tempo/skill)
3. **Como vamos medir sucesso?** (45% das empresas não medem)
4. **O contexto existe?** (ou precisa ser criado primeiro)

**💬 "Vocês têm framework de decisão para quando usar IA? Mandem no chat."**

---

## 2.5 O Papel do Líder em Times IA-First

### O que muda para heads, leads e managers

#### 1. De Executor para Orquestrador

**Antes**: Líder que "entrega" é o que produz mais
**Agora**: Líder que "entrega" é o que habilita o sistema a produzir

**Na prática:**
- Menos tempo em execução direta
- Mais tempo em context engineering
- Mais tempo em validação e feedback

#### 2. De Especialista para Arquiteto de Contexto

**Antes**: Expertise = saber fazer
**Agora**: Expertise = saber estruturar para IA fazer

**Implicação**: Conhecimento tácito precisa virar explícito

#### 3. De Gerente de Pessoas para Gerente de Sistema

**Antes**: Performance = output individual
**Agora**: Performance = output do sistema (humano + IA)

**Métricas que importam:**
- Qualidade do contexto (input)
- Taxa de aceitação (throughput)
- Evolução ao longo do tempo (learning)

**💬 "Como o papel de vocês como líderes mudou com IA? Mandem no chat."**

---

## 2.6 O Que Não Pode Mais Ser Adiado em 2026

### 3 decisões que líderes precisam tomar agora

#### Decisão 1: Definir ownership de contexto

**Pergunta**: Quem é responsável por garantir que IA tem informação suficiente?

**Se não decidir**: Times vão operar com contexto fragmentado, resultados inconsistentes

#### Decisão 2: Estabelecer métricas de IA

**Pergunta**: Como vocês vão saber se IA está ajudando ou atrapalhando?

**Se não decidir**: Vão fazer parte dos 45% que não medem (e não sabem se vale a pena)

#### Decisão 3: Investir em context engineering

**Pergunta**: Documentação, specs, warmups são prioridade ou "quando der"?

**Se não decidir**: Vão continuar no gap de 32% vs 84% de aceitação

**💬 "Qual dessas decisões é mais urgente pra vocês? Mandem no chat."**

---

## Encerramento (Bassan + JV - 5min)

### Principais Takeaways

**Do Bloco 1 (JV):**
1. **Adoção alta ≠ resultado alto** - 88% usam IA, 32% dos outputs são aceitos
2. **Contexto é o gargalo** - Não falta capacidade de geração, falta estrutura
3. **Framework > Ferramenta** - AI Framework mostrou que estrutura muda resultado

**Do Bloco 2 (Bassan):**
1. **Ownership precisa ser redesenhado** - Context, Validation, Feedback Owners
2. **Context Engineering é disciplina** - Product Spec vira infraestrutura crítica
3. **Líderes viram arquitetos de sistema** - De executores para orquestradores

### O que fazer segunda-feira

1. **Mapeie**: Onde IA está funcionando vs onde está gerando atrito no seu time?
2. **Defina**: Quem é responsável por contexto, validação e feedback hoje?
3. **Meça**: Qual a taxa de aceitação dos outputs de IA no seu time?
4. **Priorize**: Context engineering é investimento, não custo

**💬 "Mandem no chat uma palavra que resume o que vocês levam dessa conversa!"**

---

## Q&A (5-10min)

**"Vamos abrir para perguntas. Podem mandar no chat ou levantar a mão."**

*Sugestões de tópicos para preparar respostas:*
- Como começar com AI Framework em times menores
- Métricas específicas para medir impacto de IA
- Como convencer stakeholders a investir em context engineering
- Diferença entre IA para produtividade vs IA no produto

---

## Encerramento

### Recursos

- **Gravação e slides**: Vão para o email de vocês
- **Dúvidas**: Podem mandar por LinkedIn
- **AI Framework**: [Se quiserem compartilhar publicamente - confirmar]

**"Obrigado pela presença! Nos vemos na próxima Leading Tech Session."**

---

## Notas para Apresentadores

### Para JV (Bloco 1)
- Foco em **aprendizados práticos**, não teoria
- AI Framework como case principal - você construiu isso
- Dados do LinearB para dar credibilidade externa
- Tom: "O que nós descobrimos fazendo"

### Para Bassan (Bloco 2)
- Foco em **implicações para liderança**
- SOI vs SOR como framework conceitual
- Ownership e context engineering como ações concretas
- Tom: "O que isso exige de quem lidera"

### Interações
- Usar perguntas no chat para manter engajamento
- Não esperar resposta longa - acknowledgment rápido e seguir
- Guardar perguntas complexas para Q&A final

### Timing
- Bloco 1: ~25-30min (deixar margem)
- Bloco 2: ~25-30min (deixar margem)
- Q&A: 5-10min
- Total: ~1h - 1h10
