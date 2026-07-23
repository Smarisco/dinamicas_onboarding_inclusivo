# DIN-AGIL-001 — Guia de Customização
## Jogo das Bolinhas (Ballpoint Game)

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — Bolinhas com Pesos Diferentes
**Quando usar:** Times com experiência em Scrum que já conhecem o conceito de
velocity e precisam de maior desafio cognitivo.

**Como acionar:**
1. Substituir bolinhas de espuma uniformes por bolinhas de pesos distintos
   (ex.: bolinhas de borracha, plástico e espuma misturadas)
2. Atribuir pontuações diferentes por tipo: espuma = 1 pt, plástico = 2 pts,
   borracha = 3 pts
3. Anunciar os pesos antes do Sprint 1 — sem surpresa sobre a regra

**Efeito esperado:** O time é forçado a priorizar quais "tarefas" (bolinhas)
valem mais — simula variabilidade de WIP e priorização de backlog.

**Limites:** Manter as 5 regras originais intactas. Não alterar o ciclo de sprints.

---

### VAR2 — Versão Remota
**Quando usar:** Times distribuídos ou contextos de remote onboarding onde
presença física não é possível.

**Como acionar:**
1. Usar quadro digital colaborativo (Miro, MURAL ou similar) com objetos
   arrastáveis representando as bolinhas
2. Cada participante tem uma "zona" no quadro — objetos devem passar por todas
   as zonas seguindo as 5 regras adaptadas para drag-and-drop
3. Cronômetro compartilhado visível na tela (ex.: cuckoo.team ou timer no Miro)
4. Sinal visual de início/fim via reação de emoji no chat

**Limites:** A versão remota reduz o componente sensorial e físico — o aprendizado
sobre fluxo é preservado, mas a experiência de auto-organização corporal é perdida.
Informar os participantes antes.

---

### VAR3 — Debriefing Estendido
**Quando usar:** Times de engenharia com familiaridade com métricas de fluxo
(Cycle Time, Lead Time, WIP) que precisam conectar a dinâmica a dados reais.

**Como acionar:**
1. Ao final dos 5 sprints, plotar throughput em gráfico de barras no quadro
2. Calcular e exibir: média, desvio padrão e maior delta entre sprints consecutivos
3. Acrescentar perguntas ao debriefing padrão:
   - "Qual sprint teve menor variabilidade? O que isso indica sobre estabilidade do processo?"
   - "Como este gráfico se relaciona com o Cumulative Flow Diagram do seu time?"
4. Duração adicional: +15 min sobre o debriefing padrão (total: ~55 min)

**Limites:** Não usar VAR3 com times iniciantes — a análise de métricas pode
desviar o foco da lição central (Processo > Esforço bruto).

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 3–5 | 1 círculo único; todos passam bolinhas |
| 6–10 | 1 círculo único; considerar papel de observador/registrador |
| 10+ | **Não recomendado** — dividir em duas sessões paralelas |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Ruído de bolinhas | Usar exclusivamente bolinhas de espuma |
| Sinal sonoro abrupto | Substituir por cartão colorido ou luz LED |
| Aglomeração em espaços pequenos | Garantir 1 m² por participante; oferecer papel de observador |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica e não devem
ser feitas:

- Remover ou modificar qualquer uma das 5 regras originais durante a execução
- Reduzir para menos de 3 sprints (o aprendizado iterativo requer pelo menos 3
  ciclos para emergir)
- Permitir que participantes vejam o throughput de outros times durante a execução
  (quebra a auto-organização emergente)
- Substituir bolinhas por objetos grandes que exijam duas mãos (altera a dinâmica
  de passagem e a regra de contato único)
