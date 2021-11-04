# Flexbox

# Layouts e evolução
* Layout tem a ver com a maneira com que os elementos estão distribuidos na tela

# Normal flow
* Ou Flow Layout é a maneira que os elementos `block` e `inline` ficam na página
* Block ocupa a linha toda, enquanto Inline somente o elemento

## Tables
* É a maneira de tabelas onde a tag `table` recebe um display `table` fazendo com que os elementos interno como `td` e `tr` possam ser usados para montar tabela
<table>
    <tr> = linha
        <td> </td> = coluna
        <td> </td>
    </tr></table>

## Tableless
* Uso das propriedades `float`, `clear` para que os elementos possam mudar de posição na tela.

<div style="float: left">esquerda</div> posiciona a esquerda
<div style="float: right">direita</div> posiciona a direita
<div style="clear: both">normal</div> limpa os posicionamentos anteriores e começa a ser normal a partir deste

# Flexbox

* A caixa se torna flex, fazendo com que os elementos internos possam receber melhor:

- Alinhamento
- Ordenação
- Tamanhos flexíveis

* Conseguimos alterar praticamente tudo na flexbox

# Terminologias

- Flex Container (caixa com elementos dentro)
    - Flex item (elementos = item)        
- Nesting (elementos vivem dentro de outros elementos)
- Axis(eixos)
    - main (eixo principal)
        - start, end
    - cross (eixo cruzado)
        - start, end
(mais ou menos X e Y da matematica, mas podemos alterar o comportamento dos eixos e inverte-los)
- Flex sizing (item flexível)
    - flexível
    - altera width/height dos itens para preenchimento dos espaços do flex container
    - Ex: flex:1;

# Propriedades do Flex container
## Direção dos itens
* Flex é uma dimensão(horizontal ou vertical)
* Podemos mudar a direção com `flex-direction`
* valores: (row | row-reverse | column | column-reverse)

# Flex Wrap
* Podemos usar Multi Linhas
* Criar nova linha, um novo flex container, ou um novo eixo principal
    `flex-wrap: wrap;`
    `flex-wrap: wrap-reverse;` todos são quebrados para cima, invertendo
    * Alinhamento 
        * Principal 
        * Cruzado
    * Espaços entre os itens

# Flex flow
* Shorthand; uma unica propriedade para escrever os demais
 * juntamos `flex-direction` e `flex-wrap`
 * a primeira é direction e a segunda wrap:
  `flex-flow: column wrap-reverse`

  # justify-content
  - Alinhamento dos elementos dentro do container
  - Distribuição dos elementos no eixo principal
  ## valores
    - flex-start (padrão)
    - flex-end
    - center
    - space-around
    - space-between
    - space-evenly
    * Independente da direção da coluna ele seguirá essas regras

# align-items
- Alinhamento dos elementos no eixo cruzado
- Por padrão é stretch

## Valores:
- stretch
- flex-start
- flex-end
- center

# gap (espaço entre os elementos)
## Valores
 *  Unidades de medida
        fixas: px, pt
        flexíveis: %, em, rem

# Propriedade para os itens
# flex-basis
    * Por padrão já é automático `flex-basis: auto;`.
    * Se estiver em linha ele edita a largura, se estiver em coluna(column) ele edita a altura. Ou seja, relativo ao eixo principal.
    * Se editar um filho a ordem atendida ainda será do flex-basis.

# flex-grow
    * Crescimento do item dentro do container em relação aos espaços vazios.
        * Ex: Se quero que os itens "B" e "C" ocupe todo espaço vazio
        * Ex²: Se quero que o item "A" ocupe o espaço vazio
    * Se estiver em linha ele edita a largura, se estiver em coluna(column) ele edita a altura. Ou seja, relativo ao eixo principal. Necessário ter uma altura

# flex-shrink
    * Capacidade do item encolher dentro do container.
    * Por padrão flex-shrink é 1.
    * Se fazer `flex-shrink: 0` informamos que não queremos que seja encurtado mais e ele ultrapassa os limites.

# flex
* shorthand
* Podem ter 1, 2 ou 3 valores
* flex-grow; flex-shrink; flex-basis
* Por padrão: flex: 1 1 0;
* Quando troco o segundo elemento por `px` css entende que é o flex-basis.

`flex exemplificado na prática na pasta flex`

# order
* Ordenando itens
* De 0,1,2... determina a ordem
* Por padrão todos são 0
* Aceita negativos
* Muda visualmente mas não muda html, em caso de acessibilidade mudar na estrutura.