---
client: "Heloame Cleaning Services"
project: "Landing page"
start_date: "2026-07-02"
deadline: ""            # a definir com a cliente
budget: ""             # a definir com a cliente
status: discovery      # discovery | design | dev | qa | live
brief_owner: "Lucas"
---

# Brief — Heloame Cleaning Services / Landing page

> Este brief é a referência para todo o time durante o projeto. Toda decisão volta para cá. Mudanças geram change request, não edição silenciosa.
>
> Fonte primária: formulário "Criação de Site" preenchido pela cliente em 2026-06-19 (`brands-assets/Heloame Cleaning Services/Criação de Site.csv`, linha da Heloame). Onde o formulário deixou em branco, está marcado como **a definir**. Não inventar dado de negócio.

---

## 1. Sobre o cliente

- **O que faz:** empresa de serviços de limpeza (residencial, escritório, move-in/out, pós-obra), com planos recorrentes. Negócio familiar.
- **Para quem:** proprietários de imóveis (casas, apartamentos, condomínios) e pequenos escritórios na grande Columbus, Ohio (EUA). Conteúdo do site em **inglês**.
- **Tamanho / momento:** microempresa (3 a 10 funcionários), 3 anos de operação. Family-owned.
- **Concorrentes mais próximos:** outras cleaning companies da mesma região (Columbus/OH). A própria cliente citou **Wylla's Cleaning** como referência para a aba de planos.

## 2. Por que estão aqui

Colocar a operação online com uma landing page profissional que gere contato direto (telefone / futuramente formulário e redes). Hoje não há site — o canal é telefone e boca a boca. O site precisa transmitir confiança de negócio familiar sério e capturar leads da região atendida.

## 3. Objetivo do projeto

Publicar uma landing page de conversão que transforme visitantes em contatos (ligação / orçamento), posicionando a Heloame como opção confiável de limpeza em Columbus e arredores.

> Meta mensurável a fechar com a cliente na descoberta (ex.: "X ligações/orçamentos por mês nos primeiros 3 meses").

## 4. Métricas de sucesso

- Métrica 1: nº de cliques em "ligar" / contato por mês — **meta a definir**.
- Métrica 2: nº de orçamentos solicitados por mês — **meta a definir**.
- Métrica 3: Lighthouse mobile ≥ 90 nas 4 categorias (padrão de qualidade Vazio, `STUDIO.md` §3).

## 5. Escopo

### Inclui
- [x] Landing page única (single page, sem CMS/atualização) — tipo escolhido pela cliente.
- [x] Seções core do pattern de negócio de serviços (ver §6 e `patterns/service-business-site.md`): Hero (com vídeo), Services, About, Why choose us, Gallery, Contact, Areas we serve, Hours, Footer.
- [x] Aba/seção de **planos** (Weekly / Biweekly / Monthly / Deep Cleaning), inspirada estruturalmente na Wylla's Cleaning.
- [x] Click-to-call sticky no mobile + SEO local (schema `LocalBusiness`, `areaServed`).

### Não inclui
- [ ] CMS / painel de edição (é landing estática).
- [ ] E-commerce / pagamento online.
- [ ] Blog ou páginas por serviço dedicadas (podem virar change request depois).
- [ ] Redes sociais, Google Business e documentos legais — a cliente enviará depois (ver §11).

## 6. Direção visual

> Exceção legítima à regra "não puxar visual de outro projeto": **a própria cliente forneceu a ID** (paleta e tipografia) no formulário. Registrado abaixo. Confirmar e refinar na descoberta; não copiar de outro case Vazio.

- **Personalidade da marca:** confiável, familiar, detalhista, profissional, premium-acessível.
- **Paleta inicial (do formulário):**
  - Primárias / texto: preto `#000000`, cinza-escuro `#404040`.
  - Neutros / fundo: `#eeeeee`, branco `#ffffff`.
  - Acento — **degradê dourado**: `#bda462` → `#ffedb4` → `#bda462`.
- **Tipografia inicial:** Montserrat (títulos e corpo). Definir pesos e escala tipográfica na fase de design.
- **Referências aprovadas:** logo, galeria e materiais gráficos reais em `brands-assets/Heloame Cleaning Services/` (ver inventário abaixo). Wylla's Cleaning como referência **estrutural** da aba de planos.
- **Anti-referências:** a definir com a cliente (o que não pode parecer — genérico, poluído, "cupom de desconto", etc.).

