# Page Layouts
* Alguns dos métodos usados para posicionar os elementos na tela.
* Tables
    Idéia inicial do css com html, fixa.
* Floats e clear
    Possibilidade de flutuar para outro lado da tela e clear para parar ele e não afetar os elementos.
* Frameworks e Grid Systems
    Dividia a tela em linhas para se adicionar em determinado lugar.

* Flexbox
    Mais atual
* Grid
    Mais atual e utilizado


# Posicionamentos
* Controla onde, na página, o elemento irá ficar, alterando o fluxo normal dos elementos.

* Name: position
* Value: static | relative | absolute | fixed
* Lembrando que o fluxo normal dos elementos é ficar um abaixo do outro, a não ser no caso de elementos inline, que ficam um ao lado do outro.
*     O position indica onde o elemento vai ser posicionado na página. Ao usar o position podemos adicionar outras propriedades como top, right, bottom, left e z-index, que vão determinar o posicionamento final do elemento.

## static
    Por padrão os elementos são static. Isso significa que os elementos irão seguir o fluxo normal do HTML.

## relative
    Quando o position é relative os elementos são deslocados do seu posicionamento normal, mas sem afetar o posicionamento de outros elementos da página.

## absolute
    Quando ativado é como se fosse para uma camada extra. Saindo do fluxo normal. É posicionado em relação ao seu parent element mais próximo. Se esse elemento "pai" não existir, ele será posicionando em relação a página.


## fixed
    Quando ativado fica fixo na página, é como se criasse um elemento flutuante que fica fixo na página, independente do scrolling feito.

# Element Stacking
É o empilhamento de elementos. Podemos usar o z-index para determinar a ordem da posição do elemento. Quanto maior o z-index, mais "acima" vai aparecer o elemento.

#### ####
