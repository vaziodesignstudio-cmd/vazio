# Hero layouts (empresa de limpeza)

Variantes de hero para a página inicial de um site de empresa de limpeza. Escolha uma, adapte com a ID visual do cliente, e não invente uma quinta sem motivo real.

O hero é responsável por: (1) provar que o serviço entrega resultado e (2) dar acesso imediato ao contato. Headline sem CTA visível é hero ruim aqui.

## 1. Antes/depois (default)

Slider de comparação ou par lado a lado mostrando "como estava" e "como ficou". Headline + CTA sobrepostos ou ao lado.

- **Quando usar:** maioria dos casos. Antes/depois é a prova social mais forte que uma empresa de limpeza tem.
- **Quando evitar:** cliente sem fotos próprias decentes; foto genérica de banco de imagens estraga o efeito.
- **Cuidado:** as duas fotos precisam ser do **mesmo ângulo**, **mesma luz**, **mesmo enquadramento**. Antes/depois mal pareado parece falso.
- **Mobile:** virar pra vertical (antes em cima, depois embaixo) com label clara. Slider horizontal sofre em touch.

## 2. Vídeo do serviço em ação

Loop curto (5 a 12 segundos) do serviço acontecendo: passagem de pano em superfície brilhante, aspirador em ação, brilho final. Headline sobreposta.

- **Quando usar:** cliente tem material de vídeo gravado (ou aceita gravar). Funciona muito bem em comercial e pós-obra.
- **Quando evitar:** sem material gravado próprio. Vídeo genérico parece comercial de TV ruim.
- **Sempre:** `poster`, `muted`, `playsinline`, autoplay. Sem áudio. Sem controles visíveis.
- **Performance:** vídeo otimizado, <1MB pro mobile. Se passar disso, é imagem estática mesmo.

## 3. Foto full-bleed do espaço limpo

Imagem grande de um ambiente impecável (sala, cozinha, escritório, área externa). Headline + CTA sobrepostos com overlay de contraste.

- **Quando usar:** cliente tem boas fotos de espaços pós-limpeza. Bom pra serviços residenciais de alto padrão e comercial corporativo.
- **Quando evitar:** se a foto não for excelente. Em full-bleed, foto medíocre mata a marca.
- **Sempre:** overlay escuro sutil ou backdrop atrás do texto pra garantir contraste (WCAG AA mínimo).

## 4. Hero com telefone visível (foco em conversão)

Headline curta + botão "Ligar agora" (com número visível) + botão WhatsApp + imagem/vídeo lateral menor.

- **Quando usar:** cliente prioriza ligação imediata sobre form (operação local pequena, alto valor de cada lead, conversão por telefone).
- **Quando evitar:** cliente com operação a distância ou que prefere triagem por form.
- **Mobile:** os botões "Ligar" e "WhatsApp" viram **CTAs primários do hero**, não secundários. Tap-target ≥ 48px.

## 5. Hero modular (múltiplos serviços)

Headline curta + grid de 2 a 4 cards de tipos de serviço (residencial, comercial, pós-obra, profunda), cada card linka pra Service page correspondente.

- **Quando usar:** empresa atende segmentos distintos com decisões diferentes. Ajuda o visitante a se identificar rápido.
- **Quando evitar:** empresa com proposta única ("limpeza residencial premium"). Fragmenta foco sem necessidade.

## Decisões transversais

- **LCP < 2.5s** no hero. Pré-carregar a imagem/vídeo do topo. Se for vídeo, pode renderizar o `poster` primeiro e trocar.
- **Headline ≤ 8 palavras.** Subhead complementa com prova ou prazo ("Atendimento em até 24h", "Atendemos toda a zona sul").
- **CTA primário sempre visível no hero.** Em empresa de limpeza, esse CTA é quase sempre telefone, WhatsApp ou "Solicitar orçamento". Nunca "Saiba mais".
- **Trust signals no hero ou logo abaixo:** anos de atuação, nº de clientes atendidos, selo de empresa cadastrada, ou nota Google. Uma linha discreta.
- **Acessibilidade:** texto sobreposto a imagem precisa de contraste real (medir, não estimar). Vídeo nunca pode ser a única fonte de informação — headline em texto sempre.
