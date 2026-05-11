# Site de negócio local de serviços

Estrutura padrão para o arquétipo dominante de cliente Vazio: negócio local de serviços (cleaning, landscaping, contractor, pet care, beauty, automotive, etc.). Foco em SEO local, prova social e conversão por contato direto.

Esse pattern cobre as duas páginas-chave: **Homepage** e **Service page**. Outras páginas (About dedicada, FAQ, Pricing) entram conforme o brief.

## Homepage — estrutura core

Ordem default. Variações aceitáveis estão na seção de variações.

1. **Hero** — imagem ou vídeo + headline + logo + CTA primário
2. **Services** — grid de serviços oferecidos (3 a 6)
3. **About us** — quem é o negócio em 1 ou 2 parágrafos + foto
4. **Why choose us** — 3 a 5 diferenciais com ícone/número
5. **Gallery** — antes/depois, portfólio de trabalhos, ou imagens do serviço em ação
6. **Reviews** — depoimentos de clientes (3 a 6) com nome, foto opcional, estrela
7. **Follow us (Instagram)** — feed ou grid de últimos posts
8. **Contact (form)** — formulário curto + telefone + email
9. **Areas we serve** — cidades/bairros atendidos
10. **Footer** — logo, contato, redes, copyright, links legais

## Homepage — add-ons opcionais

Entram quando o cliente justificar. Não incluir sem motivo.

- **Pricing plans** — quando o cliente oferece pacotes claros (cleaning recorrente, planos mensais). Evitar se preço é por orçamento.
- **FAQ** — quando o serviço gera 5+ perguntas frequentes reais. Não inventar perguntas só pra encher.
- **Company policies** — termos, garantia, política de cancelamento. Útil pra serviços de alto valor ou recorrentes.
- **Mission / Values** — quando o cliente tem narrativa forte (negócio familiar, sustentável, comunitário). Evitar quando vira clichê.
- **CTA intermediário** — bloco "Marque agora" no meio do scroll. Bom em homepages longas (>10 seções).

## Service page — estrutura core

Página dedicada a um serviço específico. Linka da Homepage e do menu.

1. **Headline + parágrafo + image** — o quê é o serviço, pra quem, com hero próprio
2. **Schedule details** — duração, frequência, o que está incluso, o que não está
3. **Checklist** — itens do serviço em lista (gera confiança e ajuda SEO)
4. **Follow us (Instagram)** — mesmo bloco da home
5. **Contact (form)** — com campo "service" **pré-populado** com o nome desse serviço
6. **Areas we serve** — mesmas cidades/bairros (ou subset, se o serviço é geograficamente limitado)
7. **Footer**

## Variações de ordem aceitáveis

- **Reviews ↔ Gallery:** pode trocar. Reviews antes funciona quando a prova social é mais forte que o portfólio visual.
- **About ↔ Services:** Services primeiro vende mais rápido; About primeiro funciona quando a marca pessoal importa (terapeuta, advogado, profissional autônomo).
- **Why choose us:** pode ir logo após Hero (pitch curto) ou depois de Services (justifica a oferta). Não deixar no fim — esfria.
- **Areas we serve:** pode subir pro topo (depois do Hero) em clientes com forte foco geográfico ("cleaning em Barra da Tijuca"). Default é antes do footer.

## Decisões transversais

### SEO local
- "Areas we serve" não é decorativa — cada área vira uma chance de ranquear. Considerar **uma landing por cidade** quando o cliente atende 5+ áreas distintas.
- Schema.org `LocalBusiness` no `<head>` da home, com `areaServed`, `address`, `geo`, `openingHours`.
- NAP (Name, Address, Phone) consistente entre site, Google Business Profile e diretórios.

### Reviews com rich snippets
- Marcar reviews com schema.org `Review` ou `AggregateRating` no JSON-LD.
- Sempre indicar fonte (Google, Yelp, Instagram). Reviews sem fonte verificável geram desconfiança.
- Não rotacionar com carrossel automático — quebra acessibilidade e ninguém termina de ler.

### Instagram embed
- Embed oficial do Instagram é pesado (~600KB de JS). Carregar **sob demanda** com intersection observer, ou usar grid estático puxado via API/snapshot diário.
- Sempre ter fallback: se o embed falhar, mostrar link "Ver no Instagram @handle".

### Contato e telefone
- **Click-to-call sticky** em mobile (botão flutuante ou no header sticky). Maior alavanca de conversão em empresa de limpeza.
- WhatsApp via link `wa.me/` é praticamente obrigatório no Brasil.
- Form de contato: 3 a 5 campos. Service page passa o nome do serviço via query param ou estado, e o form pré-popula o campo "service".
- **CTA aparece em pelo menos 2 lugares na página:** hero + footer. Em página longa (>10 seções), inserir um terceiro CTA intermediário.
- **Labels concretas, nunca "Entre em contato" ou "Saiba mais".** Use ação direta: "Solicitar orçamento", "Ligar agora", "Falar no WhatsApp", "Agendar visita".
- **Calendário embedado (Cal.com / Calendly)** vale quando o cliente vende **visita técnica agendada** ou **orçamento presencial marcado**. Carregar sob demanda (intersection observer) — embed pesa.

### Gallery / portfólio
- Antes/depois funciona muito bem em cleaning, landscaping, automotive, beauty. Usar slider de comparação ou par lado a lado, nunca GIF.
- Imagens com `width`/`height` declarados, `loading="lazy"` exceto a do hero. Otimizar para mobile (maior parte do tráfego).

### Form de contato
- Campos mínimos: nome, telefone, serviço, mensagem opcional. Email só se o cliente prefere email a telefone.
- Honeypot anti-spam. Sem captcha visível salvo se houver spam comprovado.
- Mensagem de sucesso clara + opção de chamar no WhatsApp imediatamente.

### Footer mínimo
- Logo, NAP completo, redes ativas (não inventar), copyright, link "site por Vazio" discreto.
- Repetir o CTA principal (botão de contato) no footer — converte mais que parece.
