+++
title = "Funções"
slug = "julia-03"
date = "2020-04-27 10:45:07 UTC-03:00"
tags = ""
category = ""
link = ""
description = ""
type = "text"
+++


Nesta aula, estudamos o capítulo 3 do livro [Think Julia: How to Think Like a Computer Scientist](https://benlauwens.github.io/ThinkJulia.jl/latest/book.html#chap02).

Esta aula trata de um dos conceitos mais importantes em ciência da computação: funções.


## Screencast da aula

{{% media url=https://youtu.be/neJucNT4Dy0 %}}

## Exercícios

<!-- TEASER_END -->

### Exercício 3-1

Seja o programa

```julia
function printlyrics()
    println("I'm a lumberjack, and I'm okay.")
    println("I sleep all night and I work all day.")
end

function repeatlyrics()
    printlyrics()
    printlyrics()
end

repeatlyrics()

```

Mova a última linha deste programa para o começo do programa de modo que a chamada de função apareça antes de sua definição. Execute o programa e veja a mensagem de erro que aparece.

Agora, move a chamada de função para o fim do programa e coloque a definição de `printlyrics` após a definição de `repeatlyrics`. O que acontece quando você executa o programa?




### Exercício 3-2

Escreva uma função `rightjustify` (justifique pela direita) que recebe uma string como parâmetro e adiciona espaços à frente de modo que a última letra da string esteja na última coluna.

```julia
julia> rightjustify("lixo")
"                                                                  lixo"
```

Dica:
> Use concatenação de strings e repetição.
> Julia também possui uma função chamada `length` que
> retorna o comprimento de uma string, de modo que o valor
> de `length(monty)` é 5.

Modifique esta função de modo que ela receba um segundo argumento que especifica o número total de colunas (para trabalhar com valores diferentes de 70).



### Exercício 3-3

Um objeto de função é um valor que você pode atribuir a uma variável ou passar como argumento. Por exemplo, `dotwice` (fazer duas vezes) é uma função que recebe um objeto de  função como argumento e chama-o duas vezes:

```julia
function dotwice(f)
	 f()
	 f()
end
```

Aqui temos um exemplo que usa `dotwice` para chamar uma função chamada `printspam` duas vezes:

```julia
function printspam()
	 println("spam")
end

dotwice(printspam)
```


 1. Digite este exemplo em um script e teste.
 2. Modifique `dotwice` de modo que receba dois argumentos, um objeto de função e um valor e chama a função duas vezes, passando o valor como argumento.
 3. Copie a definição de `printtwice` definida no capítulo ao teu script.
 4. Use a versão modificada de `dotwice` para cahamar `printtwice` duas vezes, passando "spam" como argumento.
 5. Defina uma nova função chamada `dofour` (faça quatro) que recebe um objeto de função e um valor e chama a função 4 vezes, passando o argumento como parâmetro, Deveria haver apenas dois statements no corpo desta função, não quatro!


### Exercício 3-4

 1. Escreve uma função `printgrid` que desenha uma tabela como a seguir:

    ```julia
    julia> printgrid()
    + - - - - + - - - - +
    |         |         |
    |         |         |
    |         |         |
    |         |         |
    + - - - - + - - - - +
    |         |         |
    |         |         |
    |         |         |
    |         |         |
    + - - - - + - - - - +
    ```
    
 2. Escreva uma função que desenha uma tabela semelhante mas com 4 linhas e 4 colunas.

Dica:
> Para escrever mais de um valor numa linha, você pode usar uma sequência de valores separados por vírgula: `println("+", "-")`.
>
> A função `print` não avança para a próxima linha:
>
> `print("+ ")`
> 
> `println("-")`
>
> A saída de ambos statements é "+ -" na mesma linha. A saída do statement print seguinte é no começo da linha seguinte.



