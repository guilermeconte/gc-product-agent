# Motion Skill

## Objetivo

Traduzir intenção de interação em especificação visual e implementação técnica.

## Classificação

### CSS-first
- hover
- focus
- active
- color transition
- transform simples
- opacity simples

### JS/motion engine
- entrance sequencing
- scroll-linked animation
- mouse interaction
- complex timeline
- stagger
- smooth scrolling
- cross-element synchronization

## Motion Contract

```yaml
motion:
  id:
  figma_name:
  code_name:
  data_attribute:
  intent:
  trigger:
  properties:
  duration:
  easing:
  scroll:
  mouse:
  reduced_motion:
  implementation:
  dependencies:
```

## Regra

O designer descreve comportamento. O agente pesquisa/decide a implementação. O designer não precisa conhecer o nome da API.

## Exemplo

```text
"imagem cresce e revela conforme o scroll"
→ scroll-linked image reveal
→ implementação candidata
→ Figma prototype
→ data-motion="image-reveal"
→ implementação no framework
```

## Saída

`.project/design/motion.json`
