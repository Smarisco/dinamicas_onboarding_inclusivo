# DIN-REV-001 — Guia de Customização
## CRSG — Code Review Simulation Game

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — Múltiplas Linguagens
**Quando usar:** Times políglotas onde cada membro trabalha em linguagem diferente
e o objetivo é demonstrar que boas práticas de revisão são independentes de sintaxe.

**Como acionar:**
1. Preparar 3 versões do mesmo código com defeitos equivalentes — Python, JS e Java
2. Atribuir uma linguagem por participante ou dupla conforme perfil técnico
3. Revisão coletiva compara como o mesmo tipo de defeito (ex.: Code Smell) se
   manifesta diferente em cada linguagem
4. Gabarito do facilitador contém os defeitos nas 3 versões

**Efeito:** Demonstra que checklist de revisão é transferível entre linguagens —
reduz resistência de times políglotas a adotar padrões comuns.

**Limites:** Não atribuir linguagem desconhecida ao participante — o objetivo é
revisar, não aprender sintaxe nova.

---

### VAR2 — Foco em Padrões de Design
**Quando usar:** Times com experiência em revisão básica que precisam evoluir
para identificar violações arquiteturais e de design.

**Como acionar:**
1. Preparar código com violações explícitas de SOLID, DRY e KISS além dos
   defeitos padrão (Bug, Segurança, Performance, Legibilidade)
2. Adicionar ao checklist uma 6ª categoria: **Padrão de Design**
   (exemplos: God Class, Feature Envy, Shotgun Surgery)
3. Dedicar os 15 min da revisão coletiva ao debate sobre a violação de design
   mais grave identificada

**Efeito:** Eleva o nível de abstração da revisão — de erros de implementação
para decisões de arquitetura.

**Limites:** Não usar VAR2 com times iniciantes em revisão — a complexidade
das violações de design pode obscurecer os defeitos mais básicos.

---

### VAR3 — PR Real Anonimizado
**Quando usar:** Times avançados onde a prática com código fictício já foi
consolidada e o objetivo é aproximar o exercício da realidade do time.

**Como acionar:**
1. Selecionar um PR real do repositório do time — preferencialmente já mergeado
2. Anonimizar autoria: remover nome do autor e quaisquer referências identificáveis
3. Remover ou manter comentários de revisão existentes conforme objetivo:
   - Sem comentários: participantes revisam do zero e comparam com o que foi feito
   - Com comentários ocultos: revelar ao final como gabarito
4. Informar ao time antes: "este é um PR real anonimizado do nosso repositório"

**Efeito:** Máxima relevância contextual — os defeitos são reais e as decisões
de revisão têm peso de consequência real.

**Limites:** Obter consentimento implícito do time antes de usar PRs reais —
mesmo anonimizados, podem gerar desconforto se o estilo de código for
reconhecível.

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 2–3 | Revisão individual; revisão coletiva em par com facilitador |
| 4–6 | 2–3 duplas paralelas; revisão coletiva unificada ao final |
| 7+ | **Não recomendado** — dividir em grupos de no máximo 6 |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Pressão de encontrar defeitos que outros encontraram | Gabarito revelado ao final — não durante a revisão coletiva; focar em "o que aprendemos" não em "quem achou mais" |
| Feedback público sobre comentários escritos | Revisão individual concluída antes de exposição; papel de registrador disponível |
| Código denso sem estrutura visual | Syntax highlighting obrigatório; fonte ≥ 14pt na projeção coletiva |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica:

- Revelar o gabarito durante a revisão individual — elimina a descoberta
  independente que é o mecanismo pedagógico central
- Omitir a prática de reformulação de comentário (5 min) — sem ela, a dinâmica
  treina apenas identificação, não comunicação construtiva
- Usar código sem defeitos intencionais pré-definidos — a comparação com o
  gabarito é o que transforma a prática em aprendizado verificável
- Pular a revisão individual e ir direto para a coletiva — a exposição sem
  preparo individual amplifica ansiedade e reduz qualidade das contribuições
