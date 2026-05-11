# Hero layouts

Tipos de hero usados em projetos Vazio. Quando começar um projeto novo, escolha a variante e adapte; não invente um quinto tipo sem necessidade real.

## 1. Editorial split

Headline grande à esquerda, mídia à direita (vídeo curto loop ou imagem). Funciona para institucional e portfólio.

- **Quando usar:** cliente tem boa imagem ou vídeo de produto e a headline carrega a proposta.
- **Quando evitar:** cliente sem assets visuais; vira logo + texto.
- **Exemplos:** _(preencher com case studies quando houver)_

## 2. Type-only

Apenas tipografia, sem mídia. Headline ocupa a maior parte da viewport.

- **Quando usar:** marca com tipografia forte; conteúdo intelectual (consultoria, advocacia, autoria).
- **Quando evitar:** e-commerce, produto físico, qualquer coisa que precise ser vista.

## 3. Hero modular (cards)

Grid de 2 a 4 cards abaixo de uma headline curta, cada card linka para uma seção/produto.

- **Quando usar:** site com múltiplas linhas de produto ou serviço.
- **Quando evitar:** site com proposta única; fragmenta o foco.

## 4. Full-bleed media

Vídeo ou imagem ocupa 100% da viewport, headline sobreposta.

- **Quando usar:** marca com forte direção visual, lifestyle, moda, arquitetura.
- **Quando evitar:** se a imagem não for excelente. Hero ruim em full-bleed mata o site.
- **Cuidado:** contraste do texto sobre mídia; sempre usar overlay ou backdrop.

## Decisões transversais

- LCP do hero precisa ficar abaixo de 2.5s. Pré-carregar a imagem/vídeo de cima.
- Se for vídeo, sempre com `poster`, `muted`, `playsinline`, autoplay opcional.
- Headline nunca passa de 8 palavras. Subhead complementa, não repete.
