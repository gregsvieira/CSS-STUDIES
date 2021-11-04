# Page Layouts


# Grid
* Posicionamento dos elementos dentro da caixa
* Posicionamento horizontal e vertical ao mesmo tempo
* Pode ser flexível ou fixo
* Cria espaços para os elementos filhos habitarem

O grid é aplicado ao body pois trabalha com o posicionamento dos filhos

define no body o formato do grid, sendo cada aspas uma linha:
grid-template-areas: ""
...
  grid-template-areas: 
  "header header"
  "main aside"
  "footer footer"
  ;

após definir o template do grid se vincula o css dos elementos ao posicionamento grid
ex: grid-area: header;

após isso se define o tamanho de cada linha no body:
grid-template-rows: primeira segunda e terceira;
grid-template-rows: 30px 1fr 40px;

após isso se define o tamanho de cada coluna no body:
#### ####

# GRID + FLEX
 * Podemos aplicar os dois conceitos em uma mesma página, mas não no mesmo elemento
 * Logo aplicamos grid em toda a página, iremos aplicar o flex no header
    pois no header só temos uma linha para trabalhar e não queremos fazer toda uma divisão como foi feito no layout inteiro.
   display:flex;