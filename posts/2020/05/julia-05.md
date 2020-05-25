+++
title = "Condicionais e Recursão"
slug = "julia-05"
date = "2020-05-24 15:56:00 UTC-03:00"
tags = ""
category = ""
link = ""
description = ""
type = "text"
has_math=true
+++

## Capítulo 5

Neste capítulo introduzimos a execução condicional e recursão.

Principais assuntos:

 * Aritmética inteira: módulo e divisão inteira
 * Expressões booleanas
 * Operadores lógicos
 * `if`...`elseif`...`else`...`end
 * Recursão
 * Cuidado com a recursão

### Screecast da aula

 {{% media url=https://youtu.be/4aIgHnkURFY %}}


<!-- TEASER_END -->

### Problemas

**5.1** Como exercício, desenho o *stack diagram* (ver <https://benlauwens.github.io/ThinkJulia.jl/latest/book.html#stack_diagrams>) para `printn` chamado `s = "Hello"` e `n = 2`. Então escreva uma função chamada `do_n` (*fazer n*) que aceita como argumento uma função e um número e chama a função *n* vezes.

**5.2** A função `time` retorna a hora atual no meridiano de Greenwich em segunds desde uma origem, que é um ponto de referência no tempo arbitrário. Nos sistemas UNIX, a origem é primeiro de janeiro de 1970.

```julia
julia> time()
1.590347099099822e9

```

Escreva um script que lê a hora atual e converte em uma hora do dia em horas, minutos e segundos mais o número de dias desde a origem.


**5.3** O último teorema de Fermat diz que não existem inteiros *a*, *b* e *c*  tal que

\\[a^n + b^n = c^n\\]

para qualquer valor de *n* maior que 2.

 1. Escreva uma função chamada `checkfermat` que recebe 4 parâmetros - `a`, `b`, `c` e `n` e verifica se o teorema de Fermat é válido. Se `n` é maior que 2 e \\(a^n + b^n = c^n\\), o programa deve escrever: `"Caramba, Fermat estava errado!"`. Caso contrário, escrever `"Não, isso não dá certo."`
 2. Escreva uma função que pede do usuário os valores `a`, `b`, `c`  e `n`, converte para inteiro e usa `checkfermat` para verificar se eles violam o teorema de Fermat.

**5.4** Se você receb três paus, você pode ou não fazer um triângulo com eles. Por exemplo com um pau de 12 cm de comprimento e outros dois com 1 cm de comprimento, não é possível formar um triângulo. Dados três comprimentos, existe um teste simples para se verificar se é possível formar um triângulo:

> Se qualquer um dos comprimentos for maior que a soma dos outros dois então não se pode formar um
> triângulo. Caso contrário, é possível. Caso a soma de dois comprimentos seja exatamente igual ao
> terceiro, eles formam o que é chamado de triângulo "degenerado".

 1. Escreva uma função chamada `istriangle` que receb três inteiros como argumentos e escreve "Sim" ou "Não", dependendo na possibilidade de formar um triângulo ou não com os comprimentos.
 2. Escreva um função que recebe do usuário três comrimentos, converte para inteiro e usa a função `istriangle` para verificar se podem ou não formar um triângulo.

**5.5** Qual a saída do seguinte programa. Desenhe um *stack diagram* que mostra o estado do programa quando ele escreve o resultado.

```julia
function recurse(n, s)
    if n == 0
        println(s)
    else
        recurse(n-1, n+s)
    end
end

recurse(3, 0)
```

 * O que aconteceria se você chamasse esta função com: `recurse(-1, 0)`
 * Escreva um docstring que explica tudo o que uma pessoa precisa saber para usar esta função (e nada a mais).


**Os exercícios a seguir usam o pacote `ThinkJulia`, descrito no capítulo 4.

**5.6** Leia a função a seguir e veja se você consegue descobrir o que ela faz. Em seguida execute e veja se você acertou.

```julia
function draw(t, length, n)
    if n == 0
        return
    end
    angle = 50
    forward(t, length*n)
    turn(t, -angle)
    draw(t, length, n-1)
    turn(t, 2*angle)
    draw(t, length, n-1)
    turn(t, -angle)
    forward(t, -length*n)
end
```

**5.7** A curva de Kopch (<https://pt.wikipedia.org/wiki/Curva_de_Koch>) é um fractal. Para desenhar uma curva de Koch com comprimento *x*, você precisa:

 1. Desenhar a curva de Koch com comprimento \\(\frac{x}{3}\\).
 2. Virar a esquerda 60 graus.
 3. Desenhar a curva de Koch com comprimento \\(\frac{x}{3}\\).
 4. Virar para a direita 120 graus
 5. Desenhar a curva de Koch com comprimento \\(\frac{x}{3}\\).
 6. Virar a esquerda 60 graus.
 7. Desenhar a curva de Koch com comprimento \\(\frac{x}{3}\\).

A exceção é quando \\(x < 3\\): neste caso, você deve apenas desenhar uma linha reta com comprimento *x*.

 1. Escreva uma função `koch` que recebe uma tartaruga e um comprimento como parâmetros, e usa a tartaruga para desenhar a curva de Kock com o comprimento dado.
 2. Escreva a função chamada `snowflake` (floco de neve) que desenha três curvas de Koch para desenhar um floco de neve.
 3. A curva de Koch pode ser generalizada de diversas maneiras. Veja exemplos em <https://en.wikipedia.org/wiki/Koch_snowflake> e implemente a sua favorita.
 





### Links

 * Livro Think Julia: <https://benlauwens.github.io/ThinkJulia.jl/latest/book.html>
 * Instalação no windows <https://www.youtube.com/watch?v=IkegcEP3T_M>
 * Instalação no linux <https://www.youtube.com/watch?v=jDq6Iwdi82g>
ble/>
 
