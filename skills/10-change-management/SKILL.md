# Change Management Skill

## Objetivo

Permitir alterações durante qualquer fase sem perder contexto.

## Processo

```text
User change
→ classify
→ identify affected artifacts
→ calculate impact
→ create Change Request
→ approve/apply
→ invalidate dependents
→ continue from earliest affected node
```

## Categorias

- content
- design
- component
- motion
- architecture
- backend
- infrastructure
- security

## Exemplo

Alterar CTA:
- Copy: affected
- Figma: affected
- Build: affected
- QA: affected
- Discovery: unaffected

Alterar arquitetura:
- Translation: affected
- Build: affected
- QA: affected
- Design: normalmente preservado

## Versionamento

Nunca apagar silenciosamente uma versão aprovada. Registrar:

```yaml
change:
  id:
  reason:
  requested_by:
  affected_steps: []
  invalidated_artifacts: []
  approved:
  status:
```
