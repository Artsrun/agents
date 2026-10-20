This project's Baseline target is Baseline 2024.

Repo is a registry, not a runtime.

- One agent = `agents/<id>/agent.json` + README.
- Pages catalog = `docs/registry.json`. Keep the row in sync with `agent.json`.
- `kamoji` is the face. `label` is the short name. `work` is one line of what it does.
- Do not put secrets in agent.json.
- Pages script writes with textContent only.
