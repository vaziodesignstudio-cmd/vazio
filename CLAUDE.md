# Contexto Vazio (para agentes)

Este repositório é a base operacional do estúdio **Vazio** (web design). É independente da operação AstroPay; nunca misturar contextos.

## Antes de qualquer tarefa, leia

1. [STUDIO.md](STUDIO.md) — filosofia, princípios e padrão de qualidade do estúdio. Vale para todo projeto.
2. O brief do projeto ativo em `briefs/{slug}.md` — define a ID visual e o escopo daquele cliente.

## Regra de ouro sobre ID visual

Cada projeto tem **ID visual própria**. Os arquivos em `case-studies/` são **referência de qualidade**, não de visual. Nunca copiar paleta, tipografia ou layout de um case anterior para um projeto novo, exceto quando explicitamente pedido.

Padrões **estruturais** (em `patterns/`) podem e devem ser reutilizados; padrões **visuais** não.

## Idioma

- Conversa com o usuário: PT-BR.
- Código, commits, nomes de arquivo, variáveis: EN.
- Conteúdo dos sites: o que o brief do cliente definir.

## Agentes disponíveis

Ver [.claude/agents/](.claude/agents/). Núcleo inicial cobre descoberta (UX research), arquitetura de informação, UI, brand guardian por projeto, storytelling, geração de imagem, prototipagem, frontend, CMS e operação de estúdio.
