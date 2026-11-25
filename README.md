# analytics-stack

An end-to-end analytics stack built on the theLook e-commerce dataset:
ingestion (dlt) → warehouse (DuckDB / BigQuery) → modelling (dbt) → analysis and BI.
The repo holds everything needed to rebuild the system, but no data and no secrets.

## Setup

```bash
git clone <repo-url> && cd analytics-stack
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Put your Google Cloud service-account key outside the repo (or name it `*-key.json`,
which is git-ignored) and point to it from `ingestion/.dlt/secrets.toml`.
dbt's `profiles.yml` lives in `~/.dbt/`, not in this repo.

## Architecture

_Diagram placeholder: add image to `docs/`._

## Phases

_One section per phase will be added as the project progresses._
