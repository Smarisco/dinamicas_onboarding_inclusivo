# DIN-TDD-001 — Cartão do Facilitador
## TDD Kata

> **Grupo:** Hard Skills | **Temática:** Qualidade de Software | **Momento:** Meio de Sprint
> **Duração:** 60 min | **Participantes:** 1–4 | **Modalidade:** Digital

---

## Objetivo

Internalizar a disciplina do ciclo Red-Green-Refactor por meio de prática
repetitiva (kata) em problema simples e bem definido. Ao final, os participantes
devem ser capazes de nunca escrever código de produção sem um teste falhando antes.

**Construtos endereçados:** E1.x (Aprendizado) + E2.x (Confiança).

---

## Materiais

| Item | Quantidade | Observação |
|------|-----------|------------|
| IDE configurada com framework de testes | 1 por participante | pytest, JUnit, Jest ou equivalente |
| Poster visual Red → Green → Refactor | 1 | Visível na tela durante toda a prática |
| Descrição do kata com requisitos numerados | 1 por participante | Participante sabe o que vem a seguir |
| Ficha KPI | 1 por participante | Registrar ciclos completados e tempo médio por ciclo |

---

## Passo a Passo de Condução

### Fase 0 — Preparação (antes do início)

- Configurar IDE com framework de testes instalado e funcionando
- Exibir poster do ciclo Red-Green-Refactor na tela
- Configurar indicadores visuais de Red/Green claramente na IDE
- Distribuir descrição do kata com requisitos incrementais numerados

### Fase 1 — Demonstração ao Vivo (10 min)

- Facilitador implementa o **primeiro requisito** ao vivo
- Demonstrar explicitamente cada etapa:
  1. Escrever teste → ver falhar (**Red**)
  2. Escrever código mínimo → ver passar (**Green**)
  3. Melhorar o código sem quebrar o teste (**Refactor**)
- Verbalizar o raciocínio em cada passo

### Fase 2 — Prática Guiada (20 min)

- Participantes implementam os próximos requisitos
- Facilitador disponível para dúvidas — não intervém no código
- **Regra crítica:** nunca escrever linha de produção sem teste falhando antes
- Verificar estado atual antes de cada linha: Red / Green / Refactor?

### Fase 3 — Prática Autônoma (15 min)

- Participantes continuam sem intervenção do facilitador
- Facilitador observa e anota padrões para o debriefing

### Fase 4 — Debriefing (15 min)

Conduzir a reflexão com a pergunta-chave:

> *"Quando você quis pular o teste? O que te impediu?"*

**Lição central:** TDD é disciplina, não velocidade — o teste é o design.

Perguntas de aprofundamento:
- Em qual momento o ciclo Red-Green-Refactor pareceu mais natural?
- O que aconteceu quando você tentou escrever código sem o teste?
- Como o TDD mudaria a forma como você aborda um PR no trabalho real?

---

## Atenção Sensorial (TEA)

| Gatilho identificado | Adaptação recomendada |
|---------------------|-----------------------|
| Frustração ao ver testes falhando (percepção de falha pessoal) | Reforçar: **Red é o estado inicial correto e esperado** |
| Pressão de seguir o ciclo rigorosamente sem "atalhos" | Poster visual do ciclo **sempre visível** na tela |

**Adaptações adicionais:**
- IDE configurada para mostrar indicadores vermelhos/verdes claramente
- Kata com requisitos incrementais numerados — participante sabe o que vem a seguir
- Verificar estado atual (Red/Green/Refactor) antes de cada linha de código

**Condições de interrupção:**
- Interromper se participante demonstrar frustração excessiva com testes falhando
- Permitir prática solo para participantes que preferem ritmo próprio
- Oferecer pausa de 2 min sem julgamento se necessário

---

## Variability Points

| ID | Nome | Quando aplicar |
|----|------|---------------|
| VAR1 | FizzBuzz Kata | Para iniciantes absolutos em TDD |
| VAR2 | String Calculator Kata | Nível intermediário — requisitos incrementais mais complexos |
| VAR3 | Ping-Pong TDD | Prática em pair programming — um escreve o teste, o outro o código |
