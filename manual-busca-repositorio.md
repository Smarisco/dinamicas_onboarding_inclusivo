# Manual de Busca no Repositório de Dinâmicas de Onboarding Inclusivo

> Como encontrar a dinâmica certa combinando **habilidade da sprint**, **perfil do profissional** e **momento da sprint**, usando a busca do GitHub (operador `path:assets` + frases entre aspas) e o **GitHub Copilot** (linguagem natural).

Repositório: `Smarisco/dinamicas_onboarding_inclusivo`

---

## 1. Por que buscar assim

O gestor sabe três coisas ao iniciar uma sprint, mas não tem um mecanismo formal para combiná-las:

| # | Variável | O que é | Onde aparece no repositório |
|---|----------|---------|-----------------------------|
| 1 | **Habilidades da sprint** | Técnicas e não técnicas demandadas no ciclo | `README.md` (campos *Grupo*, *Temática*, *Mapeamento de Habilidades*) e `rasset.xml` (`habilidades-tecnicas`, `habilidades-nao-tecnicas`) |
| 2 | **Perfil do profissional** | Sensibilidades sensoriais e cognitivas do profissional com TEA | `rasset.xml` (`dimensao-sensorial`) e `solution/cartao-facilitador.md` |
| 3 | **Momento da sprint** | Início, meio ou fim do ciclo de onboarding | `README.md` (*Início/Meio/Fim de Sprint*) e `rasset.xml` (`momento-sprint`: `inicio`, `meio`, `fim`) |

Cada dinâmica é um ativo em `assets/DIN-XXXX-00N/`, com `README.md`, `rasset.xml` e a pasta `solution/`. Buscar **somente dentro de `assets`** evita ruído de `README.md` da raiz, `SUMMARY.md`, `catalog.xml` e `profile/`.

---

## 2. A fórmula da busca

```
repo:Smarisco/dinamicas_onboarding_inclusivo "termo 1" "termo 2" "termo 3" path:assets
```

| Parte | Função |
|-------|--------|
| `repo:Smarisco/dinamicas_onboarding_inclusivo` | Restringe a busca a este repositório (o GitHub já preenche ao buscar de dentro do repo) |
| `"termo"` | **Frase exata**: o texto entre aspas deve aparecer literalmente. Sem aspas, o GitHub trata cada palavra separadamente |
| Vários termos | Funcionam como **E** (AND): o arquivo precisa conter todos |
| `path:assets` | **Sempre no final.** Limita os resultados ao diretório `assets/` |

### Exemplo da imagem

```
repo:Smarisco/dinamicas_onboarding_inclusivo "gestão ágil" "Comunicação" "Início " path:assets
```

Lê-se: *arquivos dentro de `assets` que contenham "gestão ágil" **e** "Comunicação" **e** "Início"*.

Resultado esperado: **`DIN-AGIL-001/README.md`** (Jogo das Bolinhas), cujo domínio é "Gestão Ágil", que trabalha "Comunicação Explícita" e ocorre no "Início de Sprint".

---

## 3. Passo a passo

1. Abra o repositório no GitHub e clique na barra de busca (ou pressione `/`).
2. Escreva os termos entre aspas, **um por variável** (habilidade, perfil, momento).
3. Termine com `path:assets`.
4. Pressione **Enter** e, na página de resultados, escolha **Code**.
5. Abra o `README.md` da dinâmica encontrada para ver o guia completo; use `solution/cartao-facilitador.md` para aplicá-la.

---

## 4. Vocabulário que existe nos arquivos (use estes termos)

A busca é por texto: só encontra o que está escrito. Use exatamente estas formas.

### 4.1 Momento da sprint

| Onde buscar | Início | Meio | Fim |
|-------------|--------|------|-----|
| `README.md` e `cartao-facilitador.md` | `"Início de Sprint"` | `"Meio de Sprint"` | `"Fim de Sprint"` |
| `rasset.xml` (**sem acento**) | `"inicio"` | `"meio"` | `"fim"` |

