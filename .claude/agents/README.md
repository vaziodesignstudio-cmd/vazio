# Agentes Vazio — Núcleo

Núcleo inicial de 10 agentes especializados, clonados de [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents).

## Quando chamar cada um

### Descoberta
- **UX Researcher** (`design-ux-researcher`) — entrevistas com cliente e usuário, análise, requisitos. Use no início de todo projeto.
- **UX Architect** (`design-ux-architect`) — IA, fluxos, sitemap, wireframes de baixa fidelidade.

### Design
- **UI Designer** (`design-ui-designer`) — UI de alta fidelidade, componentes, layout final.
- **Brand Guardian** (`design-brand-guardian`) — guarda a ID visual **daquele cliente** durante o projeto. Reativar a cada novo brief.
- **Visual Storyteller** (`design-visual-storyteller`) — narrativa e copy estrutural de landing pages.
- **Image Prompt Engineer** (`design-image-prompt-engineer`) — prompts para imagens hero geradas por IA.

### Engenharia
- **Rapid Prototyper** (`engineering-rapid-prototyper`) — provas de conceito e protótipos rápidos.
- **Frontend Developer** (`engineering-frontend-developer`) — implementação final, performance, a11y.
- **CMS Developer** (`engineering-cms-developer`) — Webflow, Sanity, Payload, modelagem de conteúdo.

### Operação
- **Studio Producer** (`project-management-studio-producer`) — operação do estúdio, propostas, cronograma, comunicação com cliente.

## Como adicionar mais

Quando precisar, baixar do mesmo repo:

```bash
curl -sSL "https://raw.githubusercontent.com/msitarzewski/agency-agents/main/<categoria>/<arquivo>.md" \
  -o .claude/agents/<arquivo>.md
```

Complementares sugeridos para depois (em ordem de prioridade):
1. `engineering-code-reviewer` — gate de qualidade antes de merge
2. `marketing-seo-specialist` — SEO básico em toda entrega
3. `sales-proposal-strategist` — propostas comerciais
4. `engineering-devops-automator` — automação de deploy
5. `design-whimsy-injector` — microinterações
