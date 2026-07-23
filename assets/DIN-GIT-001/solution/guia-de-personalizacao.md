# DIN-GIT-001 — Guia de Customização
## Git em Conflito (Git in Conflict)

> Este guia descreve como acionar cada variability point definido no `rasset.xml`
> e os limites de customização para preservar a integridade da dinâmica.

---

## Variability Points

### VAR1 — Conflito em Arquivo Binário
**Quando usar:** Participantes com experiência sólida em Git que já resolvem
conflitos de texto com facilidade e precisam de desafio adicional.

**Como acionar:**
1. Adicionar ao repositório de treinamento um arquivo binário com conflito
   pré-fabricado (ex.: imagem PNG editada em duas branches com ferramentas
   diferentes, ou arquivo `.xlsx` com dados divergentes)
2. Apresentar a limitação: `git` não consegue fazer merge automático de binários
   — a resolução exige escolher uma versão ou usar ferramenta externa
3. Discutir estratégias: `git checkout --ours`, `git checkout --theirs`,
   ou exportar e reintegrar manualmente

**Efeito:** Expõe limitação estrutural do Git e força decisão de intenção
pura — sem possibilidade de combinação automática.

**Limites:** Usar apenas após C1 e C2 concluídos. Não substituir — acrescentar
como C4 opcional.

---

### VAR2 — Múltiplas Linguagens
**Quando usar:** Times políglotas (ex.: backend Python + frontend JS + serviços
Java) onde conflitos entre linguagens diferentes são realidade cotidiana.

**Como acionar:**
1. Preparar 3 versões do repositório de treinamento — uma em Python, uma em JS,
   uma em Java — com conflitos equivalentes em estrutura mas sintaxe diferente
2. Atribuir uma linguagem por dupla conforme o perfil técnico de cada participante
3. Revisão coletiva (5 min) compara como o mesmo tipo de conflito se manifesta
   diferente em cada linguagem

**Efeito:** Reforça que conflito Git é independente de linguagem — é divergência
de intenção, não de sintaxe.

**Limites:** Não misturar linguagens dentro da mesma dupla — cada dupla resolve
conflitos em sua linguagem principal.

---

### VAR3 — Ambiente Offline
**Quando usar:** Contextos com conectividade limitada (laboratórios sem internet,
eventos corporativos em locais remotos) ou quando se deseja eliminar dependência
de serviços externos.

**Como acionar:**
1. Criar repositório bare local: `git init --bare training-repo.git`
2. Cada dupla clona o repositório bare localmente — sem acesso a GitHub/GitLab
3. Push e pull feitos para o bare local via path do sistema de arquivos
4. Todos os conflitos pré-fabricados devem estar no bare antes de distribuir

**Efeito:** Preserva 100% da experiência de resolução de conflito sem dependência
de rede.

**Limites:** A experiência de PR (pull request) e code review em plataforma
remota é perdida. Compensar mencionando explicitamente no debriefing que PRs
reais funcionam com os mesmos comandos.

---

## Adaptações por Contexto

### Tamanho de equipe
| Participantes | Configuração recomendada |
|--------------|--------------------------|
| 2 | 1 dupla; facilitador disponível como suporte contínuo |
| 3–4 | 1–2 duplas; facilitador circula entre duplas |
| 5–6 | 2–3 duplas; revisão coletiva obrigatória após C1 |
| 7+ | **Não recomendado** — dividir em duas sessões de no máximo 6 |

### Perfil sensorial (TEA)
| Gatilho | Adaptação |
|---------|-----------|
| Medo de quebrar o repositório | Comunicar antes: "este repositório pode ser recriado em 30 segundos" |
| Mensagens de erro percebidas como falha | Projetar diff com VS Code / GitKraken — não terminal puro |
| Pressão de tempo | Remover cronômetro visível; substituir por checkpoints do facilitador |

---

## Limites de Customização

As seguintes alterações **invalidam** a integridade da dinâmica:

- Pular C1 (Merge Simples) e começar por C2 ou C3 — o escalonamento de
  complexidade é estrutural; sem C1, participantes chegam a C2 sem base
- Solicitar resolução individual sem suporte em dupla para participantes em
  onboarding — o isolamento amplifica a ansiedade com erros Git
- Omitir a narrativa do conflito (quem, o quê, qual branch) — sem contexto,
  a resolução vira exercício mecânico e perde o aprendizado sobre intenção
- Usar apenas terminal sem ferramenta visual de diff — inviabiliza acessibilidade
  sensorial e aumenta barreira de entrada desnecessariamente
