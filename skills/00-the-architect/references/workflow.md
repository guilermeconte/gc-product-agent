# GC Creator — Workflow

## Grafo principal

DISCOVERY → RESEARCH → COPY → DESIGN SYSTEM → FIGMA → MOTION → BUILD → QA → DELIVERY

Nem toda execução precisa passar por todas as etapas. O Orchestrator decide dependências e pode marcar uma etapa como `skipped`.

## Estados

`pending`, `ready`, `running`, `blocked`, `skipped`, `draft`, `review`, `approved`, `rejected`, `invalidated`, `done`.

## Comandos

`/start`, `/status`, `/pause`, `/resume`, `/continue`, `/review`, `/approve`, `/reject`, `/skip <step>`, `/start <step>`, `/retry <step>`, `/rollback <step>`, `/change`, `/impact`, `/apply`, `/revert`, `/sync figma`, `/audit figma`, `/run qa`.

Linguagem natural deve ser interpretada como intenção equivalente quando possível.
