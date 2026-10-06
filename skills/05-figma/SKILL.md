# Figma Skill

## Objetivo

Operar o Figma como ferramenta de Design Engine por meio do servidor MCP disponível no ambiente.

## Princípio

O agente deve preferir operações estruturadas no Figma: variables, styles, components, variants, frames, pages e prototype, em vez de apenas desenhar elementos soltos.

## Capacidades esperadas do MCP

- leitura de arquivo/páginas;
- inspeção de nodes;
- leitura de variables/styles;
- leitura de components/variants;
- leitura de prototypes;
- criação/edição de elementos quando suportado;
- sincronização de metadados;
- inspeção para Design QA.

O agente deve consultar as ferramentas MCP disponíveis antes de assumir que uma operação de escrita existe.

## Estrutura sugerida do arquivo

```text
01 · Brand
02 · Foundations
03 · Components
04 · Patterns
05 · Pages
06 · Prototypes
07 · Documentation
```

## Regras

- Figma é fonte de verdade visual quando declarado pelo projeto.
- Não sobrescrever trabalho existente sem checkpoint.
- Antes de alterações em massa, criar/registrar checkpoint.
- Manter nomes alinhados ao Naming Engine.
- Aplicar variables/styles em vez de valores isolados quando possível.
- Manter Desktop/Mobile e estados documentados.
- Registrar o que o MCP não consegue reproduzir.

## Comandos

```text
/sync figma
/audit figma
/start figma
/pause figma
/review figma
```

## Saída

`.project/figma/map.json`
`.project/figma/sync.json`
