# Vazio Studio — Operação

> Este documento é o "norte" do estúdio. Descreve o que torna um trabalho reconhecidamente Vazio, independente da ID visual de cada cliente. Cada projeto novo herda este contexto; a ID visual entra por cima.

---

## 1. Filosofia

> _A preencher por Lucas. 3 a 5 frases que respondem: por que a Vazio existe, o que ela acredita sobre web design, e o que ela recusa fazer._

**Rascunho inicial (substituir):**
- A Vazio acredita que um site bem feito é mais barato a longo prazo do que um site barato.
- Tipografia, ritmo e silêncio são tão importantes quanto cor e imagem.
- Performance e acessibilidade não são extras, são parte do design.
- Cada cliente tem uma ID visual única; o que se repete em todo trabalho Vazio é o cuidado, não o estilo.

## 2. Princípios de design (transversais)

Esses princípios se aplicam a todo projeto, mesmo que a ID visual mude:

1. **Editorial antes de decorativo.** Hierarquia tipográfica resolve a maior parte das decisões de layout.
2. **Silêncio é conteúdo.** Espaço em branco generoso, mas com intenção (não preguiça).
3. **Movimento serve à leitura.** Microinterações respondem a uma pergunta do usuário; nunca são enfeite.
4. **Acessibilidade é piso, não teto.** WCAG 2.2 AA mínimo, AAA quando o conteúdo permitir.
5. **Performance é parte do briefing.** LCP < 2.5s no 4G, CLS < 0.1, INP < 200ms.
6. **Responsividade não é só breakpoints.** Conteúdo se reorganiza, não apenas escala.

## 3. Padrão de qualidade (checklist de entrega)

Antes de qualquer entrega ir ao cliente:

- [ ] Lighthouse mobile ≥ 90 em Performance, Acessibilidade, Best Practices, SEO
- [ ] Teste em iPhone real (Safari) e Android real (Chrome)
- [ ] Teclado + leitor de tela: navegação principal funciona
- [ ] Contraste verificado em todas as combinações de cor/fundo
- [ ] Conteúdo: revisão ortográfica e gramatical feita
- [ ] OG image + favicon + meta description
- [ ] 404 e estados de erro tratados
- [ ] Formulários: validação, mensagem de sucesso, fallback sem JS quando viável

## 4. Stack padrão

> _Ajustar conforme a operação amadurece._

- **Sites institucionais / portfólio:** Webflow ou Astro + Sanity
- **Sites com lógica / app-like:** Next.js + Sanity / Payload
- **Landing pages rápidas:** Astro + Tailwind
- **Email transacional:** React Email
- **Análise:** Plausible (default) ou GA4 quando exigido pelo cliente
- **Hospedagem:** Vercel (Next/Astro), Webflow Hosting

## 5. Convenções de código

- Componentes em PascalCase, hooks em camelCase com prefixo `use`
- Sem CSS-in-JS; preferir Tailwind + CSS Modules quando precisar isolar
- Tokens de design em CSS custom properties no `:root`, mapeados no Tailwind config
- Acessibilidade: nunca remover outline sem substituir; aria-* só quando o HTML semântico não resolve
- Imagens sempre com `width`/`height` e `loading="lazy"` (exceto LCP)

## 6. Tom de voz da Vazio (não dos clientes)

Como a Vazio fala consigo mesma, nas propostas, nos case studies, no site:

- Direta, sem floreio
- Confiante sem ser arrogante
- Usa exemplos concretos, evita jargão de marketing
- Em escrita: vírgulas, pontos, parênteses. Travessões só em diálogos.

## 7. O que NÃO fazemos

- Não copiamos visual de projetos anteriores em projetos novos. Cada ID é nova.
- Não entregamos sem checklist da seção 3.
- Não aceitamos brief sem reunião de descoberta documentada.
- Não trabalhamos com escopo aberto; toda mudança vira change request.

## 8. Como usar este repo

- `STUDIO.md` (este arquivo): contexto sempre carregado.
- `briefs/`: brief de cada projeto novo. Começa do `_template.md`.
- `patterns/`: padrões **estruturais** reutilizáveis (layouts, fluxos), não visuais.
- `case-studies/`: registro de projetos entregues. Referência de qualidade, não de visual.
- `.claude/agents/`: agentes especializados disponíveis (ver `README.md`).
