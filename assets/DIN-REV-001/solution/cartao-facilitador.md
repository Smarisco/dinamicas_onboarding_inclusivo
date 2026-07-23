# DIN-REV-001 — Cartão do Facilitador
## CRSG — Code Review Simulation Game

> **Grupo:** Hard Skills | **Temática:** Revisão de Código | **Momento:** Meio de Sprint
> **Duração:** 55 min | **Participantes:** 2–6 | **Modalidade:** Digital

---

## Objetivo

Desenvolver a capacidade de identificar defeitos sistematicamente e fornecer
feedback técnico construtivo por meio de simulação de code review com defeitos
intencionais e checklists estruturados.

**Construtos endereçados:** E1.x (Aprendizado) + E2.x (Confiança).

---

## Materiais

| Item | Quantidade | Observação |
|------|-----------|------------|
| Código-fonte com defeitos intencionais | 1 por participante | Impresso ou digital — com syntax highlighting |
| Checklist de revisão por categoria | 1 por participante | Bug / Code Smell / Segurança / Performance / Legibilidade |
| Projetor ou tela compartilhada | 1 | Fonte ≥ 14pt para leitura coletiva |
| Gabarito do facilitador | 1 | Disponível ao final para comparação objetiva |
| Ficha KPI | 1 por participante | Registrar defeitos encontrados por categoria |

---

## Passo a Passo de Condução

### Fase 0 — Preparação (antes do início)

- Distribuir código-fonte e checklists (impresso ou digital)
- Configurar projetor com fonte ≥ 14pt
- Preparar gabarito do facilitador (não distribuir ainda)
- Definir o exemplo de comentário construtivo vs. destrutivo para o briefing

### Fase 1 — Briefing (5 min)

- Explicar objetivo e os 5 tipos de defeito do checklist
- Mostrar exemplo de comentário **construtivo** vs. **destrutivo**
- Anunciar estrutura: ler → identificar → categorizar → comentar → comparar

### Fase 2 — Revisão Individual/Dupla (20 min)

- Usar o checklist para identificar defeitos
- Para cada defeito encontrado, escrever um comentário seguindo o modelo:
  - **O que:** descrever o problema objetivamente
  - **Por quê:** explicar o impacto
  - **Como:** sugerir a correção
- Registrar na Ficha KPI: quantidade por categoria

### Fase 3 — Revisão Coletiva (15 min)

- Projetar o código linha a linha
- Percorrer o checklist coletivamente
- Comparar comentários dos participantes
- Facilitador revela o gabarito ao final

### Fase 4 — Prática de Comentário (5 min)

- Selecionar 1 comentário destrutivo identificado no grupo
- Reformulá-lo coletivamente em comentário construtivo

### Fase 5 — Debriefing (10 min)

Conduzir a reflexão com a pergunta-chave:

> *"Quais defeitos ninguém encontrou? O que isso nos diz sobre
> nossos pontos cegos?"*

**Lição central:** Code review é uma skill — checklists e prática
aumentam a cobertura sistematicamente.

Perguntas de aprofundamento:
- Qual categoria de defeito foi mais difícil de identificar? Por quê?
- Como um checklist muda a qualidade da revisão vs. leitura livre?
- O que você mudaria nos seus próximos PRs depois desta prática?

---

## Atenção Sensorial (TEA)

| Gatilho identificado | Adaptação recomendada |
|---------------------|-----------------------|
| Pressão de encontrar defeitos que outros encontraram e você não | Gabarito disponível ao **final** — comparação objetiva, não competitiva |
| Feedback público sobre qualidade dos comentários escritos | Revisão individual **antes** da coletiva — participante chega preparado |

**Adaptações adicionais:**
- Fornecer código com syntax highlighting — nunca plain text
- Projetar com fonte ≥ 14pt para facilitar leitura coletiva
- Checklists com categorias explícitas eliminam categorização espontânea
- Papel de registrador disponível na revisão coletiva

**Condições de interrupção:**
- Interromper se participante demonstrar ansiedade ao receber feedback público
- Permitir contribuição anônima por escrito durante a revisão coletiva

---

## Variability Points

| ID | Nome | Quando aplicar |
|----|------|---------------|
| VAR1 | Múltiplas linguagens | Python, JS e Java em código separado — para times poliglotas |
| VAR2 | Foco em padrões de design | Violações de SOLID, DRY, KISS — para perfis avançados |
| VAR3 | PR real anonimizado | PR real do próprio time — para times com maturidade em revisão |
