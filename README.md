# AgentCon SDD — Petstore Demo

Minimal setup to build a Petstore app using Spec‑Driven Development (Spec Kit). Source spec: https://petstore3.swagger.io/ (OpenAPI JSON: https://petstore3.swagger.io/api/v3/openapi.json)

## Prereqs
- macOS/Linux/Windows
- Git
- Python 3.11+
- uv
- An AI coding agent of your choice (e.g., Copilot, Claude, Gemini)

## Setup (once)
```
uv tool install specify-cli --from git+https://github.com/github/spec-kit.git
```

## Initialize (in this folder)
```
specify init --here --ai <your-agent>
```

## Run the SDD flow (in your agent chat)
```
/speckit.constitution
/speckit.specify
/speckit.plan
/speckit.tasks
/speckit.implement
```

## If time permits
- Verify tools: `specify check`
- Refine spec: `/speckit.clarify`
- Validate plan: `/speckit.analyze`

## References
- Spec Kit repo: https://github.com/github/spec-kit/tree/main
- Installation guide: https://github.github.io/spec-kit/installation.html
- Quick start: https://github.github.io/spec-kit/quickstart.html
