# AI Product Workflow

Framework de agentes para conduzir projetos de produto digital do briefing à implementação, mantendo estado persistente, integração com Figma via MCP, pesquisa técnica, Design System, copy, tradução design→código, build e QA.

## Princípios

1. Figma é fonte de verdade visual quando definido como fonte oficial.
2. O Design Contract é a interface entre Design Engine e Build Engine.
3. O workflow é orientado a estado, não linear.
4. Toda mudança deve gerar impacto e invalidar apenas os artefatos dependentes.
5. Etapas opcionais podem ser puladas sem bloquear o projeto.
6. O agente nunca deve inventar dados do usuário ou do Figma; registra pendências.
7. O usuário pode iniciar, pausar, continuar, revisar, aprovar, voltar e alterar qualquer etapa.
8. A tecnologia de implementação é variável; o Design Engine permanece agnóstico.
9. O Figma MCP é uma ferramenta do Design/Figma Agent, não a definição da arquitetura inteira.
10. O projeto só é concluído após os gates de qualidade.

## Fluxo

Discovery → Research (opcional) → Copy → Design System → Figma → Translation → Build → QA → Delivery

Research pode ser skipped. Copy pode começar como draft. Qualquer etapa pode ser reaberta por Change Request.

## Estrutura

```text
skills/
├── 00-orchestrator/
├── 01-discovery/
├── 02-research/
├── 03-copy/
├── 04-design-system/
├── 05-figma/
├── 06-motion/
├── 07-translation/
├── 08-build/
├── 09-qa/
├── 10-change-management/
└── 11-delivery/
```

## Estado mínimo

```yaml
project:
  id:
  name:
  status:

workflow:
  current_step:
  steps: []

stack:
  framework:
  language:
  styling:
  backend:
  database:

sources:
  figma:
  research: []

facts: {}
decisions: {}
preferences: {}
assumptions: {}
pending: {}
artifacts: {}
changes: []
```

## Comandos

```text
/start
/status
/pause
/resume
/continue
/review
/approve
/reject
/skip <step>
/start <step>
/pause <step>
/retry <step>
/rollback <step>
/change
/impact
/apply
/revert
/sync figma
/audit figma
/run qa
```
