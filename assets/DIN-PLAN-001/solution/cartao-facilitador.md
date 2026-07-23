# DIN-PLAN-001 — Cartão do Facilitador
## Planning Poker

> **Grupo:** Habilidades Técnicas | **Temática:** Estimativa Ágil | **Momento:** Início de Sprint
> **Duração:** 60 min | **Participantes:** 3–9 | **Modalidade:** Presencial

---

## Objetivo

Calibrar estimativas coletivas de esforço e desenvolver alinhamento técnico
entre os membros do time por meio da revelação simultânea de cartas. A
divergência entre estimativas é tratada como informação valiosa, não como erro.

**Construtos endereçados:** E1.x (Aprendizado) + E2.x (Confiança).

---

## Materiais

| Item | Quantidade | Observação |
|------|-----------|------------|
| Baralho Planning Poker (Fibonacci) | 1 por participante | Não recolher ao final — participantes mantêm o baralho |
| Lista de User Stories para estimar | 1 | Distribuída por escrito antes da reunião |
| Quadro branco ou flipchart | 1 | Para registrar estimativas e desvio padrão |
| Timer visível | 1 | Sinal visual obrigatório além do verbal |
| Agenda de stories (escrita) | 1 por participante | Distribuída antes do início |

---

## Passo a Passo de Condução

### Fase 0 — Preparação (antes do início)

- Distribuir baralhos (1 por participante)
- Distribuir lista de User Stories e agenda por escrito
- Explicar escala Fibonacci e o significado de `?`, `∞` e `☕`
- Anunciar regra principal: **revelação simultânea obrigatória**

### Fase 1 — Rodadas de Estimativa (5 rodadas)

Para cada User Story:

1. PO apresenta a story verbalmente
2. **Silêncio completo** durante a seleção da carta
3. Revelação simultânea ao sinal visual do facilitador
4. Se convergência: registrar e avançar
5. Se divergência: discussão técnica (máx. 3 min) → nova rodada

**Regra:** máximo de 3 rodadas por story.

**Registrar** na Ficha KPI: estimativa consensual + desvio padrão da rodada.

### Fase 2 — Debriefing (10 min)

Conduzir a reflexão com a pergunta-chave:

> *"O que as divergências revelaram sobre a complexidade das tarefas?"*

**Lição central:** Divergência na estimativa = divergência no entendimento
técnico — a discussão é o valor real do Planning Poker.

Perguntas de aprofundamento:
- Em qual story houve maior divergência? O que isso indica?
- Houve stories que todos estimaram igual sem discutir? Isso é bom sinal?
- Como vocês usariam esse processo no dia a dia do time?

---

## Atenção Sensorial (TEA)

| Gatilho identificado | Adaptação recomendada |
|---------------------|-----------------------|
| Pressão de justificar estimativa diferente da maioria | Anunciar verbalmente **e escrever no quadro** o valor consensual de cada story |
| Discussões técnicas longas sem estrutura clara | Usar **sinal visual** (cartão ou gesto) para revelar cartas — além do sinal verbal |

**Adaptações adicionais:**
- Silêncio completo obrigatório durante a seleção da carta
- Distribuir agenda de stories por escrito **antes** da reunião
- Participante pode registrar justificativa por escrito antes de verbalizar

**Condições de interrupção:**
- Interromper discussão técnica que ultrapasse 10 min sem convergência
- Facilitador pode impor consenso por votação final após terceira rodada

---

## Variability Points

| ID | Nome | Quando aplicar |
|----|------|---------------|
| VAR1 | Baralho T-Shirt (XS/S/M/L/XL) | Para times iniciantes em estimativa relativa |
| VAR2 | Versão online (Miro/PlanITPoker) | Para remote onboarding |
| VAR3 | Estimativa de tarefas técnicas | Para refinamento técnico (não stories de negócio) |
