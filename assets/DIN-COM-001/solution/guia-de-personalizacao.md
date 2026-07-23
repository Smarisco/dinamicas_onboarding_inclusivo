# DIN-COM-001 — Guia de Customização
## O Campo Minado (The Minefield)

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — Sem Venda (Escrita Prévia)
**Quando usar:** Participantes com ansiedade intransponível relacionada a
venda nos olhos — ou como adaptação de acessibilidade imediata.

**Como acionar:**
1. Remover a venda completamente — Navegador mantém olhos abertos mas não
   pode olhar para os objetos: olha apenas para o Guia
2. Guia escreve todos os comandos antes da travessia e lê em voz alta durante
   a execução — sem improvisar
3. Cartão de Comandos permanece obrigatório — vocabulário literal mantido

**Efeito:** Remove o gatilho sensorial da venda preservando o aprendizado
de comunicação precisa — a restrição de vocabulário continua gerando erros
quando as instruções são ambíguas.

**Limites:** Sem a venda, a dependência total das instruções diminui — o
Navegador pode usar referências visuais periféricas. Explicar explicitamente
que olhar para os objetos invalida a rodada.

---

### VAR2 — Remota via Chat
**Quando usar:** Times remotos ou híbridos onde a dinâmica presencial não
é possível.

**Como acionar:**
1. Substituir travessia física por mapa digital — grid em Miro ou Google Slides
   com objetos posicionados como células bloqueadas
2. Guia envia comandos via chat (Slack ou chat da reunião) com delay de 5s
   entre cada instrução — Navegador executa movendo cursor no grid
3. Cartão de Comandos adaptado para grid: cima/baixo/esquerda/direita + número
   de células
4. Timer compartilhado visível na tela durante cada travessia

**Efeito:** Preserva o aprendizado de precisão linguística; o delay de 5s
simula o custo de ambiguidade em comunicação assíncrona — mais próximo
do contexto real de times distribuídos.

**Limites:** A experiência sensorial da venda e da travessia física é perdida.
Verificar latência de conexão antes — delay manual de 5s exige que os
participantes se auto-disciplinem.

---

### VAR3 — Múltiplos Sistemas
**Quando usar:** Times com mais de uma stack ou linguagem onde a ambiguidade
de nomenclatura entre sistemas é um problema real e recorrente.

**Como acionar:**
1. Cada dupla recebe Cartão de Comandos com vocabulário diferente — dupla A
   usa termos de backend (request/response/timeout), dupla B usa termos de
   frontend (click/scroll/render)
2. Na fase de debriefing, comparar os erros entre duplas com vocabulários
   diferentes: qual sistema gerou mais colisões?
3. Manter a estrutura de 2 travessias com inversão de papéis

**Efeito:** Torna explícito o custo de ter múltiplos vocabulários dentro do
mesmo time — o debriefing conecta diretamente ao problema real de integração
entre sistemas.

**Limites:** Não misturar vocabulários dentro da mesma dupla — cada dupla
deve ter um único Cartão de Comandos consistente para isolar a variável
do experimento.

---

### VAR4 — Campo Codificado
**Quando usar:** Times com experiência em sistemas codificados (APIs, CLIs,
protocolos) onde o aprendizado deve focar em especificidade de sintaxe.

**Como acionar:**
1. Substituir o vocabulário literal por comandos codificados: `MOVE(N,3)`,
   `TURN(LEFT)`, `STOP` — sem linguagem natural
2. Guia só pode usar os comandos do dicionário codificado — nenhuma palavra
   fora do dicionário é válida
3. Navegador executa apenas comandos válidos — ignora instruções em linguagem
   natural

**Efeito:** Conecta diretamente ao contexto de APIs e CLIs — o erro de
ambiguidade se torna erro de sintaxe, mais próximo da realidade técnica.

**Limites:** Exige que o Cartão de Comandos seja distribuído e estudado
antes da travessia — não usar como primeira exposição sem tempo de prática
do vocabulário codificado (mínimo 5 min de familiarização).

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 8–10 | 4–5 duplas; campos simultâneos com separação física |
| 11–12 | 5–6 duplas ou trios com observador |
| 13+ | **Não recomendado** — dividir em grupos de no máximo 12 |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Ansiedade com venda nos olhos | VAR1 (Sem Venda) acionada imediatamente; óculos opacos como etapa intermediária |
| Ruído de múltiplas duplas guiando simultaneamente | Espaços separados entre duplas; VAR2 (Remota) como alternativa total |
| Pressão de tempo durante a travessia | Escrita prévia de comandos obrigatória; timer visível mas sem contagem regressiva sonora |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica:

- Permitir linguagem metafórica ou gestual durante a travessia — a restrição
  ao vocabulário literal do Cartão de Comandos é o mecanismo central que
  gera os erros de comunicação; sem ela, a dinâmica não produz dados de
  aprendizagem
- Alterar o layout do campo entre Travessia 1 e Travessia 2 — a inversão
  de papéis com campo idêntico é o que permite comparar desempenho de
  comunicação entre Guia e Navegador
- Omitir a escrita prévia de comandos — improvisar durante a travessia
  aumenta variáveis não-controladas e elimina o mecanismo de acessibilidade
  central para participantes TEA
- Pular a inversão de papéis — sem ela, apenas metade dos participantes
  pratica o papel de Guia e o aprendizado de empatia (navegar com
  instruções alheias) é perdido
