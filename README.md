# Leading Tech Session: Desenvolvimento de produto IA-first

> O que muda no desenho dos times

## Event Overview

| Field | Value |
|-------|-------|
| **Date** | January 30, 2026 |
| **Time** | 11:00 AM (BRT) |
| **Duration** | 1h - 1h10 |
| **Format** | Online |
| **Audience** | Heads, leads, and managers (Tech & Product) |
| **Speakers** | Gustavo Bassan (VP Engineering) & JV |
| **Registration** | https://hubs.li/Q03-DyVH0 |

---

## Project Status

| Phase | Status |
|-------|--------|
| References gathered | Done |
| Block outlines | Done |
| Full script | Done |
| Presentation deck | Done |
| Review & approval | Pending |

---

## Objective

Share **practical, real learnings** about what changes when AI stops being a support tool and becomes part of product/software development.

Move beyond generic AI discourse and focus on what really matters for Product and Technology leaders today:

- What worked and what didn't in practice in 2025
- Which decisions became harder (and more important)
- Where current team design starts to break down
- What needs to be redesigned to operate AI-first product in 2026

### Expected Outcomes for Audience

Participants should leave with:

- **Concrete references** from what's already being done in real teams
- **Clearer criteria** for deciding when and how to use AI
- **Practical inputs** to rethink ownership, responsibilities, and context
- **More clarity** about which leadership decisions can no longer be postponed in 2026

---

## Session Format

- 2 presenters
- 2 time blocks: ~30 minutes each
- Sequential talks (not a debate)
- Part 2 complements what was presented in Part 1
- Short final space for questions

---

## Block 1: O Que Aprendemos Construindo Produto com IA em 2025

**Presenter:** JV
**Duration:** ~30 minutes

**Central question:**
> "O que 2025 nos ensinou, na prática, sobre construir produto com IA no centro?"

### Content Structure

1. **Abertura** - Data reality (88.3% adoption, 32.7% AI PR acceptance)
2. **Onde IA funcionou bem** - POCs, features de baixa-média complexidade
3. **Onde IA quebrou expectativas** - Delegation without structure, AI PR problems, agent excess
4. **AI Framework** - Our practical response (5 capabilities, TDAID methodology)
5. **3 Princípios validados** - Context Engineering, Human-in-the-Loop shift, Repertório
6. **Dados de mercado** - LinearB 2026 Benchmarks
7. **Transição** - Setup for Block 2

### Key Message

> "A ferramenta não é o mais importante. É como a empresa se organiza para usar as ferramentas disponíveis."

---

## Block 2: O Que Esses Aprendizados Exigem do Desenho dos Times em 2026

**Presenter:** Gustavo Bassan
**Duration:** ~30 minutes

**Central question:**
> "O que líderes precisam redesenhar agora para operar produto IA-first em 2026?"

### Content Structure

1. **O Shift Fundamental** - Systems of Record → Systems of Intelligence
2. **Redesenhando Ownership** - Context Owner, Validation Owner, Feedback Owner
3. **Context Engineering como Disciplina** - Product Spec as infrastructure, warmup practices
4. **Evitando IA por Conveniência** - Decision framework, 4 questions before implementing AI
5. **O Papel do Líder** - Executor → Orchestrator, Specialist → Context Architect
6. **3 Decisões que não podem ser adiadas** - Ownership, Metrics, Context Engineering investment

---

## Reference Materials

### External Data Sources

| Source | File | Status |
|--------|------|--------|
| LinearB 2026 Software Engineering Benchmarks | `references/LinearB_2026_Software_Engineering_Benchmarks_Report.pdf` | Added |
| ABN Asia Report | `references/1765455980320_www.abnasia.org.pdf` | Added |

### Key Data Points Used

| Metric | Value | Source |
|--------|-------|--------|
| AI adoption in teams | 88.3% (up from 71.6%) | LinearB 2026 |
| AI PR acceptance rate | 32.7% | LinearB 2026 |
| Manual PR acceptance rate | 84.4% | LinearB 2026 |
| Companies not measuring AI impact | 45% | LinearB 2026 |
| AI PRs size increase | 2.6x larger | LinearB 2026 |
| AI PRs pickup time | 5.3x longer | LinearB 2026 |

