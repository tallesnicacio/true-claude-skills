# TRUE — Claude Code Skills

Skills e practices para o Claude Code usados pela equipe TRUE.

## Conteudo

### Skills

- **sales-enablement** — Criacao de apresentacoes, pitch decks, one-pagers, objection handling, demo scripts e playbooks de vendas
- **true-brand-guide** — Guia de marca v6.0 da TRUE para qualquer material visual (landing pages, banners, social media, emails, interfaces)

### Practices

- **true-source-design-system.md** — Design tokens do e-commerce (cores, tipografia, espacamento, componentes)
- **design-system-foundation.md** — Setup de design system com shadcn/ui a partir de screenshots
- **design-system-new-page.md** — Workflow para construir paginas a partir de designs/screenshots

## Instalacao

### Skills

Copie as pastas de skills para `~/.claude/skills/`:

```bash
# Clonar o repositorio
git clone git@github.com:tallesnicacio/true-claude-skills.git

# Copiar skills
cp -r true-claude-skills/skills/sales-enablement ~/.claude/skills/
cp -r true-claude-skills/skills/true-brand-guide ~/.claude/skills/
```

### Practices

Copie os arquivos de practices para `~/.claude/practices/`:

```bash
cp true-claude-skills/practices/*.md ~/.claude/practices/
```

### Verificacao

Abra o Claude Code e teste:
- `/sales-enablement` para criar um pitch deck
- Mencione "TRUE" ou "peca para a True" para ativar o brand guide

## Estrutura

```
skills/
  sales-enablement/
    SKILL.md              # Skill principal
    evals/evals.json      # Testes de validacao
    references/
      deck-frameworks.md      # Frameworks slide-by-slide
      one-pager-templates.md  # Templates de one-pagers
      objection-library.md    # Biblioteca de objecoes
      demo-scripts.md         # Scripts de demo
  true-brand-guide/
    SKILL.md              # Guia de marca completo v6.0
practices/
  true-source-design-system.md   # Design tokens do e-commerce
  design-system-foundation.md    # Setup shadcn/ui
  design-system-new-page.md      # Workflow de paginas
```
