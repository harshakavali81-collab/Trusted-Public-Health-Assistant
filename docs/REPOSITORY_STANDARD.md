# Repository standard

## Layout

This repository keeps its working source paths. A shared portfolio structure does not require moving a React application, Python package, BI workbook or Verilog project into identical runtime directories.

| Area | Convention |
| --- | --- |
| Landing page | `README.md`: purpose, visuals, demo, features, stack, architecture, setup, tradeoffs and roadmap |
| Detailed reference | `PROJECT_GUIDE.md`: retained project-specific explanation and historical release notes |
| Documentation | `docs/`: design, inventory, reproduction and evidence |
| Work intake | `.github/ISSUE_TEMPLATE/`: bug and feature forms |
| Review | `.github/PULL_REQUEST_TEMPLATE.md`: linked issue, behavior and validation |
| Automation | `.github/workflows/portfolio-docs.yml`: README section and local-link checks |
| Source and tests | Existing project-specific paths listed below; no empty source/test placeholders |

## Workflow

1. Open an issue describing the user problem and measurable acceptance criteria.
2. Add it to a GitHub Project with Todo, In progress, Review and Done states when a board is configured.
3. Use a focused branch and meaningful commits, such as `docs: correct local setup paths` or `fix(api): reject malformed input`.
4. Run the project's documented checks and `python scripts/check_portfolio_docs.py`.
5. Open a pull request with actual validation results and `Closes #<issue-number>`.
6. Merge after review; record release evidence and update the issue/board.

Board creation, profile pins, repository social previews and milestone settings require account-level configuration. This file does not claim those settings have been applied.

## Validation scope

The documentation check validates the landing-page headings and local link targets only. It does not execute models, certify test coverage, inspect Git history for secrets, verify external websites, or prove production readiness. Existing application workflows remain the source of runtime CI evidence.

Keep credentials in local environment variables. A gitignore rule does not remove secrets already tracked or committed. Use only permitted sample data in public demos.

## Inventory at standardization

The following are the pre-existing public project files. New standardization files are described above. Historical guides may mention external bundles that are not part of this list.

- [`Dockerfile`](<../Dockerfile>)
- [`PROJECT.json`](<../PROJECT.json>)
- [`README.md`](<../README.md>)
- [`app`](<../app>)
- [`app/__init__.py`](<../app/__init__.py>)
- [`app/catalog.py`](<../app/catalog.py>)
- [`app/classification.py`](<../app/classification.py>)
- [`app/engine.py`](<../app/engine.py>)
- [`app/forecasting.py`](<../app/forecasting.py>)
- [`app/main.py`](<../app/main.py>)
- [`app/records.py`](<../app/records.py>)
- [`app/retrieval.py`](<../app/retrieval.py>)
- [`app/source_registry.py`](<../app/source_registry.py>)
- [`app/sources.py`](<../app/sources.py>)
- [`app/spatial.py`](<../app/spatial.py>)
- [`app/storage.py`](<../app/storage.py>)
- [`assets`](<../assets>)
- [`assets/architecture.svg`](<../assets/architecture.svg>)
- [`assets/cover.svg`](<../assets/cover.svg>)
- [`assets/synthetic-trend.svg`](<../assets/synthetic-trend.svg>)
- [`cli.py`](<../cli.py>)
- [`docker-compose.yml`](<../docker-compose.yml>)
- [`docs`](<../docs>)
- [`docs/ACCEPTANCE.md`](<../docs/ACCEPTANCE.md>)
- [`docs/ARCHITECTURE.md`](<../docs/ARCHITECTURE.md>)
- [`docs/BASELINE_COMPARISON.md`](<../docs/BASELINE_COMPARISON.md>)
- [`docs/DATA_STORAGE.md`](<../docs/DATA_STORAGE.md>)
- [`docs/EVALUATION.md`](<../docs/EVALUATION.md>)
- [`docs/MODEL_CARD.md`](<../docs/MODEL_CARD.md>)
- [`docs/PROJECT_STRUCTURE.md`](<../docs/PROJECT_STRUCTURE.md>)
- [`docs/SECURITY.md`](<../docs/SECURITY.md>)
- [`docs/THREAT_MODEL.md`](<../docs/THREAT_MODEL.md>)
- [`docs/workflow.mmd`](<../docs/workflow.mmd>)
- [`frontend`](<../frontend>)
- [`frontend/index.html`](<../frontend/index.html>)
- [`pytest.ini`](<../pytest.ini>)
- [`requirements.txt`](<../requirements.txt>)
- [`sample_request.json`](<../sample_request.json>)
- [`tests`](<../tests>)
- [`tests/test_demo.py`](<../tests/test_demo.py>)
