# Design System Skill

## Objetivo

Criar ou auditar um Design System estruturado, reutilizável e conectado ao código.

## Ordem

1. Brand
2. Foundations
3. Tokens
4. Typography
5. Layout/Grid
6. Spacing
7. Radius
8. Motion tokens
9. States
10. Primitives
11. Components
12. Patterns
13. Templates/Sections
14. Pages
15. Responsive rules
16. Accessibility

## Foundations mínimas

### Color
- brand
- neutral
- semantic: success, warning, error, info
- surface
- text
- border
- focus
- overlay
- category/context colors quando aplicável

### Typography
- font family
- display
- headings
- body
- labels
- caption
- code
- weights
- line heights
- letter spacing

### Spacing
- escala de spacing
- page padding
- section spacing
- component gap
- grid gap
- control inset

### Layout
- page max width
- container
- grid
- columns
- gutters
- breakpoints
- section widths

### Shape
- radius
- border widths
- icon sizes

### Motion
- durations
- easings
- delays
- stagger
- reduced-motion behavior

## Primitives mínimas

- Container
- Stack
- Inline
- Grid
- Divider
- Spacer
- Icon
- Image
- Link
- Text
- Heading
- Label
- Eyebrow
- Badge
- Index/metadata label

## Componentes básicos de site

### Navigation
- Header
- Logo
- Nav
- NavItem
- NavButton
- MobileMenuButton
- MenuOverlay
- Breadcrumb

### Actions
- Button
- ButtonLink
- IconButton
- Link
- ExternalLink

### Forms
- Field
- Label
- Input
- Textarea
- Select
- Checkbox
- Radio
- Switch
- FormMessage
- ErrorMessage
- SubmitButton

### Content
- Card
- MediaCard
- ProjectCard
- ArticleCard
- Stat
- StatCard
- Quote
- List
- Accordion
- Tabs

### Feedback
- Alert
- Toast
- Loading
- Skeleton
- EmptyState

### Layout/site
- Section
- Hero
- Footer
- CTA
- SocialLinks
- ContactBlock

### Responsive
Cada componente deve declarar comportamento em:
- desktop;
- tablet quando aplicável;
- mobile.

## Naming

O Design System deve produzir uma tabela de correspondência:

| Figma | Código | CSS | Data |
|---|---|---|---|
| Project Card | ProjectCard | .project-card | project-card |
| Menu Overlay | MenuOverlay | .menu-overlay | menu-overlay |

O nome deve respeitar a linguagem e convenções da stack escolhida.

## Regra

Não criar componentes só porque são comuns. Criar os que fazem sentido para o produto, partindo da biblioteca base acima.

## Saída

`.project/design/tokens.json`
`.project/design/components.json`
`.project/design/pages.json`
`.project/design/naming.json`
