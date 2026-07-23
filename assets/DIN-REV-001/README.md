# DIN-REV-001 — CRSG (Code Review Simulation Game)

> **Grupo:** Habilidades Técnicas | **Temática:** Revisão de Código | **Momento:** Meio de Sprint

---

## 1. Identificação

| Campo | Valor |
|-------|-------|
| **Asset ID** | DIN-REV-001 |
| **Nome** | CRSG — Code Review Simulation Game |
| **Versão RAS** | 3.0 |
| **Autor** | Equipe RAS — ras-dinamicas@institucional.br |
| **Domínio** | Habilidades Técnicas |
| **Subdomínio** | Revisão de Código |
| **Status** | Em validação interna |
| **Criação** | 2025-01-01 |
| **Última Atualização** | 2026-05-05 |
| **Licença** | CC-BY 4.0 |

**Tags:** `Revisão de Código` `Detecção de Defeitos` `Refatoração` `Feedback Técnico` `Onboarding`

---

## 2. Contexto

Simulação de code review em que participantes recebem trechos de código com defeitos intencionais e devem identificá-los usando checklists estruturados, além de redigir comentários de revisão construtivos.

**Objetivo de aprendizagem:** Desenvolver capacidade de identificar defeitos sistematicamente e fornecer feedback técnico construtivo. Fundamentado nos construtos E1.x (Aprendizado) e E2.x (Confiança), conforme Ju et al., ICSE 2021, Tabela III.

---

## 3. Artefatos

| ID | Artefato | Tipo | Papel | Localização |
|----|----------|------|-------|-------------|
| ART-08A | Códigos-fonte com defeitos | TXT | Entrada | DIN-REV-001/codigos_defeitos.txt |
| ART-08B | Checklists de revisão | Markdown | Entrada | DIN-REV-001/checklists_revisao.md |
| ART-08C | Guia do Facilitador | Markdown | Entrada | DIN-REV-001/guia_facilitador.md |
| ART-08D | Ficha KPI | XLSX | Saída | DIN-REV-001/registro_kpi.xlsx |

---

## 7. Relacionamentos

| Asset ID | Nome | Tipo | Justificativa |
|----------|------|------|---------------|
| DIN-GIT-001 | Git em Conflito | Similar / Complementar | Conflitos Git surgem naturalmente de revisões de código |
| DIN-TDD-001 | TDD Kata | Similar | Foco comum em qualidade de código |

---

## Referências

- Ardic, T. et al. (2025). *CRSG — Code Review Simulation Game*.
- Ju, A. et al. (2021). *A Case Study of Onboarding in Software Teams*. ICSE 2021.
- Hause, M. et al. (2025). *RAS 3.0*. INCOSE INSIGHT, Vol.28/5.
