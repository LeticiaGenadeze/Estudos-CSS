### Estudando CSS com a <a href="https://www.rocketseat.com.br/">Rocketseat</a>

Neste repositório deixarei por escrito algumas questões teóricas e helps sobre CSS.

### CSS 
- [Conhecendo o CSS](#hello-css)
- [Comentários](#comentarios)
- [Box Model](#box-model)
- [Regra important](#regra-important)
- [Tipos Numéricos e Unidades Comuns](#numericos-unidades)


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