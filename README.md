# ETHEX: Public Repo

## Repository Structure

```
├── README.md                          ← This file
├── codebook/
│   └── ethex_codebook.csv             ← Full codebook: 69 codes with definitions, frequencies, provenance
├── patterns/
│   └── requirement_patterns.md        ← All 16 explainability requirement patterns (4 roles × 4 clusters)
└── survey/
    └── explanations.md                ← All baseline vs. taxonomy-informed explanation pairs
└── scenarios/
    └── scenario-on-screen.pdf                   ← PDF of on screen display for scenarios
    └── scenario-descriptions.pdf       ← PDF of on screen display for scenarios

```

## Artifact Descriptions

### Codebook (`codebook/`)
- **`ethex_codebook.csv`** — The complete ETHEX codebook. Each row is one of 69 codes. 

### Requirement Patterns (`patterns/`)

- **`requirement_patterns.md`** — All 16 explainability requirement patterns derived by crossing 4 stakeholder roles (Autonomous Systems Expert, Ethics Specialist, Operational Practitioner, Layperson) with 4 ethical scenario clusters (Triage, Epistemic, Values, Boundary). Each pattern includes a descriptive name, context, priority categories, parameterized requirement template, and a grounded example traced to a coded participant utterance. Includes the pattern index (Table VII from the paper) and usage instructions.

### Survey Materials (`survey/`)

- **`explanations.md`** — All 20 explanation pairs (10 scenarios × 2 decisions) in readable Markdown. Documents the generation methodology, counterbalancing approach, and presents each baseline/taxonomy-informed pair side by side.
