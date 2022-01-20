### Estudando CSS com a <a href="https://www.rocketseat.com.br/">Rocketseat</a>

Neste repositório deixarei por escrito algumas questões teóricas e helps sobre CSS.

### CSS 
- [Conhecendo o CSS](#hello-css)
- [Comentários](#comentarios)
- [Box Model](#box-model)
- [Regra important](#regra-important)
- [Tipos Numéricos e Unidades Comuns](#numericos-unidades)
- [Position](#position)
- [Display block e inline](#display-block-inline)

##

#### <a name="hello-css"></a> Conhecendo o CSS

CSS é um acrônimo para Cascading Style Sheet, uma forma de escrever uma folha de estilos em cascata;

O CSS é um código para criar estilos no HTML, que é a estrutura de todo o documento, já o CSS seria a beleza, a "parte bonita".

CSS não é uma linguagem de programação.

##

#### <a name="comentarios"></a> Comentários

Os comentários no css não irão afetar o código e podem nos ajudar a lembrar de blocos de códigos ou agrupar e organizar nosso código.

Os comentários abrem com /* e terminam com */ .

##

#### <a name="box-model"></a> Box Model

É uma caixa retangular. Essa caixa possui as mesmas propriedades de uma caixa 2D, e tem como propriedades:
- Tamanho (largura x altura width e height, respectivamente
- Conteúdo: o content
- Bordas: o border
- Preenchimento interno: o padding
- Espaços fora da caixa: a margin

##

#### <a name="regra-important"></a> Regra important

sintaxe: !important

São raras as ocasiões nas quais se devem usar um iportant, pois é em geral uma má pratica, visto que quebra o fluxo natural da cascata e pode acabar te atrapalhando caso você a deixe em algum lugar no seu código.

Portanto evitar ao máximo seu uso.

##

#### <a name="numericos-unidades"></a> Tipos numéricos e Unidades Comuns

Tipos numéricos:

- integer - número inteiro como -10 ou 223
- number - número decimal como -2.4, 64 ou 0.234
- dimension - é um <number> com uma unidade junto: 90deg, 2s, 8px
- percentage - representa uma fração de outro número: 50%

Unidades comuns: 

- length - é um dos mais usados no CSS e representa um valor de distância: px, em, vw
- angle - representa um ângulo: deg, rad, turn
- time - representa um tempo: s, ms
- resolution - representa resoluções para dispositivos: dpi

##

#### <a name="position"></a> Position

<position>

Representa um conjunto de coordenadas
top, right, bottom, left e center
Usado para alguns tipos de propriedades como o background-position
Não confundir com a propriedade position

##

#### <a name="display-block-inline"></a> Display block e inline

display: block; vs display: inline;

- Display Block
    - Ocupa toda a linha, colocando o próximo elemento abaixo desse
    - width e height são respeitados
    - padding, margin, border irão funcionar normalmente
    - p, div, section, todos os headings: h1, h2

- Display Inline
    - Os elementos ficam ao lado do outro e não empurram outros elementos para baixo
    - width e height não funcionam
    - Somente valores horizontais de margin
    - a, strong, span, em 

##

#### <a name="margin"></a> Margin

Margin, é o espaço (margem) entre os elementos

Podemos dividir o margin em 4 valores:

margin-top | margin-right | margin-bottom | margin-left

Geralmente usamos uma forma abreviada (shorthand) para escrever o margin. Esse formato segue o sentido horário iniciando pelo top, seguindo para right, bottom e left.

```css
margin: 12px 16px 10px 4px; /* TOP = 12px | RIGHT = 16px | BOTTOM = 10px | LEFT = 4px */
margin: 12px 16px 0; /* TOP = 12px | RIGHT = 16px | BOTTOM = 0px | LEFT = 16px */
margin: 8px 16px; /* TOP = 8px | RIGHT = 16px | BOTTOM = 8px | LEFT = 16px */
margin: 8px; /* TOP = 8px | RIGHT = 8px | BOTTOM = 8px | LEFT = 8px */
```