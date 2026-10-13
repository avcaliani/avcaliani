<div align="center">

# Repo Conventions

![gif](https://media.giphy.com/media/9itja4ux9fpFTSu7le/giphy.gif)

How I organize my GitHub: which kinds of repos exist, how they evolve, and how they are tagged.

</div>

## Categories

```yaml
scratchpad:
  type: mono-repo
  description: Quick experiments for technologies with no lab.
  folders: [data, front-end, misc]  # created on demand
  question: What happens if I try this?

lab:
  type: single repo
  name: lab-<tech>
  description: Learning repo for one technology.
  question: How does this behave?

archive:
  type: mono-repo (private)
  description: Frozen projects kept for history only.
  question: What did this look like at the time?
```

Standalone projects keep their own names (e.g. `kafka-in-docker`, `mr-owlf`) and have no intent.

## Graduation Rule

```mermaid
---
config:
  look: handDrawn
---
flowchart LR
    S["📝 scratchpad"] -->|"Lab exists"| L["🔬 lab"]
    L -->|"Outdated, still useful"| A["📦 archived lab"]
    A -->|"Not needed anymore"| R["🗄️ archive"]
```

- **archived lab**: GitHub-archived, public, kept for consulting.
- **archive**: private, historical only.

### Lab Layout

```text
lab-<tech>/
├── snippets/   quick experiments
└── pocs/       end-to-end software
```

## Tags

Use only tags that describe what the repo actually contains: one or two Identity, plus the Technology and Concept tags it demonstrates.

```bash
# identity
data-engineering distributed-systems backend learning

# technology
airflow dbt spark flink kafka redpanda duckdb iceberg delta-lake parquet avro terraform docker kubernetes

# concept
batch-processing stream-processing event-driven data-modeling schema-evolution query-optimization
cost-optimization exactly-once backpressure observability governance
```
