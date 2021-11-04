# Pseudo-classes

* É um tipo de seletor que irá selecionar um elemento que estiver em um estado específico.

** Exemplo: É o primeiro elemento dentro de uma caixa, ou, o elemento está com o ponteiro do mouse sobre ele.

Pseudo-classes começam com 2 pontos seguido do nome da pseudo class :pseudo-class-name

## Selecionando elementos com pseudo-classes

* :first-child
    Primeiro elemento filho

* :nth-of-type()
    Pega o elemento por tipo e posição. O tipo vem antes, e a posição entre parenteses. elementoPai elementoFilho:nth-of-type(posição-em-número)    

* :nht-child()
    Começa pela contagem dos filhos do Elemento pai. Somente se o elemento estiver como primeiro filho.

    ** :nth-child(odd) e :nth-child(even)
        even - números pares
        odd - números ímpares


## Ações do usuário

* :hover
    Vai mudar o link/elemento quando o usuário passar o mouse sobre ele


* :focus
   É aplicado quando o elemento recebe o foco da ação do usuário que pode ser feita utilizando o teclado ou clicando no elemento com o mouse. 
   
   É comumente usado em campos de input como uma forma de mostrar qual o input "ativo".

## Atributos:

* :disabled
    Vai mudar o link/elemento quando o usuário passar o mouse sobre ele


* :required
   É aplicado quando o elemento recebe o foco da ação do usuário que pode ser feita utilizando o teclado ou clicando no elemento com o mouse. 


# Referência

* * https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes 


  