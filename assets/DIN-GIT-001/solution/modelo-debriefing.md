# DIN-GIT-001 — Template de Debriefing
## Git em Conflito (Git in Conflict)

> **Duração do debriefing:** 8–10 min | **Condução:** Facilitador
> **Construtos avaliados:** E1.x (Aprendizado) + E2.x (Confiança) — Ju et al., ICSE 2021, Tabela III

## Estrutura de Condução

| Etapa | Tempo | Formato |
|-------|-------|---------|
| Pergunta-chave | 2 min | Facilitador lança — silêncio para reflexão antes das respostas |
| Respostas abertas | 4 min | Voluntário ou rodada — sem pressão para falar |
| Síntese da lição | 2 min | Facilitador fecha com a lição central |
| Registro de ações | 2 min | Cada participante escreve 1 compromisso pessoal |

> **Regra TEA:** aceitar respostas escritas (post-it ou chat) como equivalentes às verbais em qualquer etapa.

---

## Pergunta-Chave

> *"Como comunicar melhor ao fazer um PR para evitar conflitos futuros?"*

**Lição central:** Conflito Git = divergência de intenção — resolver requer comunicação, não apenas comandos.

---

## Perguntas-Guia de Reflexão

### Bloco 1 — O que aconteceu? (Gather Data)

1. Qual dos três conflitos foi mais difícil de resolver? O que o tornou mais complexo?
2. Em que momento você percebeu que o conflito não era apenas técnico — havia intenções divergentes?
3. Quais marcadores de conflito (`<<<<<<<`, `=======`, `>>>>>>>`) foram mais confusos de interpretar?

### Bloco 2 — Por que aconteceu? (Generate Insights)

4. O que levou as duas versões a divergir? Foi falta de comunicação antes do commit ou decisão técnica diferente?
5. Quando você escolheu uma versão sobre a outra, como tomou essa decisão? Consultou o parceiro?
6. O que tornaria um PR mais fácil de integrar — menos código, melhor descrição ou commits menores?

### Bloco 3 — O que aprendemos? (E1 — Aprendizado)

7. Qual é a diferença entre `git merge` e `git rebase` na perspectiva de quem vai revisar o histórico?
8. Como o checklist de 5 passos (Identificar → Abrir → Escolher/combinar → Remover marcadores → Commitar) mudou sua abordagem?
9. O que é um "conflito de intenção" em contraste com um "conflito de texto"?

### Bloco 4 — Como nos relacionamos? (E2 — Confiança)

10. Em algum momento você sentiu ansiedade ao ver mensagens de erro do Git? O que ajudou a reduzir esse desconforto?
11. Como trabalhar em dupla mudou a forma de abordar o conflito em comparação com resolver sozinho?
12. O que tornaria mais fácil pedir ajuda ao ver um conflito que você não entende?

### Bloco 5 — O que faremos diferente? (Ação)

13. Descreva uma prática de comunicação em PRs que você adotaria para reduzir conflitos futuros.
14. Como você descreveria o contexto de uma mudança em uma mensagem de commit para ajudar quem vai resolver conflitos depois?

---

## Indicadores de Aprendizagem Esperados

| Construto | Indicador observável | Como verificar |
|-----------|---------------------|----------------|
| **E1.x — Aprendizado** | Participante distingue conflito técnico de conflito de intenção | Resposta à pergunta 4 ou 9 |
| **E2.x — Confiança** | Participante identifica gatilho de ansiedade e estratégia de redução | Resposta à pergunta 10 ou 12 |
| **Aprendizado Experiencial** | Participante conecta resolução de conflito Git a prática real de PR | Resposta à pergunta 6 ou 13 |

---

## Registro Pós-Sessão (preencher pelo facilitador)

Data: ___ | Participantes: ___ | Duplas: ___

Conflitos resolvidos por dupla: C1:___ C2:___ C3 (opcional):___

Estratégia mais usada na resolução: ___

Insight mais relevante: ___

Ação coletiva acordada: ___

Observações sensoriais (ansiedade com erros, pressão de tempo): ___

---

## Referência

Ju, A. et al. (2021). A Case Study of Onboarding in Software Teams. ICSE 2021 — Tabela III: E1, E2.
