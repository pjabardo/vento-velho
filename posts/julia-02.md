+++
title = "Variáveis, expressões e statements"
slug = "julia-02"
date = "2020-04-27 09:37:24 UTC-03:00"
tags = "julia, variáveis, expressões, statements, precedência de operadores"
category = ""
link = ""
description = ""
type = "text"
+++

Nesta segunda aula, estudamos o capítulo 2 do livro [Think Julia: How to Think Like a Computer Scientist](https://benlauwens.github.io/ThinkJulia.jl/latest/book.html#chap02).

Esta aula trata de conceitos básicos como variáveis, expressões e statements.


## Screencast da aula

{{% media url=https://youtu.be/Z8O7MRm1CDo %}}

## Exercícios

<!-- TEASER_END -->


### Exercício 2-1

Para checar a tua compreensão, digite os statements seguintes no terminal (REPL) Julia e veja o que eles fazem:

```julia
5
x = 5
x + 1
```

### Exercício 2-2
Reiterando o conselho do capítulo anterior, quando você aprende um novo recurso, você deveria testá-lo no modo interativo e errar de propósito para ver o que acontece.

 1. Sabemos que `n = 42` está correto. E `42 = n`?
 2. O que acontece com `x = y = 1`?
 3. Em algumas linguagens de programação (C/C++ por exemplo), todo statement termina com o ponto-e-vírgula, `;`. O que acontece se você coloca um ponto-e-vírgula ao final de um statement de Julia?
 4. E um ponto final `.` ao fim de um statement?
 5. Na notação usual de matemática, para multiplicar `x` e `y`, basta justapô-los: `x y`. O que acontece quando você faz isso em Julia? E quando você escreve `5x`?
 

### Exercício 2-1

Pratique usando Julia no terminal como uma calculadora:

 1. O volume de uma esfera com raio $r$ é $\frac{4}{3}\pi r^3$. Qual o volume de uma esfera com raio 5m?
 2. Suponha que o preço de capa de um livro seja R\$ 24,95 mas livrarias têm um desconto de 40%. O envio do livro custa R\$ 3 para o primeiro livro e 75 centavos para cada cópia adicional. Qual o custo total para a livraria de 60 cópias?
 3. Se eu saio de casa às 6:52 da manhã e corro 1 km a um ritmo leve (6 min por km), 5 km a um rítmo mais forte (5 min por km) e 1 km no rítmo leve, que horas eu chego em casa?
 