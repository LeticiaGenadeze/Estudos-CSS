### Estudando CSS

Neste repositório deixarei por escrito algumas questões teóricas e helps sobre CSS do curso que fiz com a <a href="https://www.rocketseat.com.br/">Rocketseat</a>

### CSS 
- [Conhecendo o CSS](#hello-css)
- [Comentários](#comentarios)
- [Box Model](#box-model)
- [Regra important](#regra-important)
- [Tipos Numéricos e Unidades Comuns](#numericos-unidades)
- [Position](#position)
- [Display block e inline](#display-block-inline)
- [Margin](#margin)
- [Padding](#padding)
- [Border-outline](#border-outline)
- [Cores](#cores)
- [Background](#background)
- [Posicionar os elementos na tela](#position)
- [Fontes](#fontes)


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

##

#### <a name="padding"></a> Padding

O padding é o preenchimento interno da caixa.

A propriedade padding pode ser escrita como nos formatos apresentados abaixo:
padding-top | padding-right | padding-bottom | padding-left

Geralmente usamos uma forma abreviada (shorthand) para escrever o padding. Esse formato segue o sentido horário iniciando pelo top, seguindo para right, bottom e left.

```css
padding: 12px 16px 10px 4px; /* TOP = 12px | RIGHT = 16px | BOTTOM = 10px | LEFT = 4px */
padding: 12px 16px 0; /* TOP = 12px | RIGHT = 16px | BOTTOM = 0px | LEFT = 16px */
padding: 8px 16px; /* TOP = 8px | RIGHT = 16px | BOTTOM = 8px | LEFT = 16px */
padding: 8px; /* TOP = 8px | RIGHT = 8px | BOTTOM = 8px | LEFT = 8px */
```

O padding pode ter valores (values) de comprimento (px, em, rem) ou de porcentagem (%)

O padding poderá causar diferença na largura de um elemento

##

#### <a name="border-outline"></a> Border-outline

São as bordas da caixa

value: border-style | border-width | border-color

style: solid | dotted | dashed | double | groove | ridge | inset | outset
width: length
color: color


```css
div {
	/* shorthand */
	border-top: solid 2px; /* top | right | bottom | left */

	/* style */
	border: solid;

	/* width <length> | style */
	border: 2px dotted;

	/* style | color */
	border: outset #f33;

	/* width | style | color */
	border: medium dashed green;

}
```
O outline é muito semelhante ao border, mas difere em 4 sentidos:
- Não modifica o tamanho da caixa, pois não é parte do Box Model
- Poderá ser diferente de retangular
- Não permite ajuste individuais
- Mais usado pelo user agent para acessibilidade

##

#### <a name="cores"></a> Cores

Usamos CSS para alterar cores do nosso documento.

Tipos:
- background-color (para caixas)
- color (para textos)
- border-color (para caixas)
- outros

Valores
- Podemos definir valores por:
- palavra-chave (blue, transparent)
- hexadecimal (#990011)
- funções: rgb, rgba, hsl, hsla

##

#### <a name="background"></a> Background

- Background-color

A propriedade background-color define a cor de fundo do elemento selecionado.

- Background-image

Para adicionar uma imagem como background podemos usar a propriedade background-image.
Por padrão a imagem vai se repetir e podemos modificar essa opção usando a propriedade background-repeat.

- Background-position

Com a propriedade background-position podemos mudar a posição da imagem do background.

- Background-size

Para mudar o tamanho da imagem do background usamos a propriedade background-size.

- Background-origin-clip

A propriedade background-origin é quem define o ponto de origem de uma imagem específica.
O background-clip define se a cor ou imagem do background iniciam debaixo de sua área de borda, preenchimento ou conteúdo.

- Background-attachment

A propriedade background-attachment determina se a posição da imagem vai ser fixa ou se vai rolar junto com o conteúdo.

- Gradient

linear-gradient() é a função usada para criar gradient linear com o CSS.
radial-gradient() é a função usada para criar gradient circular.

##

#### <a name="position"></a> Posicionar os elementos na tela

- Position

Controla onde, na página, o elemento irá ficar, alterando o fluxo normal dos elementos.

Name: position
Value: static | relative | absolute | fixed

Lembrando que o fluxo normal dos elementos é ficar um abaixo do outro, a não ser no caso de elementos inline, que ficam um ao lado do outro.

- Static 

Por padrão os elementos são static. Isso significa que os elementos irão seguir o fluxo normal do HTML.

- Relative

O position indica onde o elemento vai ser posicionado na página. Ao usar o position podemos adicionar outras propriedades como top, right, bottom, left e z-index, que vão determinar o posicionamento final do elemento.

Quando o position é relative os elementos são deslocados do seu posicionamento normal, mas sem afetar o posicionamento de outros elementos da página.

- Absolute

Quando o position é absolute o elemento é deslocado saindo do fluxo normal. O elemento de position absolute é posicionado em relação ao seu parent element mais próximo. Se esse elemento "pai" não existir, ele será posicionando em relação ao bloco contendo a raiz do elemento.

- Fixed

Quando aplicado o position fixed é como se criasse um elemento flutuante que fica fixo na página, independente do scrolling feito.

- Element Stacking

É o empilhamento de elementos. Podemos usar o z-index para determinar a ordem da posição do elemento. Quanto maior o z-index, mais "acima" vai aparecer o elemento.

- Flexbox

Nos permite posicionar os elementos dentro da caixa
Controle em uma dimensão (horizontal ou vertical)
Alinhamento, direcionamento, ordenar e tamanhos

```css
div.parent {
	display: flex;
}
```

- Flex-direction
    - Qual a direção do flex: horizontal ou vertical
    - row | column

- Alinhamento
    - justify-content
    - align-items


##

#### <a name="fontes"></a> Fontes

- Font Family
Tipo de fonte de um elemento

- Font Weight
Peso da fonte
Valores: normal | bold | bolder | lighter | 100 | 200 | 300 | 400 | 500 | 600 | 700 | 800 | 900
Dependendo da família da fonte não conseguimos utilizar todos os pesos de fonte

- Font Style
É o estilo da fonte
Valores: normal | italic | oblique
Os valores que podem ser aplicados dependem da fonte usada

- Font Size
Tamanho da fonte





##



Referências:

 https://developer.mozilla.org/en-US/docs/Web/CSS/border
