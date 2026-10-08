# Ficha de Herói: Cavaleiro Gale

Página web em formato de ficha de RPG de um cavaleiro original, inspirado na estética sombria de Dark Souls, mas com um herói protetor e gentil.

## Estrutura de pastas

```
ficha-heroi/
├── index.html
├── css/
│   └── style.css
├── img/
│   └── gale.svg
└── README.md
```

## Universo e identidade visual

- **Personagem:** Gale, Cavaleiro Guardião da Chama Pálida.
- **Paleta (variáveis em `:root`):** azul da capa, prata do aço, ouro envelhecido e laranja de brasa sobre fundo quase preto.
- **Fontes (Google Fonts):** Cinzel nos títulos e IM Fell English nos textos.
- **Ícones:** Font Awesome 6.

## Decisões de UI/UX

1. **Hierarquia visual:** o nome do herói é o maior elemento da página, em ouro e com brilho de brasa. Depois vêm os títulos de seção e, por fim, o texto corrido.
2. **Contraste e legibilidade:** texto claro sobre fundo escuro, com contraste acima do mínimo WCAG AA. As fontes mais estilizadas ficam só nos títulos, e o corpo usa tamanho maior e entrelinha de 1.7 para compensar a fonte antiga.
3. **Consistência:** todos os cards seguem o mesmo padrão (borda, espaçamento e raio das bordas), e a cor da borda indica a raridade do item (comum, raro ou lendário).
4. **Affordance e feedback:** menu, botões e cards mudam de cor e crescem levemente no `hover`. Links e botões também têm destaque no foco do teclado (`:focus-visible`).
5. **Área de toque (Lei de Fitts):** itens do menu e botões têm no mínimo 44 a 48 px de altura.
6. **Proximidade (Gestalt):** em cada atributo, ícone, nome, valor e barra ficam juntos e separados dos outros atributos por um espaço maior.
7. **Fluxo de leitura:** as seções seguem a ordem do menu, que leva do herói (quem é) até o contato com a guilda.

## Requisitos atendidos

- HTML semântico: `header`, `nav`, `main`, `section`, `article`, `footer`, `h1` a `h3`, `p`, `img`, `a`, `ul`.
- Imagem com `alt` descritivo.
- CSS externo, com blocos comentados por seção.
- Flexbox no menu, Grid no inventário e `media queries` para 1, 2 e 3 colunas.
- Variáveis CSS usadas em vários elementos.
- Barras de atributo feitas só com HTML e CSS (`div` com `width` em porcentagem).
- `transition` em menu, botões e cards, e pseudo-elemento `::before` nos cards.
- Item de destaque lendário, links de comunidade e biografia com avatar.

## Como abrir

Abra o `index.html` no navegador. É preciso estar conectado à internet para carregar as fontes e os ícones.
