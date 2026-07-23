# DIN-TDD-001 — Guia de Customização
## TDD Kata

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — FizzBuzz Kata
**Quando usar:** Participantes sem nenhuma experiência prévia com TDD ou com
testes automatizados — primeiro contato com o ciclo Red-Green-Refactor.

**Como acionar:**
1. Usar o enunciado FizzBuzz como kata: imprimir números de 1 a 100, substituindo
   múltiplos de 3 por "Fizz", múltiplos de 5 por "Buzz" e múltiplos de 15 por "FizzBuzz"
2. Numerar os requisitos incrementalmente: R1 (números simples) → R2 (Fizz) →
   R3 (Buzz) → R4 (FizzBuzz)
3. Demonstrar R1 ao vivo antes de liberar prática guiada

**Efeito:** Problema familiar e sem ambiguidade de domínio — participante foca
no ciclo, não no problema.

**Limites:** Não usar FizzBuzz com participantes que já têm experiência em
testes — a simplicidade do problema pode gerar desengajamento.

---

### VAR2 — String Calculator Kata
**Quando usar:** Participantes com familiaridade básica com testes que precisam
de kata com requisitos incrementais mais ricos e múltiplos casos de borda.

**Como acionar:**
1. Usar o enunciado String Calculator (Roy Osherove): função que recebe string
   com números separados por vírgula e retorna a soma
2. Requisitos incrementais: R1 (string vazia = 0) → R2 (1 número) → R3 (2
   números) → R4 (múltiplos números) → R5 (delimitador customizado) → R6
   (negativos lançam exceção)
3. Disponibilizar todos os requisitos numerados — participante avança no próprio
   ritmo dentro do tempo disponível

**Efeito:** Kata com alta densidade de casos de borda — força prática de
refatoração real entre cada requisito.

**Limites:** String Calculator requer ~90 min para completude total. Em sessões
de 60 min, definir até R4 como meta e R5/R6 como bônus.

---

### VAR3 — Ping-Pong TDD
**Quando usar:** Duplas que precisam praticar TDD colaborativo — um escreve o
teste, o outro implementa o código mínimo para passá-lo, alternando a cada
ciclo.

**Como acionar:**
1. Formar duplas (1 participante por máquina com compartilhamento de tela, ou
   pair programming presencial em 1 máquina)
2. Regra Ping-Pong: Participante A escreve teste (Red) → Participante B
   implementa código mínimo (Green) → Participante B escreve próximo teste →
   Participante A implementa → e assim por diante
3. Refatoração é responsabilidade de quem está com o teclado no momento Green
4. Usar qualquer kata (FizzBuzz ou String Calculator) como base

**Efeito:** Treina comunicação técnica implícita via código — o teste é a
especificação que um parceiro escreve para o outro.

**Limites:** Não usar Ping-Pong com participantes em primeiro contato com TDD —
a complexidade da alternância pode obscurecer o aprendizado do ciclo básico.

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 1 | Prática solo com facilitador disponível; ritmo próprio |
| 2 | Dupla padrão ou Ping-Pong TDD (VAR3) |
| 3 | 1 trio com rotação de teclado a cada ciclo |
| 4 | 2 duplas paralelas; revisão coletiva ao final |
| 5+ | **Não recomendado** — dividir em sessões de no máximo 4 |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Frustração ao ver testes falhando | Reforçar antes: "Red é o estado correto e esperado"; poster visual do ciclo sempre visível |
| Pressão de seguir o ciclo sem atalhos | Requisitos numerados previamente — participante sabe o próximo passo |
| Ansiedade com ritmo do parceiro (Ping-Pong) | Oferecer prática solo antes de Ping-Pong |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica:

- Escrever código de produção antes de ter um teste falhando — viola a regra
  central do TDD e elimina o aprendizado sobre design orientado a testes
- Omitir a fase de refatoração — sem Refactor, o ciclo vira Red-Green apenas
  e não demonstra o valor de design incremental
- Remover os requisitos numerados e apresentar o problema completo de uma vez —
  o incrementalismo é o mecanismo pedagógico central
- Usar kata sem casos de borda claros — katas abertos demais geram paralisia
  de análise e desviam o foco do ciclo para o problema
