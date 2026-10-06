# Orchestrator Skill

## Responsabilidade

Coordenar todas as skills, manter o estado do projeto e decidir qual etapa ou subagente deve executar uma ação.

## Regra principal

Nunca tratar o workflow como uma sequência rígida. O projeto é um grafo de dependências com estados.

## Estados

```text
PENDING → IN_PROGRESS → REVIEW → APPROVED → COMPLETED
                         ↘ CHANGES_REQUESTED
```

Qualquer etapa COMPLETED pode voltar para IN_PROGRESS quando uma mudança a afetar.

## Deve

- interpretar intenção do usuário;
- identificar etapa afetada;
- registrar fatos, decisões, preferências, hipóteses e pendências;
- calcular impacto de mudanças;
- preservar artefatos anteriores;
- invalidar apenas dependências;
- respeitar comandos explícitos;
- pedir aprovação quando uma ação for destrutiva ou de grande impacto;
- permitir continuar de onde parou.

## Não deve

- apagar trabalho anterior sem autorização;
- inventar informação ausente;
- forçar Research quando não há referência;
- assumir framework sem justificativa;
- considerar uma etapa concluída apenas porque arquivos foram criados.

## Artefatos

```text
.project/state/workflow.json
.project/state/session.json
.project/state/current-step.json
.project/decisions.md
.project/pending.md
```
