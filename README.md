# Time-Compressed Employability Model

A two-part analytical framework examining why formal education systematically underdelivers on skill relevance at graduation — and why the trajectory after entry depends entirely on the nature of the skills acquired.

**[→ View the live report](https://zerobline.github.io/Time-Compressed-Employability-Model/)**

---

## What this is

This is a single-file static HTML report presenting an original strategic framework for understanding the economic value of formal education over time. It combines analytical writing, mathematical modelling, and data visualisation into a document designed to be read, shared, and cited.

The framework was developed across two versions, both included in the report:

- **Version 1** establishes the *pre-entry* problem: structural curriculum lag and study duration compress the window of employability before a graduate even enters the workforce.
- **Version 2** extends the model *post-entry*: not all skills decay at the same rate. Some compound. The model identifies which, why, and what determines the difference.

---

## The framework at a glance

### Version 1 — The compression problem

Every graduate enters the labour market with a structural deficit. Two delays combine to shrink the Effective Employability Window (EEW):

| Component | Description |
|-----------|-------------|
| **A — Curriculum lag** | Time between a skill becoming market-relevant and a university incorporating it into its programme |
| **B — Study duration** | Time spent completing the degree while market conditions continue to evolve |
| **L = A + B** | Total lag at graduation |
| **EEW** | What remains: Total Skill Lifespan − L |

**Core equation:**
```
EEW = Total Skill Lifespan − (A + B)
```

**Value curve (linear approximation):**
```
Skill Value(t) = Peak − Decay × (t − t₀)     where t₀ = A + B
```

The key insight: skills are *already partially obsolete* at the moment they are first applied. This is not a graduate's failure — it is an architectural feature of how education systems are structured.

### Version 2 — The post-entry divergence

Version 1 treats all skills as equivalent after graduation. Version 2 corrects this. It introduces a third force — **compounding (κ)** — alongside decay (δ), splitting the post-graduation trajectory into three distinct paths:

| Trajectory | Formula | Skill type |
|------------|---------|------------|
| **Compounding** | V(t) = V₀ · e^(κt) | Abstract, transferable, leveraged skills |
| **Decay** | V(t) = V₀ · e^(−δt) | Tool-bound, context-specific skills |
| **Hybrid arc** | Slight decay → compounding | Most real careers |

**Four determinants of whether a skill compounds:**

1. **Transferability** — applies across domains, roles, and industries; not locked to one context
2. **Abstraction level** — higher-order principles outlast implementations; frameworks outlast syntax
3. **Feedback loops** — practised repeatedly with legible outcomes; gets sharper, not rustier
4. **Leverage potential** — amplifies other skills or other people's output; returns scale with use

**The headline:**
> *Lag explains where you start. Decay and compounding determine where you end.*

---

## Repository contents

```
.
├── index.html      # Full report — self-contained, no dependencies
└── README.md       # This file
```

The entire report is a **single HTML file with zero external dependencies** at runtime. Fonts are loaded from Google Fonts; everything else — layout, charts, SVG visualisations, and prose — is inline.

---

## Deploying to GitHub Pages

1. **Fork or clone** this repository
2. Go to **Settings → Pages**
3. Under *Source*, select `Deploy from a branch`
4. Choose `main` (or `master`) and `/ (root)`
5. Click **Save**

Your report will be live at:
```
https://[your-username].github.io/[your-repo-name]/
```

If the file is named `index.html`, it will serve automatically. If you've kept the filename as `employability_model_report.html`, either rename it to `index.html` or update the Pages source path accordingly.

---

## Design

The report is designed to read like a professional strategy document — the aesthetic is deliberately close to what you'd find from a top-tier management consultancy: restrained typography, structured prose, ruled exhibit frames, and data visualisation that earns its place analytically rather than decoratively.

**Typography:** EB Garamond (display, pull quotes, formulas) + DM Sans (body, labels, metadata)

**Colour palette:**

| Role | Value | Usage |
|------|-------|-------|
| Cover / key message | `#1c2333` | Deep slate-navy — primary dark surface |
| Market relevance | `#0F6E56` | Teal — the "ideal" benchmark curve |
| Education output | `#BA7517` | Amber — the lagging delivered curve |
| Relevance gap | `#E24B4A` | Red — compression and deficit |
| Compounding | `#534AB7` | Purple — κ > 0 trajectory |
| Hybrid arc | `#1D9E75` | Teal-light — the realistic career path |

**Visualisations:** Hand-authored SVG, inline in the HTML. No charting library required. Curves are illustrative — they represent structural tendencies, not empirically fitted regressions.

---

## Who this is for

This framework is relevant to anyone thinking about the economics of learning, skills, and careers:

- **Students and graduates** auditing their own skill portfolios for compounding potential
- **Education designers and curriculum strategists** identifying where lag compression is most damaging and how to reduce it
- **HR and talent leaders** evaluating what to look for beyond credentials at hiring
- **Researchers and policy analysts** working on future-of-work, human capital, or education reform
- **Career coaches and advisors** helping clients build strategies that account for post-entry skill dynamics

---

## Limitations and methodological notes

The curves in this framework are illustrative. They represent structural tendencies derived from analytical reasoning, not empirically fitted regressions. The exponential form V(t) = V₀·e^(κt) and V(t) = V₀·e^(−δt) is chosen for analytical tractability and qualitative accuracy; actual skill value functions are likely more complex, discontinuous, and context-dependent.

The framework is designed as a **strategic thinking tool**, not a predictive model. Rate constants κ (compounding) and δ (decay) vary significantly by field, individual, and institutional context. Readers should calibrate these to their own domain's observed rates of skill obsolescence.

---

## Licence

This work is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt it for any purpose, including commercial use, with attribution.

If you use this framework in a presentation, article, or report, a link back to this repository is appreciated but not required.

---

## Contributing

Ideas for extensions are welcome via Issues:

- Empirical calibration of κ and δ by industry or skill category
- Interactive version with adjustable parameters (A, B, κ, δ)
- Additional scenarios: bootcamp vs degree, continuous learning models, AI-accelerated obsolescence
- Translations

Pull requests for corrections to the analytical framing or prose are also welcome.

---

*Framework developed 2025. Report design and visualisations produced with Claude (Anthropic).*


