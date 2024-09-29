# Características da linguagem

## Código-fonte e escopo

O ambiente estatístico R foi criada pelos professores na década de 1990 para ensinar introdução à estatística na
Universidade de Auckland na Nova Zelándia.  Ele foi criado como versão em software livre do ambiente estatístico proprietário
denominado S-plus da empresa [TIBCO](https://www.tibco.com/). O ambiente S-plus utiliza uma linguagem de script denominada S,
sendo a linguagem R apenas um dialeto da linguagem S.  Por isso, poderemos nos referir à linguagem, indistintamente por 
S ou R, mas sempre usaremos o nome R quando nos referirmos ao ambiente onde ela é executada, pois apenas temos interesse no
ambiente R e não no ambiente S-plus. 

O código-fonte de´S deve ser escrito em arquivo de texto de sistema operacional e, como toda linguagem
de programação S opera sobre objetos armazenados na memória principal do computador e possui um léxico (conjunto de símbolos 
usados para designar objetos de memória e operações com estes objetos).  Sua sintaxe é, porém, desenhada especificamente
para a realização de cálculos estatísticos.  O dialeto R, por isso, optou por dar suporte prioritário ao paradigma de
programação funcional.  Isto significa que a maior parte dos objetos podem ser manipulados por meio de funções que operam
tal como funções matemáticas e, de modo geral, todo o código é composto por expressões ou funções matemáticas.
A forma como R implementa o paradigma funcional é diretamente inspirado pela linguagem [Scheme](https://www.scheme.org/).

Ainda assim, de fato, R é uma linguagem multiparadigma, permitindo escrever códigos sequenciais, estruturados, procedurais e
até mesmo orientado a objetos, muito embora, neste último caso, tenha-se nativamente um conceito de orientação a objetos
bastante heterodoxo.

Assim, sendo uma linguagem preferencialmente funcional, funções são particularmente importante em R, servindo para 
definir escopo de nomes de nomes para os objetos manipulados pela linguagem.  Assim, objetos definidos dentro do corpo de 
funções existem apenas enquanto a função onde ele foi definido está em memória (*escopo local*) ao passo que objetos definidos fora do corpo
de qualquer função existem durante toda a execução do programa (*escopo global*)

## Gestão de memória

A memória é gerenciada automaticamente pela implementação, não sendo necessário que o programador se preocupe com este tipo 
de questão.  Assim, a única limitação para se criar um objeto em memória é a disponibilidade de memória física para isto

## Implementações

Como dissemos, há duas implementações principais da linguagem S, quais sejam, o ambiente S-plus e o ambiente R.  Nosso foco
aqui é exclusivamente a implementação realizada pelo ambiente R, ainda que, por vezes, mencionemos a implementação realizada
pelo ambinete S-plus para fins de comparação.

Por isso, o padrão a que nos referimos é o proposto pelo R Core Team em 
[R languagem definition](https://cran.r-project.org/doc/manuals/r-release/R-lang.html)
.

## Estrutura do programa

O código-fonte R fica armazenado em arquivos de texto de sistema operacional com extensão .R.  Não há uma estrutrua prescrita,
posto que a linguagem, sendo multiparadigma, permite várias formas de escrever o código.  Ainda assim, refere-se aqui a boas
práticas de programação e, em particular, ao [Google R Style Guide](https://google.github.io/styleguide/Rguide.html).

Como o padrão de código do Google é um adendo ao padrão de uma das mais famosas bibliotecas de código R, referimo-nos, por
vezes, ao padrão do [Tidyverse style guide](https://style.tidyverse.org/)



