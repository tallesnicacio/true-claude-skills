# Design System — True Source E-commerce

Extraido do Figma (fileKey: HpVcAiIeNKc0J6EN5PPAVP) em 2026-03-19.
Usar como referencia para TODOS os frontends da True Source.

## Cores (Design Tokens)

### Primarias
- `--marrom: #481216` — texto principal, titulos, icones
- `--laranja: #FB6E13` — CTA primario, destaques, menu ativo
- `--laranja-light: #F5EFEB` — backgrounds leves, tags inativas, search bar
- `--branco: #FFFFFF` — fundo principal

### Secundarias
- `--verde: #2F854D` — botao comprar, assinatura, badges desconto
- `--verde-escuro: #44682E` — links de assinatura
- `--dark: #3C3C3B` — texto secundario (footer, body)
- `--grey: #8E8E8D` — texto muted, placeholders

### Borders
- `--stroke-marrom: rgba(72, 18, 22, 0.2)` — bordas suaves
- `--stroke-light: #E2E2E2` — bordas claras (inputs)

## Tipografia

### Fontes (ordem de prioridade)
1. **ABC Solar** — titulos, headings, labels de secao
2. **Figtree** — corpo de texto, menus, tags, CTAs
3. **Inter** — textos pequenos, breadcrumbs, disclaimers

### Escala Tipografica
| Token | Familia | Peso | Tamanho | Letter-spacing | Uso |
|-------|---------|------|---------|----------------|-----|
| H1 | ABC Solar | Bold 700 | 24px | -1% | Titulos de produto, precos |
| H2 | ABC Solar | Bold 700 | 20px | -1% | Subtitulos de secao |
| Menu | Figtree | Bold 700 | 14px | -1% | Itens de menu, labels |
| Menu-2 | ABC Solar | Regular 400 | 14px | -1% | Labels de secao (SABOR, TAMANHO) |
| Text-Bold | Figtree | Bold 700 | 14px | 0 | Texto bold em tags, CTAs inline |
| Text-Body | Figtree | Regular 400 | 14px | 0 | Texto corpo |
| Text-Mini | Figtree | Regular 400 | 12px | 0 | Texto pequeno |
| Text-Mini-Bold | Inter | Bold 700 | 12px | 0 | Badges de pagamento |
| CTA-Label | ABC Solar | Bold 700 | 14-18px | -1% | Texto de botoes CTA |

## Border Radius
- `--radius-sm: 6px` — inputs, cards de compra, radio options
- `--radius-md: 20px` — cards de produto, containers de imagem
- `--radius-lg: 35px` — secoes (top corners — PDP, Rodape)
- `--radius-pill: 200px` — tags inativas, badges, pills
- `--radius-full: 300px` — botoes CTA, search bar, tags ativas

## Espacamento
- `--space-page: 40px` — padding horizontal da pagina
- `--space-section: 40px` — gap entre secoes grandes
- `--space-block: 32px` — gap entre blocos
- `--space-group: 24px` — gap entre grupos de elementos
- `--space-element: 16px` — gap entre elementos relacionados
- `--space-tag: 8px` — gap entre tags
- `--space-tag-padding: 12px` — padding interno de tags
- `--space-cta-h: 24px` — padding horizontal CTA
- `--space-cta-v: 18px` — padding vertical CTA
- `--space-card: 24px` — padding interno de cards

## Componentes

### Header
- Border-top: 4px solid var(--laranja)
- Logo (140x49px) + Search bar (bg laranja-light, radius-full) + Icons (user, help, cart)
- Menu: items Figtree Bold 14px, separador bullet, item ativo em laranja, "Assinatura" em cor laranja

### Tag
- **Ativa:** bg laranja, texto marrom, icone check-circle, radius-full (300px)
- **Inativa:** bg laranja-light, texto marrom, radius-pill (200px)
- Padding: 12px, font: Figtree Bold 14px

### CTA Button
- **Primario (Laranja):** bg laranja, texto branco, radius-full, font ABC Solar Bold
- **Comprar (Verde):** bg verde, texto branco, radius-sm (6px), font ABC Solar Bold, icone cart
- **Produto-especifico:** bg cor do produto (ex: #F5C00F amarelo), texto marrom, radius-full

### Radio Option (Assinatura)
- **Selecionado:** border 1.5px verde, bg branco
- **Nao selecionado:** border 1px stroke-marrom
- Badge desconto: bg verde, texto branco, radius-pill, font Figtree Bold 14px

### Quantity Selector
- Container: bg branco, radius-sm
- Botoes "-" / "+" : font 18px
- Numero: font Figtree Bold 14px

### Card de Compra
- bg laranja-light, radius-md (20px), padding 24px
- Preco: ABC Solar Bold 24px
- Preco riscado + parcelamento: Figtree Regular 14px
- Assinatura: texto verde

### Footer
- bg branco, radius-lg top corners (35px)
- Newsletter: input com CTA laranja embutido
- Menu 4 colunas: titulos ABC Solar Bold, items Inter Regular
- Links destaque: ABC Solar Bold em cor laranja
- Selos pagamento: Visa, Mastercard, Diners, Boleto, Pix
- Redes sociais: icones em circulos com border laranja

### BreadCrumb
- Home icon (16px) + "/" separador + links uppercase
- Font: Figtree/Inter Regular 12px
- Cor: marrom (ativo), grey (inativo)

## Iconografia
- Biblioteca: Untitled UI
- Tamanhos padrao: 16px (inline), 24px (normal), 28px (header)
- Icones principais: user-circle, shopping-cart-01, check-circle, home-05, chevron-down, search, arrow-narrow-right, message-question-square, star-01, instagram, youtube

## Layout
- Max-width: 1440px
- Pagina padding: 40px horizontal
- Secoes com rounded top corners (35px) criando efeito de sobreposicao
- Produto: layout 2 colunas (foto sticky left + info right)

## Regras Gerais
1. Textos uppercase em: titulos de produto, labels de secao, menu footer, CTAs
2. Cores de produto podem variar (amarelo magnesio, etc) mas seguir mesmo padrao de contraste com marrom
3. Sempre usar var() para referenciar tokens de cor
4. Manter hierarquia visual: ABC Solar para titulos, Figtree para corpo, Inter para micro-texto