### Internal References

| Source | Path | Description |
|--------|------|-------------|
| Previous LTS | `areas/marketing/2025/upstream/` | Template and format reference |
| Product Foundation | `areas/product/foundation/articles/` | Frameworks (SOI, Palantirization) |
| AI Framework | `areas/product/operating-system/_old/labs/ai-framework/` | Internal case study |

---

## Deliverables

### Pre-Event

- [x] **Reference materials** - LinearB report, ABN Asia report
- [x] **Block 1 outline** - `drafts/block-1-outline.md`
- [x] **Block 2 outline** - `drafts/block-2-outline.md`
- [x] **Full script** - `drafts/full-script.md` (Portuguese)
- [x] **Presentation deck blueprint** - `drafts/presentation-deck.md`
- [x] **Visual presentation** - `drafts/presentation.pdf` (45 slides)
- [ ] **Review & approval** - Final sign-off from speakers

### Post-Event

- [ ] Recording upload
- [ ] Materials sent to registrants
- [ ] Feedback collection

---

## Folder Structure

```
projects/lts-ia-first-2026/
├── README.md                    # This file
├── references/                  # External data and benchmarks
│   ├── LinearB_2026_Software_Engineering_Benchmarks_Report.pdf
│   └── 1765455980320_www.abnasia.org.pdf
└── drafts/                      # Working documents
    ├── block-1-outline.md       # JV's block structure
    ├── block-2-outline.md       # Bassan's block structure
    ├── full-script.md           # Complete speaker script (PT-BR)
    ├── presentation-deck.md     # Slide-by-slide blueprint for designer
    ├── presentation.html        # Visual deck source (editable)
    └── presentation.pdf         # Final visual deck (45 slides)
```

---

## Presentation Design

The visual deck (`presentation.pdf`) was created with the following specifications:

| Attribute | Value |
|-----------|-------|
| Slides | 45 |
| Dimensions | 1920x1080 (16:9) |
| Theme | Dark (#0a0a0b base) |
| Accent | Blue (#3b82f6) |
| Typography | Inter |
| Format | PDF (1.1MB) |

### Design Elements

- Color-coded data points (green positive, red warning)
- Card-based layouts for case studies
- Clean comparison grids (DE → PARA pattern)
- Flow diagrams for AI Framework workflow
- Section dividers with gradient backgrounds

The `presentation.html` file can be edited directly for modifications. The `presentation-deck.md` serves as a blueprint if a designer needs to recreate the deck in another tool.

---

## Key Frameworks Introduced

### 1. AI Framework (Internal Case)

BossaBox's framework for AI-assisted product development:
- **5 Capabilities**: PM, Tech Lead, SWE, QA, Refinement
- **TDAID**: Test-Driven AI Development (Planning → Red → Green → Validate)
- **Result**: 32% → 80%+ PR acceptance rate

### 2. Systems of Intelligence (SOI)

Transition from Systems of Record to Systems of Intelligence:
- Human-in-the-loop → Human-on-the-loop
- Dashboards → Real-time intelligence
- Human middleware → Autonomous outcomes

### 3. Three Owners Model

New ownership structure for AI-first teams:
- **Context Owner** - Ensures AI has sufficient information
- **Validation Owner** - Validates outputs before decisions
- **Feedback Owner** - Captures learnings for system improvement

---

## Next Steps

1. **Speaker Review** - JV and Bassan review full script and presentation
2. **Rehearsal** - Run through timing and transitions
3. **Final Adjustments** - Incorporate speaker feedback
4. **Event Execution** - January 30, 2026, 11:00 AM

---

## Notes

- All content is in Brazilian Portuguese
- Interactive elements (chat prompts) included throughout
- Estimated timing allows buffer for Q&A
- AI Framework is the primary internal case study demonstrating the principles
