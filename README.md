# Repositório de Dinâmicas de Onboarding

> Repositório de dinâmicas estruturadas como ativos reutilizáveis para o ensino e integração de engenheiros de software com Transtorno do Espectro Autista (TEA).

---

## Sobre este repositório

Este repositório organiza dinâmicas de onboarding modeladas segundo o padrão **Reusable Asset Specification (RAS)** da OMG. Cada dinâmica é um ativo versionado, descrito por um manifesto `rasset.xml` conforme o **RAS-TEA Onboarding Profile** (especialização do RAS Default Profile 2.2), que permite ao gestor **descobrir, selecionar e aplicar** a prática adequada ao perfil do profissional e ao momento da sprint — sem depender de memória institucional.

A abordagem transforma práticas de integração isoladas em ativos **descobríveis, versionados e reproduzíveis** por qualquer equipe, com ou sem experiência prévia em neurodiversidade.

> **Artigo:** Repositório de Dinâmicas Reutilizáveis: Promovendo o Onboarding Inclusivo para Engenheiros de Software com TEA — Stela Marisco Duarte, Daniel Vitoriano Santos, Maria Istela Cagnin. SBES 2026 (CBSoft 2026). [PREENCHER: link do artigo aceito]

---

## Ponto de entrada

| Arquivo | Descrição |
|---------|-----------|
| [`catalog.xml`](catalog.xml) | Catálogo raiz — lista todos os 12 ativos com metadados de classificação |
| [`profile/descricao-perfil.md`](profile/descricao-perfil.md) | Documentação do RAS-TEA Onboarding Profile |
| [`profile/ras-tea-profile.xsd`](profile/ras-tea-profile.xsd) | Schema XSD do perfil — validação dos `rasset.xml` |
| [`SUMMARY.md`](SUMMARY.md) | Navegação GitBook por três eixos de classificação |

---

## Estrutura do repositório

```
dinamicas-onboarding/
│
├── catalog.xml                  ← Catálogo raiz (entrada principal)
│
├── profile/
│   ├── ras-tea-profile.xsd      ← Schema XSD do perfil RAS-TEA
│   └── descricao-perfil.md     ← Documentação do perfil
│
├── assets/
│   ├── DIN-AGIL-001/            → Jogo das Bolinhas
│   │   ├── rasset.xml           ← Manifesto RAS canônico
│   │   ├── README.md            ← Documentação legível
│   │   └── solution/
│   │       ├── cartao-facilitador.md
│   │       ├── modelo-debriefing.md
│   │       ├── checklist.md
│   │       └── guia-de-personalizacao.md
│   ├── DIN-AGIL-002/ …
│   ├── DIN-GIT-001/  …
│   ├── DIN-PLAN-001/ …
│   ├── DIN-TDD-001/  …
│   ├── DIN-REV-001/  …
│   ├── DIN-MAND-001/ …
│   ├── DIN-RETRO-001/…
│   ├── DIN-SOFT-001/ …
│   ├── DIN-COM-001/  …
│   ├── DIN-FEED-001/ …
│   └── DIN-PSAF-001/ …
│
├── SUMMARY.md                   ← Navegação GitBook
└── README.md
```

---

## Manifesto canônico: rasset.xml

O arquivo `rasset.xml` em cada diretório de ativo é o **manifesto RAS canônico**. Ele é a fonte de verdade para consumo por ferramentas RAS-compatíveis.

Estrutura mínima de um `rasset.xml` conforme o RAS-TEA Profile:

```xml
<asset xmlns="http://www.rational.com/ras/rasdefaultprofile2_0" …>
  <profile name="RAS-TEA Onboarding Profile"
    id-history="F1C842AD-…::31E5BFBF-…::TEA-ONB-PROF-2026-0001" …/>
  <classification
    context="" descriptor=""
    habilidades-tecnicas="…" habilidades-nao-tecnicas="…"
    dimensao-sensorial="…" momento-sprint="inicio|meio|fim"
    duracao="…" qtd-min-participantes="…" qtd-max-participantes="…"
    modalidade="…" publico-alvo="…"/>
  <solution>
    <!-- cartao-facilitador e modelo-debriefing obrigatórios -->
  </solution>
  <usage>…</usage>
  <related-asset …/>
</asset>
```

---

## Classificação tridimensional

Cada dinâmica é classificada segundo três eixos ortogonais que permitem filtragem precisa:

| Eixo  | O que classifica | Exemplo |
|-------------------|-----------------|---------|
| `Eixo de Habilidades` | habilidades técnicas/não técnicas desenvolvidas | Comunicação assertiva, controle de versão |
| `Eixo de Perfil Sensorial` | Dimensões de neurodiversidade endereçadas | Sensibilidade auditiva, previsibilidade |
| `Eixo de Contexto Ágil` | Momento da sprint: `inicio`, `meio` ou `fim` | Retrospectiva → fim |

---

## Ativos instanciados

| ID | Nome | Grupo | Momento | Modalidade |
|----|------|-------|---------|------------|
| DIN-AGIL-001 | Jogo das Bolinhas | Habilidades Técnicas | início | presencial |
| DIN-AGIL-002 | Construção com Blocos | Habilidades Técnicas | início | presencial |
| DIN-GIT-001 | Git em Conflito | Habilidades Técnicas | meio | digital |
| DIN-PLAN-001 | Planning Poker | Habilidades Técnicas | início | presencial |
| DIN-TDD-001 | TDD Kata | Habilidades Técnicas | meio | digital |
| DIN-REV-001 | CRSG | Habilidades Técnicas | meio | digital |
| DIN-MAND-001 | Peço, Logo Recebo | Habilidades Não Técnicas | fim | presencial |
| DIN-RETRO-001 | Retrospectiva Guiada | Habilidades Não Técnicas | fim | presencial ou digital |
| DIN-SOFT-001 | A Moeda de Duas Faces | Habilidades Não Técnicas | fim | presencial |
| DIN-COM-001 | O Campo Minado | Habilidades Não Técnicas | meio | presencial |
| DIN-FEED-001 | Feedback em 4 Passos | Habilidades Não Técnicas | fim | presencial ou digital |
| DIN-PSAF-001 | Termômetro Psicológico | Habilidades Não Técnicas | fim | presencial ou digital |