### Inventário de assets (`brands-assets/Heloame Cleaning Services/`)
- **Logo/** — PNG (2 versões) + SVG.
- **Gallery/** — 6 imagens (6–11.png).
- **Services/** — 4 artes: Residential, Office, Move in & Out, Post-Construction.
- **Graphic Material/** — Business Card e Flyer (PDF).
- **Video - Inicio/** — `Website - Heloame Cleaning Services .mp4` (para o hero).
- **Google Drive (mídias):** https://drive.google.com/drive/folders/1TXXgms-gfHNb9IIU0mxxOxiJnNRsEfYe — **verificar conteúdo e baixar o que faltar**.

## 7. Stack proposta

Landing estática rápida → default de landing do `STUDIO.md` §4.

- **Frontend:** Astro + Tailwind (tokens de cor/tipografia em CSS custom properties).
- **CMS:** nenhum (conteúdo fixo em código).
- **Hospedagem:** Vercel (ou Webflow, se a cliente preferir editar sozinha depois — decidir na descoberta).
- **Analytics:** Plausible (default).

## 8. Conteúdo

- **Quem escreve:** Misto — a cliente já forneceu quase todo o copy no formulário (headlines, serviços, about, why-choose-us, checklists). Vazio revisa/edita para ritmo e SEO.
- **Idiomas:** EN (público de Columbus, OH).
- **Estado atual:** conteúdo **pronto** (do formulário), a revisar. Faltam: depoimentos/reviews, links de redes, e-mail definitivo (o atual é provisório).

### Copy aprovado pela cliente (do formulário)
- **Hero (Home):** "Reliable Cleaning Solutions for Your Home"
- **Services — título:** "Professional Cleaning Services You Can Trust" · **parágrafo:** "We provide cleaning services designed to keep your home clean, comfortable, and welcoming."
- **Serviços (4 + planos):** Residential, Office, Move-In/Move-Out, Post-Construction, cada um com checklist detalhado; planos Weekly / Biweekly / Monthly / Deep Cleaning. Texto integral no CSV.
- **About — título:** "A Family-Owned Company Committed to Quality" · **parágrafo:** 3 anos de experiência, negócio familiar, foco em qualidade, comunicação clara e satisfação do cliente.
- **Why choose us — título:** "Why Homeowners Choose Us" · **diferenciais:** 1) Family-Owned, 2) 3 anos de experiência, 3) Attention to detail, 4) Clear & efficient communication, 5) Professionalism, 6) 100% satisfaction guaranteed, 7) Exceed expectations, 8) Quality over speed.
- **Gallery — título:** "Our Excellence!"

### Dados de contato (do formulário)
- **Telefone:** (614) 260-3655
- **E-mail:** heloamealmeida@icloud.com *(provisório — confirmar o definitivo)*
- **Localização:** Columbus, Ohio
- **Areas we serve (26):** Bexley, Blacklick, Canal Winchester, Clintonville, Columbus, Delaware, Dublin, Galena, Gahanna, Galloway, Grove City, Groveport, Hilliard, Johnstown, Lewis Center, Marysville, New Albany, Pataskala, Pickerington, Plain City, Powell, Reynoldsburg, Sunbury, Upper Arlington, Westerville, Worthington.
- **Horário:** Seg–Sáb 8am–6pm · Dom fechado.
- **Instagram / Facebook / Google Business:** *"enviar posteriormente"* — pendente.

## 9. Cronograma

| Fase | Início | Entrega | Responsável |
|---|---|---|---|
| Descoberta | 2026-07-02 |  | Lucas |
| Design  |  |  |  |
| Dev |  |  |  |
| QA |  |  |  |
| Go-live |  |  |  |

> Datas a fechar com a cliente.

## 10. Stakeholders

- **Decisor final:** Heloame Almeida (proprietária).
- **Ponto de contato diário:** a confirmar.
- **Aprovadores adicionais:** —

## 11. Riscos conhecidos

- Risco: redes sociais, Google Business e docs legais ainda não enviados → mitigação: publicar com placeholders/links ocultos e ativar quando chegarem; NAP consistente desde o início.
- Risco: e-mail de contato é provisório → mitigação: confirmar o definitivo antes do go-live (evita retrabalho de SEO/NAP).
- Risco: sem reviews/depoimentos ainda → mitigação: reservar a seção Reviews no layout e preencher pós-coleta (schema `Review` quando houver).
- Risco: pasta do Google Drive de mídias não verificada → mitigação: auditar conteúdo antes do design para não faltar imagem em alta.

## 12. Decisões registradas

- 2026-07-02 — Projeto criado a partir do formulário "Criação de Site" (resposta de 2026-06-19). Tipo: landing page única. Stack default de landing (Astro + Tailwind). ID visual usa a paleta/tipografia fornecidas pela cliente (preto/cinza/branco + degradê dourado, Montserrat).
