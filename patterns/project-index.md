# Índice de projetos (portfólio)

Como organizar a página que lista os projetos de um cliente (ou da própria Vazio).

## Layouts comuns

### Lista vertical com hover-preview
- Lista de nomes em tipografia grande.
- Ao hover, preview da imagem aparece (canto da tela ou inline).
- Funciona bem para portfólio de estúdio, fotógrafo, designer.

### Grid 2 ou 3 colunas
- Cards com imagem + título + 1 tag.
- Funciona para portfólio com volume (10+ projetos) e variedade visual.

### Timeline / scroll horizontal
- Projetos em sequência cronológica.
- Bom para arquitetura, processo, antes/depois.
- Cuidado em mobile: precisa virar vertical com clareza.

## Decisões transversais

- Ordenação padrão: mais recente primeiro. Filtros adicionais (tipo, ano) só se houver 12+ itens.
- Cada card linka para a página do case (sem modal). Modal só se o case for muito curto.
- Carregamento: primeiros 6 a 8 itens; depois lazy ou paginação. Nunca infinite scroll sem botão de "ver mais".
- Hover preview precisa ter fallback em touch: tap leva direto ao case.
