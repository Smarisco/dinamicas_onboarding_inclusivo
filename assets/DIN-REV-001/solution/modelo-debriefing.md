# DIN-REV-001 — Template de Debriefing
## CRSG — Code Review Simulation Game

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

> *"Quais defeitos ninguém encontrou? O que isso nos diz sobre nossos pontos cegos?"*

**Lição central:** Code review é uma skill — checklists e prática aumentam cobertura.

---

## Perguntas-Guia de Reflexão

### Bloco 1 — O que aconteceu? (Gather Data)

1. Quantos defeitos você identificou individualmente? Quantos foram encontrados pela dupla/grupo coletivamente?
2. Em qual categoria de defeito (Bug, Code Smell, Segurança, Performance, Legibilidade) você encontrou mais itens?
3. Qual foi o defeito mais difícil de detectar? Por quê ele passou despercebido na primeira leitura?

### Bloco 2 — Por que aconteceu? (Generate Insights)

4. Quais defeitos ninguém encontrou? O que essa lacuna coletiva revela sobre o que o grupo tende a ignorar?
5. Como o checklist mudou sua abordagem de leitura em comparação com uma revisão sem estrutura?
6. O que distingue um comentário de revisão construtivo de um destrutivo? O que muda na recepção de cada um?

### Bloco 3 — O que aprendemos? (E1 — Aprendizado)

7. Por que Code Smells e problemas de Legibilidade são frequentemente ignorados em revisões reais?
8. Como o uso de checklists com categorias explícitas reduz a dependência de expertise individual?
9. O que é um "ponto cego coletivo" e por que revisores diferentes encontram defeitos diferentes?

### Bloco 4 — Como nos relacionamos? (E2 — Confiança)

10. Em algum momento você sentiu desconforto ao perceber que outros encontraram defeitos que você não viu?
11. Como você se sentiu ao ter seu comentário reformulado de destrutivo para construtivo? O que mudou na mensagem?
12. O que tornaria mais fácil dar feedback técnico crítico sem que o autor perceba como ataque pessoal?

### Bloco 5 — O que faremos diferente? (Ação)

13. Cite uma categoria de defeito que você passará a verificar explicitamente em revisões reais a partir de agora.
14. Como você reformularia um comentário de revisão que normalmente escreveria de forma direta mas que pode ser percebido como agressivo?

---

## Indicadores de Aprendizagem Esperados

| Construto | Indicador observável | Como verificar |
|-----------|---------------------|----------------|
| **E1.x — Aprendizado** | Participante identifica categoria de defeito que consistentemente escapa à sua revisão | Resposta à pergunta 4 ou 9 |
| **E2.x — Confiança** | Participante descreve diferença de impacto entre comentário construtivo e destrutivo | Resposta à pergunta 6 ou 11 |
| **Aprendizado Experiencial** | Participante conecta simulação à prática real de PR review no time | Resposta à pergunta 8 ou 13 |

---

## Registro Pós-Sessão (preencher pelo facilitador)

Data: ___ | Participantes: ___ | Defeitos no gabarito: ___

Defeitos encontrados (média por participante): ___

Categoria com menor cobertura coletiva: ___

Defeitos não encontrados por ninguém: ___

Insight mais relevante: ___

Ação coletiva acordada: ___

Observações sensoriais (pressão de encontrar defeitos, feedback público): ___

---

## Referência

Ju, A. et al. (2021). A Case Study of Onboarding in Software Teams. ICSE 2021 — Tabela III: E1, E2.
