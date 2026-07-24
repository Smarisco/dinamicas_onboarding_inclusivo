# RAS-TEA Onboarding Profile — Description

## Profile Identity

| Field | Value |
|-------|-------|
| **Profile Name** | RAS-TEA Onboarding Profile |
| **Profile ID** | TEA-ONB-PROF-2026-0001 |
| **Version** | 1.0 |
| **Status** | Em validação interna |
| **Created** | 2026-01-01 |
| **Last Updated** | 2026-05-17 |
| **License** | CC-BY 4.0 |
| **Namespace** | `http://www.rational.com/ras/rasdefaultprofile2_0` |
| **Schema** | `profile/ras-tea-profile.xsd` |

---

## Derivation Chain

```
OMG Core RAS Specification (v2.2)
  └── id: F1C842AD-CE85-4261-ACA7-178C457018A1
       │
       ├── RAS Default Profile 2.2
       │     └── id: 31E5BFBF-B16E-4253-8037-98D70D07F35F
       │
       └── RAS-TEA Onboarding Profile 1.0  ← this profile
             └── id: TEA-ONB-PROF-2026-0001
```

### id-history value (canonical, used in every rasset.xml)

```
F1C842AD-CE85-4261-ACA7-178C457018A1::31E5BFBF-B16E-4253-8037-98D70D07F35F::TEA-ONB-PROF-2026-0001
```

---

## Purpose

The **RAS-TEA Onboarding Profile** specialises the OMG Reusable Asset Specification Default Profile 2.2 for the context of software-engineering onboarding dynamics designed for and inclusive of people on the Autism Spectrum (TEA — Transtorno do Espectro Autista).

It preserves full backward compatibility with any RAS 2.2-compliant toolchain while adding three additive, non-breaking extensions described below.

---

## Additive Extensions

### Extension 1 — Mandatory Classification Section

Every asset conforming to this profile **must** include a `<classification>` section (RAS Sec. 6.4.3) with at least the following three context elements:

| Context ID | Name | Required Descriptor Names |
|------------|------|--------------------------|
| `ctx-habilidades` | Eixo de Habilidades | `habilidades-tecnicas`, `habilidades-nao-tecnicas` |
| `ctx-sensorial` | Eixo de Perfil Sensorial | `dimensao-sensorial` |
| `ctx-sprint` | Eixo de Contexto Ágil | `momento-sprint` |

The `momento-sprint` descriptor accepts exactly three values: `inicio`, `meio`, or `fim`.

### Extension 2 — Three Mandatory Classification Contexts

The three contexts `ctx-habilidades`, `ctx-sensorial`, and `ctx-sprint` are **mandatory** in every conforming asset. A validator implementing this profile must reject any `rasset.xml` that lacks any one of these three context declarations.

Rationale: these axes are the primary navigation dimensions used in `catalog.xml`, `SUMMARY.md`, and the GitBook interface. Without them an asset cannot be properly filtered or sequenced in an onboarding journey.

### Extension 3 — Two Mandatory Solution Artifacts

Every conforming asset **must** include at least two artifacts in its `<solution>` section (RAS Sec. 6.4.6) with the following artifact types:

| Required Type | Description |
|---------------|-------------|
| `cartao-facilitador` | Facilitator card providing step-by-step execution instructions, time-boxes, and sensory-safety cues for the activity facilitator. |
| `template-debriefing` | Debriefing template for post-activity structured reflection, aligned with ICSE 2021 constructs (E1–E3). |

Additional artifact types (`checklist`, `customization-guide`, etc.) are permitted but not required.

---

## Accessibility Compliance — OAP-1.0

All assets conforming to this profile must also comply with the **Onboarding Accessibility Profile version 1.0 (OAP-1.0)**, which defines:

- Sensory trigger identification (`sensoryTriggers` field)
- Adaptations for sensory sensitivities (`sensoryAdaptations`)
- Communication support accommodations (`communicationSupports`)
- Predictability structures (`predictabilityStructures`)
- Facilitator readiness checklist (`facilitatorReadiness`)

OAP-1.0 metadata is stored in `profile_info.json` alongside each asset and is referenced in the `dimensao-sensorial` descriptor of the classification section.

---

## Related Standards and References

- OMG. (2005). *Reusable Asset Specification, v2.2*. OMG Document formal/2005-11-02.
- Hause, M. et al. (2025). *RAS 3.0*. INCOSE INSIGHT, Vol.28/5.
- Ju, A. et al. (2021). *A Case Study of Onboarding in Software Teams*. ICSE 2021.
- Edmondson, A. (1999). *Psychological Safety and Learning Behavior in Work Teams*. Administrative Science Quarterly.
