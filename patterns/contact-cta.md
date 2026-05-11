# Contato e CTA de fim de página

Padrão Vazio para fechar páginas e converter contato.

## Tipos

### 1. Conversa direta (default)
Bloco grande com pergunta convidativa ("Vamos conversar?") + link de email. Sem formulário.

- **Quando usar:** estúdio, consultoria, serviços de alto valor onde a primeira conversa importa mais do que a velocidade.
- **Email:** mailto direto, com `subject` pré-preenchido quando útil.

### 2. Formulário curto
3 a 5 campos máximo: nome, email, mensagem, e no máximo 1 ou 2 contextuais (tipo de projeto, prazo).

- **Quando usar:** cliente espera volume e precisa filtrar leads.
- **Sempre:** mensagem de sucesso clara após envio. Honeypot ou anti-spam. Sem captcha visível salvo se necessário.

### 3. Calendário embedado
Embed de Cal.com / Calendly direto na página.

- **Quando usar:** cliente vende reuniões agendadas (coaching, consultoria por hora).
- **Cuidado:** embed pesa; carregar sob demanda (intersection observer).

## Decisões transversais

- Em todo site, CTA de contato aparece em pelo menos 2 lugares: footer + uma vez no meio do conteúdo principal.
- Footer mínimo Vazio: logo, contato, redes (apenas as ativas), copyright, link "site por Vazio" (opcional, sempre discreto).
- Nunca usar "Get in touch" como única label. Sempre algo concreto: "Envie um email", "Marque 30 minutos", etc.
