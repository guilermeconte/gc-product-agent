# Copy Skill

## Objetivo

Criar, organizar, editar e versionar conteúdo textual do produto.

## Responsabilidades

- mapear conteúdo por página e seção;
- gerar copy provisória quando necessário;
- preservar voz e posicionamento;
- editar textos fornecidos;
- criar CTA, headings, labels, mensagens de erro e microcopy;
- registrar conteúdo como draft/approved.

## Modelo

```yaml
copy:
  page:
    section:
      field:
        text:
        purpose:
        status: draft|review|approved
```

## Regra

Texto ausente não bloqueia Design ou Figma. Usar placeholder semanticamente adequado e marcar como `draft`.

## Saída

`.project/copy/content.md`
`.project/copy/sitemap.md`