> **Atenção ao acento:** o GitHub diferencia `Início` de `inicio`. Em `README.md` o texto tem acento; em `rasset.xml` o valor técnico não tem. Para achar nos dois, prefira `"Início de Sprint"` (README) ou faça uma segunda busca com `"inicio"`.

Distribuição atual: 3 dinâmicas no início, 4 no meio, 5 no fim.

### 4.2 Habilidades (grupo e temática)

| Grupo | Termo de busca |
|-------|----------------|
| Técnicas | `"Habilidades Técnicas"` |
| Não técnicas | `"Habilidades Não Técnicas"` |

Temáticas existentes: Metodologias Ágeis, Comunicação, Feedback, Controle de Versão, Autoadvocacia, Estimativa Ágil, Segurança Psicológica, Cerimônias Ágeis, Revisão de Código, Colaboração em Pares, Qualidade.

Habilidades específicas que podem ser usadas como termo: `"Escuta Ativa"`, `"Segurança Psicológica"`, `"Feedback Estruturado"`, `"Test-Driven Development"`, `"Story Points"`, `"Comunicação Assertiva"`, `"Refatoração"`, `"Autorregulação"`, entre outras (veja `rasset.xml`, descritores `habilidades-*`).

### 4.3 Perfil sensorial do profissional

Os gatilhos sensoriais estão descritos em linguagem natural no descritor `dimensao-sensorial`. Termos que existem:

| Sensibilidade | Termo de busca |
|---------------|----------------|
| Ruído / som abrupto | `"Ruído"`, `"Barulho"`, `"Sinal sonoro abrupto"` |
| Aglomeração / espaço | `"Aglomeração"` |
| Pressão de tempo | `"Pressão de tempo"` |
| Feedback inesperado | `"Feedback inesperado"` |
| Exposição em grupo | `"Pressão de revelar vulnerabilidade em grupo"` |
| Fala em tempo real | `"Pressão de formular resposta verbal em tempo real"` |
| Restrição sensorial | `"Venda ou objeto cobrindo os olhos"` |
| Múltiplas vozes | `"Múltiplas vozes simultâneas"` |

> **Leitura correta do perfil:** esses termos descrevem o que a dinâmica **pode causar** de desconforto. Para um profissional sensível a ruído, o objetivo é **encontrar o que evitar ou o que adaptar**. Abra o `solution/guia-de-personalizacao.md` da dinâmica para ver as variações (pontos de variabilidade `VAR1`, `VAR2`...).

---

## 5. Receitas prontas

| Objetivo | Busca |
|----------|-------|
| Dinâmica técnica para **início** de sprint | `"Habilidades Técnicas" "Início de Sprint" path:assets` |
| Dinâmica não técnica para **fim** de sprint | `"Habilidades Não Técnicas" "Fim de Sprint" path:assets` |
| Comunicação no **meio** da sprint | `"Comunicação" "Meio de Sprint" path:assets` |
| Segurança psicológica no fim | `"Segurança Psicológica" "Fim de Sprint" path:assets` |
| Dinâmicas que envolvem **pressão de tempo** | `"Pressão de tempo" path:assets` |
| Dinâmicas com **ruído** (para adaptar/evitar) | `"Ruído" path:assets` |
| Combinação completa (exemplo da imagem) | `"gestão ágil" "Comunicação" "Início " path:assets` |
| Dinâmicas de uma pasta específica | `"Início de Sprint" path:assets/DIN-AGIL-001` |

Sempre inclua o prefixo `repo:Smarisco/dinamicas_onboarding_inclusivo` quando buscar fora do repositório.

---

## 6. Buscando com o GitHub Copilot (linguagem natural)

O Copilot (ícone no canto superior direito do GitHub) é um **aliado complementar**. Ele aceita perguntas em português, sem operadores e sem aspas, e o contexto já vem com o repositório selecionado (caixa inferior mostrando `Smarisco/dinamicas_onboar...`).

### Quando usar cada um

