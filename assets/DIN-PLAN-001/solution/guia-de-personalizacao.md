# DIN-PLAN-001 — Guia de Customização
## Planning Poker

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — Baralho T-Shirt
**Quando usar:** Times iniciantes em estimativa relativa que ainda não têm
familiaridade com a escala Fibonacci ou com o conceito de story points.

**Como acionar:**
1. Substituir os baralhos Fibonacci por cartões T-Shirt: XS / S / M / L / XL
2. Explicar correspondência indicativa (não obrigatória): XS=1, S=2, M=3, L=5, XL=8
3. Manter a regra de revelação simultânea e o limite de 3 rodadas por story
4. Após 2–3 sessões com T-Shirt, migrar gradualmente para Fibonacci

**Efeito:** Reduz a barreira de entrada para times sem cultura de estimativa;
facilita discussão qualitativa antes de quantitativa.

**Limites:** Não usar T-Shirt em times com backlog técnico complexo — a escala
qualitativa perde granularidade necessária para decisões de capacidade.

---

### VAR2 — Versão Online
**Quando usar:** Times distribuídos ou híbridos onde Planning Poker presencial
não é possível.

**Como acionar:**
1. Usar PlanITPoker, Scrumpoker Online ou equivalente com votação anônima
2. Alternativa no Miro: criar área de votação com post-its numerados ocultos
   até revelação simultânea via timer
3. Manter o silêncio durante a votação via mute no sistema de videoconferência
4. PO compartilha a story em tela antes de cada rodada — todos leem antes de votar

**Efeito:** Preserva revelação simultânea e anonimato da votação; elimina
influência social presencial.

**Limites:** Garantir que a ferramenta escolhida suporte revelação simultânea
— ferramentas que mostram votos progressivamente invalidam o mecanismo central.

---

### VAR3 — Estimativa de Tarefas Técnicas
**Quando usar:** Sessões de refinamento técnico onde o time precisa estimar
tarefas de implementação (não user stories de produto).

**Como acionar:**
1. Substituir a lista de User Stories por lista de tarefas técnicas
   (ex.: "Migrar banco para PostgreSQL", "Implementar cache Redis", "Refatorar módulo X")
2. Adaptar o critério de consenso: em vez de story points de produto, usar
   estimativa de esforço técnico em horas ou dias ideais
3. Manter as demais regras intactas (revelação simultânea, limite de rodadas)

**Efeito:** Treina o time a estimar complexidade técnica com a mesma disciplina
usada para estimativa de produto.

**Limites:** Não misturar user stories e tarefas técnicas na mesma sessão —
as unidades de medida são incomparáveis e geram confusão.

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 3–4 | Sessão compacta — até 10 stories em 60 min |
| 5–7 | Configuração padrão — 5–8 stories em 60 min |
| 8–9 | Dividir em 2 grupos para estimativa paralela; comparar resultados ao final |
| 10+ | **Não recomendado** — acima de 9 participantes, discussões perdem foco |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Pressão de justificar estimativa diferente da maioria | Permitir justificativa escrita antes de falar; facilitador lê em voz alta |
| Discussões técnicas longas sem estrutura | Cronômetro de 10 min por discussão visível; facilitador interrompe ao atingir limite |
| Surpresa sobre o conteúdo das stories | Distribuir lista de stories por escrito antes da sessão |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica:

- Revelar as cartas de forma não simultânea — qualquer ordem sequencial cria
  ancoragem e invalida a independência das estimativas
- Permitir mais de 3 rodadas por story sem impor consenso — discussões ilimitadas
  transformam estimativa em negociação política
- Omitir o registro de desvio padrão — a divergência quantificada é o dado
  central da Ficha KPI e do debriefing
- Usar a escala T-Shirt e Fibonacci na mesma sessão — a mistura cria ambiguidade
  sobre o que cada valor representa
