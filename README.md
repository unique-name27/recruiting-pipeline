# Pipeline Review

A recruiting pipeline review tool for hiring teams, designed like an editorial broadsheet instead of a SaaS dashboard. Drop in an ATS export (Greenhouse-style `.xlsx` / `.csv`), confirm the column mapping once, and get a full report: flow visualization, aging analysis, forecasts, and an executive update you can paste into email.

Everything runs client-side in a single HTML file — no build, no server, and **no data ever leaves your machine**.

## Try it online

| Edition | Link | What it is |
|---|---|---|
| **Stable** | [pipeline-review.html](https://unique-name27.github.io/recruiting-pipeline/pipeline-review.html) | The core report — reviewed features only |
| **Lab** | [pipeline-review-lab.html](https://unique-name27.github.io/recruiting-pipeline/pipeline-review-lab.html) | Everything in stable plus experimental features |
| Classic | [recruitingpipeline.html](https://unique-name27.github.io/recruiting-pipeline/recruitingpipeline.html) | The original dashboard version (kept for reference) |

Press **Sample data** on any edition to explore with a generated 1,800-candidate dataset — no upload needed.

## Stable features

- **Two primary views**: Current pipeline (who's active right now) and Total pipeline (everyone, including rejected), plus historical presets with prior-period comparisons
- **The river** — a custom Sankey flow of candidates through stages, with rejections draining to a bottom band; every ribbon is clickable and filters the whole report
- **Aging board** — every active candidate as a dot positioned by days-in-stage, colored against stage norms; overdue candidates are impossible to miss
- **Attention flags with root-cause investigations** — bottlenecks, overdue candidates, offer-accept drops, and empty funnels, each expanding into a breakdown of where the problem concentrates and who to talk to
- **Requisitions table** — per-req end-to-end funnel with health flags
- **Powerful filtering** — faceted multi-select on every dimension (including hiring manager and any extra column from your file), free-text search, saved views, and click-to-drill from every visualization with back/Escape navigation
- **Robust mapping** — confidence-scored column auto-detection, stage and status normalization for arbitrary ATS vocabularies, mapping profiles remembered per file signature
- **Export PDF** and a copy-paste executive summary

## Lab additions (experimental)

- **Hiring forecast** — per-candidate hire odds from your historical pass rates, a 90-day fan chart, per-req targets with gap analysis, and a **scenario planner** (what if screens were faster / pass rates higher / more applicants?)
- **Time machine** — reconstruct the pipeline as of any past date, watch an animated **replay** of its history, and see composition over time
- **Process analytics** — survival curves and a cohort velocity heatmap that shows the process speeding up or slowing down
- **Action queue** — overdue candidates grouped by owner (coordinator / recruiter / hiring manager) with ready-to-send follow-up messages
- **Stage SLAs**, a **since-last-visit diff**, **Greenhouse job links**, and a **Ctrl+K command palette**
- **Three editions** (Broadsheet / Terminal / Studio), three flow views (River / Board / Funnel), and a Customize screen with a gallery of optional visualizations

## Running locally

Download either HTML file and double-click it. That's the whole install.

## Privacy

All parsing, analysis, and storage happen in your browser (IndexedDB). Uploads are never transmitted anywhere; the pages are static files.