| Use a busca com `path:assets` quando... | Use o Copilot quando... |
|------------------------------------------|--------------------------|
| Você sabe os termos exatos | Você descreve a situação, não os termos |
| Quer **lista completa e auditável** de arquivos | Quer **recomendação explicada** e comparação |
| Precisa de resultado reproduzível | Quer resumir, comparar ou adaptar uma dinâmica |

### Exemplos de perguntas

```
Quais dinâmicas servem para o início da sprint e trabalham habilidades técnicas?
```
```
Tenho um profissional com TEA sensível a ruído. Quais dinâmicas do meio da sprint devo evitar ou adaptar?
```
```
Compare DIN-FEED-001 e DIN-PSAF-001: habilidades, momento da sprint e riscos sensoriais.
```
```
Quero trabalhar comunicação sem exigir resposta verbal imediata. O que o repositório oferece?
```
```
Resuma o cartão do facilitador da DIN-AGIL-001 em 5 passos.
```

### Boas práticas com o Copilot

- Cite as **três variáveis** na pergunta: habilidade, perfil sensorial, momento da sprint.
- Peça sempre **o ID da dinâmica** (`DIN-...`) e **o arquivo de origem** da informação.
- **Confirme** abrindo o `README.md` ou o `rasset.xml` citado: o Copilot pode errar ou omitir ativos.
- Para decisões de seleção, **repita a busca textual** (seção 5) e compare as duas respostas.

---

## 7. Fluxo recomendado

```
1. Defina: habilidade  +  perfil sensorial  +  momento da sprint
2. Busca textual (path:assets)  →  candidatas
3. Copilot  →  comparar candidatas e riscos sensoriais
4. Abrir README.md  →  confirmar grupo, temática e momento
5. Abrir solution/guia-de-personalizacao.md  →  adaptar ao perfil
6. Aplicar com solution/cartao-facilitador.md + checklist.md
7. Fechar com solution/modelo-debriefing.md
```

---

## 8. Solução de problemas

| Sintoma | Causa provável | Correção |
|---------|----------------|----------|
| Nenhum resultado | Acento ou grafia diferente do arquivo | Teste sem acento (`inicio`) ou com a forma exata do README (`Início de Sprint`) |
| Nenhum resultado com 3+ termos | Os termos estão em arquivos diferentes (a busca é **por arquivo**) | Reduza para 2 termos ou use o `README.md`, que concentra habilidade, temática e momento |
| Resultados demais | Termo genérico (ex.: `"Comunicação"`) | Combine com o momento e o grupo |
| Resultados fora de `assets` | `path:assets` ausente ou no início | Coloque `path:assets` no **final** |
| Resultado vazio de `rasset.xml` | Valor técnico sem acento | Use `"inicio"`, `"meio"`, `"fim"` |
| Copilot cita dinâmica inexistente | Alucinação | Confirme o ID em `catalog.xml` (lista os 12 ativos) |

---

## 9. Catálogo rápido (12 dinâmicas)

| ID | Dinâmica | Grupo | Momento |
|----|----------|-------|---------|
| DIN-AGIL-001 | Jogo das Bolinhas | Técnica | Início |
| DIN-AGIL-002 | Construção com Blocos | Técnica | Início |
| DIN-PLAN-001 | Planning Poker | Técnica | Início |
| DIN-GIT-001 | Git em Conflito | Técnica | Meio |
| DIN-TDD-001 | TDD Kata | Técnica | Meio |
| DIN-REV-001 | CRSG (Revisão de Código) | Técnica | Meio |
| DIN-COM-001 | O Campo Minado | Não técnica | Meio |
| DIN-MAND-001 | Peço, Logo Recebo | Não técnica | Fim |
| DIN-SOFT-001 | A Moeda de Duas Faces | Não técnica | Fim |
| DIN-RETRO-001 | Retrospectiva Guiada | Não técnica | Fim |
| DIN-FEED-001 | Feedback em 4 Passos | Não técnica | Fim |
| DIN-PSAF-001 | Termômetro Psicológico | Não técnica | Fim |

Navegação alternativa sem busca: `SUMMARY.md` organiza o repositório pelos três eixos (momento, grupo de habilidades, perfil sensorial).
