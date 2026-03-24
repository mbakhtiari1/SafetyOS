# 🛡️ SafetyOS

**An Open-Source Safety and Quality Management Learning Platform for Radiation Oncology**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-mbakhtiari1.github.io%2FSafetyOS-blue?style=for-the-badge)](https://mbakhtiari1.github.io/SafetyOS)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

> **SafetyOS is a learning platform and clinical governance scaffold — not clinical decision support software. All generated checklists require clinical review and physician approval before any clinical application.**

---

## What is SafetyOS?

SafetyOS is a single-file, zero-installation safety and quality management platform for radiation oncology departments. It implements the daily safety management system architecture described in [Bakhtiari (PLOS Digital Health, 2025)](https://doi.org/10.1371/journal.pdig.0000669), connecting incident learning, proactive risk assessment, process mapping, daily operational management, and policy governance in a closed Plan-Do-Study-Act loop.

It is designed for:
- **Residents** beginning their safety science education
- **Community physicists** who need a structured entry point into TG-100 and systems-theoretic safety methods
- **Departments** that want to operationalize safety management without vendor contracts or IT infrastructure

**No installation. No server. No internet connection required.** One HTML file. Any browser. Any computer. Any clinic.

---

## 🚀 Quick Start

**Option 1 — Use the live web version (recommended):**
👉 [https://mbakhtiari1.github.io/SafetyOS](https://mbakhtiari1.github.io/SafetyOS)

**Option 2 — Download and run locally:**
1. Download `index.html` from this repository
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Click **Start Fresh** to load demo data and literature examples

---

## Features

### Five Integrated Modules

| Module | Purpose | Methods |
|---|---|---|
| 📋 **Daily Huddle** | Operational safety review | Plan-Do-Study-Act daily management |
| 🗺️ **Process Maps** | RT workflow visualization with risk coloring | TG-100 process mapping; STAMP control structure perspective |
| 🔍 **ILS & RCA** | Incident learning and root cause analysis | Ford et al. (2012) event taxonomy; 5 Whys; CAST-informed analysis |
| ⚠️ **Risk Assessment** | Proactive FMEA and STPA | TG-100 FMEA; STPA (Leveson 2004) |
| 📁 **P&P Audit** | Policy governance with ILS linkage | Bidirectional incident-to-policy tracing |

### Pre-Loaded Literature Examples

SafetyOS ships with real incidents and risk assessment projects from published safety science papers — not hypothetical examples:

**Incidents (ILS):**
- **LIT001** — Rectal cancer isocenter error, 10 cm superior to intended location. Analyzed with all four methods: RCA, London Protocol, AcciMap, and CAST. *(Wong & Pawlicki, JACMP 2025; Gosbee & Anderson, BMJ 2003)*
- **LIT002** — Wrong SGRT reference surface loaded for breast patient. *(Wong & Pawlicki, JACMP 2025 — primary CAST worked example)*
- **LIT003** — Treatment plan transferred to R&V before approval (STPA UCA 49 — found by STPA, missed by 7-year HFMEA). *(Silvis-Cividjian et al., Safety Science 2020)*

**Risk Assessment Projects:**
- FMEA: Surface-Guided Cranial Radiosurgery — *(Manger, Paxton, Pawlicki, Kim, Med Phys 2015)*
- FMEA: AI Auto-Contouring & Automated Planning — *(Nealon, Balter, Court et al., Pract Radiat Oncol 2022)*
- FMEA: New Technology Implementation & Commissioning — *(Pawlicki et al., Med Phys 2019)*
- STPA: RT Clinical Operations (Halcyon) — 10 UCAs, 73% non-technical finding — *(Pawlicki et al., Med Phys 2019)*
- STPA: IMRT Process UCAs That FMEA Missed — 8 Wrong Timing UCAs — *(Silvis-Cividjian et al., Safety Science 2020)*

### Key Design Decisions

- **Ford et al. (2012) event type taxonomy** — Process Improvement / Unsafe Condition / Near Miss / Incident, separate from severity scoring
- **Causality distribution chart** benchmarked against the Pawlicki et al. (2019) finding that **73% of RT causal scenarios are non-technical**
- **CAST-informed analysis panel** auto-appears for Significant and Serious incidents — based on STAMP/CAST (Leveson 2004; Wong & Pawlicki 2025)
- **ILS → P&P bidirectional linkage** — incidents flag policies for review; policies display linked incident counts
- **FMEA checklist extraction** — generates role-separated, RPN-filtered checklists (DRAFT, requires clinical review)
- **TG-100 FMEA templates** pre-linked to the built-in 15-step RT process map

---

## The 73% Finding

Pawlicki et al. (2019) performed a full STPA safety assessment of the Halcyon system and found that **73% of causal scenarios in routine radiation therapy are non-technical** — organizational management 33%, procedural 23%, human behavior 14%. Only 27% were equipment-related.

Most radiation oncology safety programs address the 27% technical side. SafetyOS is designed to make the 73% visible and actionable.

---

## Data and Privacy

All data is stored in **browser localStorage** — it never leaves your computer. No data is sent to any server. Export your data regularly using the **Save CSV** button.

> **Note:** Browser localStorage is not suitable for multi-user clinical production use. Each user maintains their own independent data store. Export CSV to share data between users or computers.

---

## Citation

If you use SafetyOS in research, education, or clinical work, please cite:

```
Bakhtiari M. SafetyOS: An Open-Source Safety and Quality Management Learning 
Platform for Radiation Oncology. Pract Radiat Oncol. [Under Review] 2025.
```

This platform implements the architecture described in:

```
Bakhtiari M. Process mining applications in radiation oncology quality management: 
a framework for daily safety management system implementation. 
PLOS Digital Health. 2025. https://doi.org/10.1371/journal.pdig.0000669
```

---

## References

This platform integrates evidence from the following published works:

1. Huq MS, et al. The report of Task Group 100 of the AAPM. *Med Phys.* 2016;43(7):4209–4262.
2. Ford EC, et al. Consensus recommendations for incident learning database structures in radiation oncology. *Med Phys.* 2012;39(12):7272–7290.
3. Pawlicki T, et al. Clinical safety assessment of the Halcyon system. *Med Phys.* 2019;46(10):4340–4345.
4. Silvis-Cividjian N, et al. Using a systems-theoretic approach to analyze safety in radiation therapy. *Safety Science.* 2020;122:104519.
5. Wong LM, Pawlicki T. A review of accident models and incident analysis techniques. *J Appl Clin Med Phys.* 2025;26:e14623.
6. Manger RP, et al. FMEA and fault tree analysis of surface image guided cranial radiosurgery. *Med Phys.* 2015;42(5):2449–2461.
7. Nealon KA, et al. Using FMEA to evaluate risk in the clinical adoption of automated contouring and treatment planning tools. *Pract Radiat Oncol.* 2022;12(4):e344–e353.
8. Leveson NG. A new accident model for engineering safer systems. *Safety Science.* 2004;42(4):237–270.
9. Gosbee J, Anderson T. Human factors engineering design demonstrations can enlighten your RCA team. *BMJ Qual Saf.* 2003;12(2):119–121.

---

## License

MIT License — free to use, modify, and distribute with attribution.

---

## Author

**Mohammad Bakhtiari, PhD, DABR, EMBA, CPHQ, CPPS, CSSBB**  
Senior Medical Physicist, WellSpan Radiation Oncology  
Chair, AAPM Risk Assessment Working Group

---

*SafetyOS is free, open-source, and requires no installation. One HTML file. Any browser. Any computer. Any clinic.*
