# GC Creator v0.3.1

Plugin Claude para criação de produtos digitais.

## Estrutura nativa

- `.claude-plugin/plugin.json` — manifesto
- `skills/` — 12 habilidades
- `skills/*/references/` — conteúdo e recursos carregados pelas habilidades
- `.mcp.json` — configuração opcional de MCP do usuário

O antigo diretório `content/` foi removido porque não é um componente nativo de plugin do Claude.

## MCP do usuário

O template usa:

- `GC_CREATOR_MCP_URL`
- `GC_CREATOR_MCP_TOKEN`

Não coloque credenciais reais no Git.

O GC Creator não presume um servidor Figma específico. Quando um MCP estiver conectado, a skill correspondente deve descobrir as ferramentas disponíveis antes de executar qualquer operação.


## Compatibilidade Claude
Cada `SKILL.md` inicia com YAML frontmatter obrigatório (`name` e `description`) para ser reconhecido pelo Claude.


## Primary entry point

The primary user-facing skill is **The Architect** (`skills/00-the-architect`). Users should normally start with `/create`, `/start`, `/continue`, or `/infinity-ideas`. The Architect activates the specialist skills as required instead of requiring the user to invoke each skill manually.
