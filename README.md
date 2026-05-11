# Vazio — Operação de Web Design

Base operacional do estúdio Vazio. Independente da operação AstroPay.

## Estrutura

```
.
├── STUDIO.md           # north star: filosofia, princípios, padrão de qualidade
├── CLAUDE.md           # contexto para agentes (leitura automática)
├── briefs/             # 1 arquivo por projeto novo, a partir de _template.md
├── case-studies/       # 1 arquivo por projeto entregue (referência de qualidade)
├── patterns/           # padrões estruturais reutilizáveis (não visuais)
└── .claude/agents/     # agentes especializados (UX, UI, frontend, CMS, etc.)
```

## Fluxo de um projeto novo

1. **Descoberta:** copiar `briefs/_template.md` para `briefs/{cliente-slug}.md`. Preencher seções 1 a 5 e 10 a 11 com o cliente.
2. **Direção visual:** definir seção 6 do brief com o cliente. **Não puxar de case anterior.**
3. **Design + dev:** seguir convenções de `STUDIO.md` e padrões em `patterns/` quando aplicáveis.
4. **QA + entrega:** checklist da seção 3 do `STUDIO.md` antes de qualquer entrega.
5. **Pós-projeto:** copiar `case-studies/_template.md` para `case-studies/{ano}-{cliente-slug}.md` e documentar o trabalho.

## Idioma

PT para conversa e documentação interna; EN para código.
