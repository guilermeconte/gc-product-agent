# GC Creator — Architecture

O sistema separa três camadas:

1. **Content** — conhecimento estável, contratos, schemas, princípios e documentação.
2. **Skills** — procedimentos especializados executados pelo Claude.
3. **Connectors/MCP** — ferramentas e dados externos.

O plugin não deve assumir que uma integração existe. Primeiro deve inspecionar as ferramentas disponíveis e só então executar ações.

### Estado do projeto

`.project/` é a fonte de verdade do projeto em execução.

```text
.project/
├── manifest.yaml
├── state/
│   ├── workflow.json
│   ├── current-step.json
│   └── session.json
├── discovery/
├── research/
├── copy/
├── design/
├── figma/
├── build/
└── qa/
```
