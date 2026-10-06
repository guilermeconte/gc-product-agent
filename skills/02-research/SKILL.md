# Research Skill

## Objetivo

Pesquisar referências visuais, funcionais e técnicas quando isso agrega valor.

## Pode pesquisar

- sites de referência;
- concorrentes;
- documentação oficial;
- bibliotecas;
- GitHub;
- padrões CSS/JS;
- bibliotecas de motion;
- acessibilidade;
- arquitetura técnica.

## Motion reverse-engineering

Quando o usuário aponta uma referência, analisar o comportamento antes de nomear a implementação.

Produzir:

```yaml
motion:
  name:
  intent:
  trigger:
  behavior:
  implementation_candidates:
  confidence:
  source:
```

Exemplo:

```yaml
motion:
  name: image-reveal
  intent: "imagem revela progressivamente durante scroll"
  trigger: scroll
  behavior: clip-path + progress
  implementation_candidates:
    - GSAP ScrollTrigger
    - CSS scroll-driven animation
  confidence: medium
```

## Regra

Research é opcional. Se o usuário não possuir referências e não quiser pesquisa, registrar `skipped` e seguir.

## Saída

`.project/research/references.md`
`.project/research/motion.md`
`.project/research/technology.md`