---

## Como usar este repositório

### Para gestores e mentores

Acesse a documentação navegável no **GitBook** (link abaixo) e filtre as dinâmicas por:
- Momento da sprint (início, meio ou fim)
- Habilidade que deseja desenvolver
- Perfil sensorial do profissional

### Para contribuidores

Siga o fluxo de branches:

```
feat/assets/<DIN-ID>  →  develop  →  main
```

Antes de abrir um Pull Request, certifique-se de que:
- [ ] O diretório `assets/<DIN-ID>/` segue a estrutura padrão
- [ ] O `rasset.xml` está bem-formado e válido contra `profile/ras-tea-profile.xsd`
- [ ] O `catalog.xml` foi atualizado com a nova entrada
- [ ] O `SUMMARY.md` foi atualizado com a nova dinâmica nos três eixos

---

## Requirements

Para inspecionar e validar este artefato não é necessário instalar nenhuma linguagem de programação ou runtime. São suficientes:

- **Leitor de XML** — qualquer editor de texto ou IDE com suporte a XML (ex.: VS Code, IntelliJ, Notepad++) para inspecionar `rasset.xml` e `catalog.xml`.
- **Validador de schema XML** — um dos seguintes:
  - **PowerShell 5.1+** (nativo no Windows 10/11) — usado no passo de validação abaixo.
  - **`xmllint`** (Linux/macOS via `libxml2`) — alternativa equivalente.
- **Visualizador de Markdown** — para leitura dos artefatos em `solution/` e do perfil em `profile/descricao-perfil.md`.
- **Opcional:** conta GitBook para navegação web a partir do `SUMMARY.md`.

---

## Installation

Não há instalação de dependências. Para verificar que o artefato está íntegro, execute o comando abaixo **a partir da raiz do repositório**.

### Windows (PowerShell 5.1+)

```powershell
Get-ChildItem -Path assets -Recurse -Filter rasset.xml |
  ForEach-Object { [xml](Get-Content $_.FullName) | Out-Null; Write-Output "OK: $($_.Directory.Name)/rasset.xml" }
[xml](Get-Content catalog.xml) | Out-Null; Write-Output "OK: catalog.xml"
```

**Saída esperada (sem erros):**
```
OK: DIN-AGIL-001/rasset.xml
OK: DIN-AGIL-002/rasset.xml
OK: DIN-COM-001/rasset.xml
OK: DIN-FEED-001/rasset.xml
OK: DIN-GIT-001/rasset.xml
OK: DIN-MAND-001/rasset.xml
OK: DIN-PLAN-001/rasset.xml
OK: DIN-PSAF-001/rasset.xml
OK: DIN-RETRO-001/rasset.xml
OK: DIN-REV-001/rasset.xml
OK: DIN-SOFT-001/rasset.xml
OK: DIN-TDD-001/rasset.xml
OK: catalog.xml
```

Se algum arquivo estiver malformado, o PowerShell lança uma exceção com o caminho e a linha do erro antes de prosseguir.

### Linux / macOS (xmllint)

```bash
find assets -name rasset.xml | sort | xargs -I{} xmllint --noout {} && \
  xmllint --noout catalog.xml && \
  echo "Todos os arquivos XML: OK"
```

**Saída esperada:** `Todos os arquivos XML: OK` (sem linhas de erro anteriores).

---

## Branches

| Branch | Finalidade |
|--------|-----------|
| `main` | Conteúdo revisado e publicado — sincronizado com o GitBook |
| `develop` | Branch de integração antes da publicação |
| `feat/assets/<DIN-ID>` | Branch de trabalho para nova dinâmica |
| `fix/assets/<DIN-ID>` | Branch de correção de conteúdo existente |
| `update/assets/<DIN-ID>` | Branch de atualização de dinâmica existente |

---

## Convenção de commits

```
feat(assets/DIN-AGIL-001): instancia ativo RAS — Jogo das Bolinhas
fix(assets/DIN-COM-001): corrige variability-point auditivo
update(assets/DIN-PSAF-001): revisa guia do facilitador
docs(root): atualiza catalog.xml e SUMMARY.md
```

---

## Documentação

A versão navegável deste repositório está publicada no GitBook:  
*(link será adicionado após integração)*

---

## Referência

Este repositório é o artefato de suporte ao artigo:

> **Repositório de Dinâmicas Estruturadas como Ativo Reutilizável para o Ensino e Integração de Engenheiros de Software com TEA**  
> Submetido ao SBES 2026.

Protocolos utilizados:
- Object Management Group. *Reusable Asset Specification, Version 2.2*. OMG, 2005.
- Hause, M. et al. (2025). *RAS 3.0*. INCOSE INSIGHT, Vol.28/5.
- Ju, A. et al. (2021). *A Case Study of Onboarding in Software Teams*. ICSE 2021.

---

## Disponibilidade

## Disponibilidade

Os artefatos completos (manifestos rasset.xml e guias de customização) estão
disponíveis publicamente neste repositório, com identificação completa dos autores.
