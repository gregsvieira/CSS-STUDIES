# Trabalhando com fontes
* A tipografia transmite uma mensagem

- negrito
- tamanho
- estilo

## Basic Font Properties

font-family
font-weight
font-style
font-size


## Font Family

* Tipo de fonte de um elemento
* Lista de fontes e ordem de prioridade
* inclui *fallback*(plano b) font
    - serif (fontes serifadas, com pés)
    - sans-serif (fontes não serifadas, sem pés)

Exemplo:
p {
    font-family: "Times New Roman", Times, serif;
}
Explicação: 
    familia-da-fonte: "Fonte 1º opção", Se não achar a primeira opção, se não achar a segunda opção;


## Font Weight
* Peso da fonte
* Valores: normal | bold | bolder | lighter | 100 | 200 | 300 | 400 | 500 | 600 | 700 | 800 | 900
* Dependendo da família da fonte não conseguimos utilizar todos os pesos de fonte

## Font Style

* É o estilo da fonte
* Valores: normal | italic | oblique
* Os valores que podem ser aplicados dependem da fonte usada

## Font-size
* Tamanho da fonte

* Referência
https://www.w3.org/TR/css-fonts-3/



##### ###### 

# Web Fonts

* Fontes do sistema x Fontes da web

* Fontes do sistema são as fontes que estão instaladas na máquina do usuário e nem sempre o cliente vai ter instalado as fontes usadas no projeto e isso pode fazer com que os estilos dos textos não sejam aplicados corretamente, mas para resolver esses casos podemos preparar nossas fonts para web ou usar fontes da web.

* Como usar fontes para web?

* @font-face
* @import (colocado no css)
ex: 
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+Mono:wght@300&display=swap');
* link (colocado no head html)
ex: 
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Mono:wght@300&display=swap" rel="stylesheet">


* Referências:
* https://fonts.google.com/
* https://css-tricks.com/snippets/css/using-font-face/

##### ###### 

# Font Variant
* Faz variações na apresentação da fonte
Ex: font-variant: small-caps
que põe mini capslock
https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant


# Font Stretch

* Alargamento ou encolhimento da fonte
* Aceita palavras-chaves como: expanded, condensed, normal
* Aceita porcentagens de 50% a 200%
* Essa propriedade não vai funcionar em todas as fontes


p {
	font-stretch: expanded;
}

https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch

Referência
https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals


# Letter spacing
* Define o espaçamento entre os caracteres
        Ref: https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing


# word-spacing
* Define o espaçamento entre palavras
    Ref: https://developer.mozilla.org/en-US/docs/Web/CSS/word-spacing

# Line-height
* Define os espaços entre linhas
* Pode ser com unidades ou sem unidades de medida
* Valores comuns: 1.5 ou 2
    https://developer.mozilla.org/en-US/docs/Web/CSS/line-height

# Text-transform
* Transformação do texto
* Valores podem ser: none | capitalize | uppercase | lowercase | full-width | full-size-kana
https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform


# Text-decoration
* Aparência decorativa de um texto
* line: underline | overline | line-through
* podemos aplicar mais de 1 valor
* style: wavy | dotted | double | dashed | solid
* color: <color> values


https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration

# Text-align
* Alinhamento de um texto
* Valores: start | end | left | right | center | justify | match-parent


https://developer.mozilla.org/en-US/docs/Web/CSS/text-align


# text-shadow
* Sombra aplicada a um texto
* Permite múltiplos valores
1px 1px 1px red,
2px 2px 1px green;
/* offset-x | offset-y | blur-radius | color */

https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow


# Shorthand
* Podemos usar o shorthand font para determinar os seguintes valores: 
font-style, font-variant, font-weight, font-stretch, font-size, line-height e font-family
  
  font: italic normal bold normal 3em/1.5 Helvetica, Arial, sans-serif;
