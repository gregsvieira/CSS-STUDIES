# Combinators
Combinadores, pois eles trabalham para buscar e combinar seletores a fim de aplicar uma estilização

##  Tipos:

# Descendant combinator

* Identificado por um espaço entre os seletores
* Busca um elemento dentro de outro, mesmo que existam outros elementos no caminho
* Se existir outros elementos iguais serão aplicados também
* Ele encontra mesmo que ajam outros elementos dentro do caminho

# Child combinator

* Identificado pelo sinal > entre dois seletores
* seleciona somente o elemento que é filho direto do pai
* Elementos depois do filho direto serão desconsiderados

# Adjacent Sibling Combinator

* Identificado pelo sinal + entre dois seletores
* Seleciona somente o elemento do lado direito que é irmão direto na hierarquia
* Exemplo do botão, selecionamos o botão direito e no css acrescentamos ao lado esquerdo dele um espaçamento

# General sibling combinator

* Irmão combinado de maneira geral
* Identificado pelo sinal ~ entre dois seletores
* Seleciona todos os elementos irmãos


# Utilizando combinators #
* Dica:
Seletores muito específicos tendem a causar dificuldades no reuso das regras de estilização. 
Ex: ul > li[class="red"] {
	color: red;
}

Muitas vezes, um simples uso de classes, torna o trabalho mais eficiente e podemos reaproveitar no futuro. Simplificando, ex: 
.red {
    color: red;
    }