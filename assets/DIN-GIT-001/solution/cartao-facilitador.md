# DIN-GIT-001 — Cartão do Facilitador
## Git em Conflito (Git in Conflict)

> **Grupo:** Habilidades Técnicas | **Temática:** Controle de Versão | **Momento:** Meio de Sprint
> **Duração:** 60 min | **Participantes:** 2–6 | **Modalidade:** Digital

---

## Objetivo

Desenvolver confiança e fluência na resolução de conflitos Git, eliminando o
medo de "quebrar o repositório". Os participantes praticam o ciclo completo de
identificação, resolução e commit de conflitos de merge em ambiente seguro de
treinamento.

**Construtos endereçados:** E1.x (Aprendizado) + E2.x (Confiança).

---

## Materiais

| Item | Quantidade | Observação |
|------|-----------|------------|
| Repositório Git de treinamento | 1 | Com conflitos pré-fabricados — pode ser recriado a qualquer momento |
| IDE com 3-way merge view | 1 por participante | VS Code ou GitKraken recomendados |
| Checklist de 5 passos (impresso ou digital) | 1 por dupla | Identificar → Abrir → Escolher/combinar → Remover marcadores → Commitar |
| Projetor ou tela compartilhada | 1 | Para revisão coletiva do diff side-by-side |

---

## Passo a Passo de Condução

### Fase 0 — Preparação (antes do início)

- Clonar o repositório de treinamento em cada máquina
- Configurar `user.name` e `user.email` em cada ambiente
- Projetar o diff side-by-side no quadro antes da resolução individual
- Apresentar narrativa completa: quem fez o quê em qual branch

### Fase 1 — Briefing (5 min)

- Apresentar o cenário narrativo do conflito
- Distribuir o checklist de 5 passos:
  1. **Identificar** — `git status` e `git diff`
  2. **Abrir** — editor com visualização de conflito
  3. **Escolher/combinar** — decidir qual versão preservar
  4. **Remover marcadores** — eliminar `<<<<<<<`, `=======`, `>>>>>>>`
  5. **Commitar** — registrar a resolução
- Mostrar exemplo de comentário de commit para resolução de conflito

### Fase 2 — Conflito 1: Merge Simples (15 min)

- Duplas executam `git merge` no repositório de treinamento
- Resolvem conflito de texto simples usando o checklist
- Garantem commit limpo ao final

### Fase 3 — Revisão Coletiva (5 min)

- Discutir estratégias usadas pelas duplas
- Comparar abordagens diferentes para o mesmo conflito

### Fase 4 — Conflito 2: Lógica Conflitante (15 min)

- Ambas as versões são válidas e precisam ser combinadas
- Duplas praticam a fusão intencional de código

### Fase 5 — Conflito 3: Rebase (10 min — opcional)

- Apenas para perfis avançados
- Praticar `git rebase` como alternativa ao merge

### Fase 6 — Debriefing (10 min)

Conduzir a reflexão com a pergunta-chave:

> *"Como comunicar melhor ao fazer um PR para evitar conflitos futuros?"*

**Lição central:** Conflito Git = divergência de intenção — resolver requer
comunicação, não apenas comandos.

Perguntas de aprofundamento:
- Qual mensagem de erro causou mais ansiedade? Por quê?
- O que vocês fariam diferente antes de abrir o PR?
- Como o tamanho do PR influencia a frequência de conflitos?

---

## Atenção Sensorial (TEA)

| Gatilho identificado | Adaptação recomendada |
|---------------------|-----------------------|
| Medo de "quebrar" o repositório compartilhado | Reforçar que **o repositório de treinamento pode ser recriado** a qualquer momento |
| Mensagens de erro Git percebidas como falha pessoal | Usar **VS Code 3-way merge view** ou GitKraken para visualização clara |
| Pressão de tempo na resolução | Prática **em dupla** recomendada — reduz pressão de resolução solo |

**Condições de interrupção:**
- Interromper se participante demonstrar ansiedade elevada ao ver mensagens de erro
- Reforçar que erros são reversíveis — demonstrar `git reset` se necessário
- Permitir consulta ao facilitador a qualquer momento sem julgamento

---

## Variability Points

| ID | Nome | Quando aplicar |
|----|------|---------------|
| VAR1 | Conflito em arquivo binário | Para perfis avançados com experiência em Git |
| VAR2 | Múltiplas linguagens | Python, JS e Java em conflito simultâneo |
| VAR3 | Ambiente offline | Repositório local bare sem acesso à internet |
