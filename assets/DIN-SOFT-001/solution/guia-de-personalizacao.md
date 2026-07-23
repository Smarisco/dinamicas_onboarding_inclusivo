# DIN-SOFT-001 — Guia de Customização
## A Moeda de Duas Faces (The Two-Sided Coin)

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — Versão GDPR/LGPD
**Quando usar:** Times que trabalham com dados pessoais ou em contextos regulados
onde o trade-off privacidade vs. funcionalidade é recorrente no dia a dia.

**Como acionar:**
1. Substituir o cenário padrão (Lançar Agora vs. Atrasar e Testar) pelo cenário:
   - Grupo A (Dev): "Implementar a funcionalidade agora e tratar conformidade LGPD depois"
   - Grupo B (QA/Legal): "Garantir conformidade LGPD antes de qualquer lançamento"
2. Distribuir cartão com contexto: funcionalidade de coleta de dados pessoais com
   prazo de lançamento em 2 semanas; auditoria LGPD pendente
3. Manter a estrutura de 3 argumentos técnicos + 3 de negócio por grupo

**Efeito:** Conecta a dinâmica a um dilema real e frequente em times de produto
— aumenta engajamento e transferência para o trabalho real.

**Limites:** Não usar se o time estiver ativamente em processo de auditoria
LGPD — o debate pode gerar ansiedade em vez de aprendizado.

---

### VAR2 — Versão Dívida Técnica
**Quando usar:** Times com acúmulo de dívida técnica onde o debate
refatorar vs. feature nova é uma tensão real e frequente.

**Como acionar:**
1. Substituir o cenário padrão pelo cenário:
   - Grupo A (Dev/Produto): "Entregar a nova feature agora — refatoração pode esperar"
   - Grupo B (Arquitetura/Tech Lead): "Refatorar o módulo X antes de qualquer feature nova"
2. Distribuir cartão com contexto: módulo X tem 40% de cobertura de testes e
   3 bugs conhecidos; feature nova é prioridade do PO para o próximo sprint
3. Manter a estrutura de argumentos e as fases de debate

**Efeito:** Torna explícito o custo invisível da dívida técnica — participantes
precisam articular esse custo em termos de negócio, não apenas técnicos.

**Limites:** Não usar módulo real do repositório do time como exemplo — pode
gerar defensividade dos autores originais do código.

---

### VAR3 — Versão Silenciosa
**Quando usar:** Participantes com ansiedade social elevada para quem debate
oral representa barreira — ou como alternativa imediata quando o debate
escala para conflito.

**Como acionar:**
1. Substituir toda a fase de debate oral por troca de post-its no quadro:
   - Grupo A cola argumento → Grupo B lê e cola contra-argumento → e assim por diante
   - Facilitador gerencia a ordem dos post-its e lê em voz alta se necessário
2. Bastão da fala substituído por marcador de vez (post-it colorido) que indica
   de qual grupo é a vez de colar
3. Inversão de papéis mantida: grupos trocam de coluna e escrevem 1 argumento
   na posição oposta

**Efeito:** Remove completamente a pressão de vocalização mantendo o aprendizado
de argumentação e empatia cognitiva.

**Limites:** A dinâmica de debate oral tem componente de regulação emocional
em tempo real que VAR3 não reproduz. Usar VAR3 como adaptação de acessibilidade
e oferecer versão oral em sessões futuras quando o grupo estiver mais confortável.

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 6–8 | 2 grupos de 3–4; debate com todos em círculo |
| 9–14 | 2 grupos de 4–7; porta-vozes designados por grupo para o debate |
| 15–20 | 2 grupos de 7–10; porta-vozes rotativos (2 por grupo); observadores registram argumentos |
| 21+ | **Não recomendado** — dividir em múltiplos debates paralelos com facilitadores |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Debate acalorado pode escalar | Bastão da fala obrigatório; facilitador interrompe imediatamente se tom elevar |
| Pressão de defender posição contrária | "Advogado do diabo" explicado antes; argumentos preparados em post-its — sem improvisação |
| Múltiplas vozes simultâneas | Bastão da fala físico elimina sobreposição; VAR3 como alternativa total |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica:

- Omitir a explicação de "advogado do diabo" antes do debate — sem esta
  ancoragem, participantes com rigidez cognitiva interpretam a inversão de
  papéis como exigência de mudar de opinião genuinamente
- Remover o bastão da fala ou torná-lo opcional — sem o bastão, vozes
  dominantes tomam o debate e o aprendizado de escuta ativa é perdido
- Pular a inversão de papéis — é o mecanismo central de empatia cognitiva;
  sem ela, a dinâmica vira debate comum sem aprendizado de perspectiva oposta
- Permitir argumentos pessoais ou emocionais — a restrição a argumentos
  técnicos e de negócio é o que mantém o debate seguro e produtivo
