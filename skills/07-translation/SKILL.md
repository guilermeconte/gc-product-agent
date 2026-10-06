---
name: 07-translation
description: Translate design contracts and product decisions into framework-agnostic implementation contracts and code mappings.
---

# Translation Skill

## Objetivo

Converter o Design Contract em um Code Contract sem amarrar o Design Engine a uma stack.

## Mapeamentos

- token → variável da stack;
- component → componente/partial;
- page → route;
- motion → implementation;
- state → UI state;
- responsive rule → media/container rule;
- accessibility requirement → semantic/ARIA behavior.

## Naming

```text
Figma: Project Card
React: ProjectCard
Vue: ProjectCard.vue
Blade: project-card.blade.php
CSS: .project-card
Data: [data-component="project-card"]
```

## Saída

`.project/build/code-contract.json`
