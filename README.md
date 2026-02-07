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
/speckit.constitution Strict OpenAPI 3.0 spec adherence (https://petstore3.swagger.io/api/v3/openapi.json). All endpoints, schemas, and responses must match the spec exactly. Test-first development. Direct framework usage, no unnecessary abstractions.
```

```
/speckit.specify Build a pet store API where users can browse available pets by category, add pets to a shopping cart, and place orders. Admin users can manage pet inventory and status.
```

```
/speckit.plan Node.js with Express, PostgreSQL for persistence, Jest for testing. Minimal middleware, direct OpenAPI spec adherence.
```

```
/speckit.tasks
```

```
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
