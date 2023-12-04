+++
title = "Modelos, escalas e semelhança"
slug = "modelos-escalas-e-semelhanca"
date = "2023-11-21 15:02:10 UTC-03:00"
tags = "modelos,escalas,semelhança,análise dimensional,teorema de Buckingham"
category = ""
link = ""
description = ""
type = "text"
+++


# Análise dimensional

Análise dimensional sempre me facinou. A primeira vez que eu vi, tinha hora que parecia matemágica. Aí você começa a entrar mais a fundo e percebe que é mais trivial e menos poderoso do que parece. No final, a aplicação mais comum é _semelhança_: como fazer ensaios em modelos reduzidos. Mas essa é uma visão muito pobre, e na verdade a análise dimensional está diretamente relacionado aos modelos que estamos usando e qual a régua que usamos para caracterizar um problema físico. 

Fundamentalmente, não podemos pensar sobre um problema sem fazer a análise dimensional. O objetivo deste cursinho é tentar abordar o assunto a partir de diferentes pontos de vista, queremos ir além da obtenção de parâmetros adimensionais e semelhança

# Estrutura do curso

Começamos discutindo o que são modelos e suas escalas. Usamos as equações diferenciais de alguns problemas simples para fazer isso.

Na segunda aula, apresentamos a análise dimensional, ou melhor, o que consta no capítulo de qualquer livro didático de análise dimensional.

Finalmente, na terceira aula mostramos algumas aplicações e alguns paradoxos.

# Referências e notas de aula

 * [Notas de aula da primeira aula](../modelos/01-modelos.pdf)
 * [Artigo/livreto que estou escrevendo](../modelos/modelos.pdf) está cheio de errinhos e inconsistências mas o jeitão está lá. Está no [repositório github](https://github.com/pjabardo/livro-modelos).
 * [Barenblatt, "Scaling"](https://www.cambridge.org/core/books/scaling/E08325F4C8A14AAD4742E39FE5D0A6B3) Este livrinho é uma obra de arte. Na verdade, quaisquer dos livros do Barenblatt são brilhantes. 
 * [Barenblatt, "Scaling, Self-similarity and Intermediate Asymptotics"](https://www.cambridge.org/core/books/scaling-selfsimilarity-and-intermediate-asymptotics/3B56096C3B7E822794C81B51F7370B82) parecido com o Scaling mas aprofunda um pouco mais.
 * [Lemons, Don S. "A Student's Guide to Dimensional Analysis"](https://www.cambridge.org/core/books/a-students-guide-to-dimensional-analysis/2CD61E4BF2A72CF58A26AE8E882F7BB5). Livrinho moderno e muito fácil de ler com aplicações em diversas áreas.
 * Bridgman, P. W. "Dimensional Analysis", 1931. Livro antigo e um verdadeiro clássico. Continua sendo um dos melhores livros da área.
 * Langhaar, Henry L. "Dimensional Analysis and Theory of Modelos", 1951. Outro clássico. Muito bom e completo. Curiosamente, meu pai era amigo do autor e comprou dele diretamente.
 * [Snyder, "Guideline for Fluid Modeling of Atmospheric Diffusion", 1981, relatória da EPA EPA-600/8-81-009](https://nepis.epa.gov/Exe/ZyNET.exe/2000BDW8.TXT?ZyActionD=ZyDocument&Client=EPA&Index=1981+Thru+1985&Docs=&Query=&Time=&EndTime=&SearchMethod=1&TocRestrict=n&Toc=&TocEntry=&QField=&QFieldYear=&QFieldMonth=&QFieldDay=&IntQFieldOp=0&ExtQFieldOp=0&XmlQuery=&File=D%3A%5Czyfiles%5CIndex%20Data%5C81thru85%5CTxt%5C00000000%5C2000BDW8.txt&User=ANONYMOUS&Password=anonymous&SortMethod=h%7C-&MaximumDocuments=1&FuzzyDegree=0&ImageQuality=r75g8/r75g8/x150y150g16/i425&Display=hpfr&DefSeekPage=x&SearchBack=ZyActionL&Back=ZyActionS&BackDesc=Results%20page&MaximumPages=1&ZyEntry=1&SeekPage=x&ZyPURL). Um verdadeiro tratado sobre difusão na atmosfera.
 * Sedov, L. I., "Similarity and dimensional methods in mechanics". Último da lista mas provavelmente o melhor. Fácil de encontrar digitalmente. Em sebos ainda é possível encontrar no Brasil em Francês.
 

# Aula 01

## Slides da aula

* [Notas de aula da primeira aula](../modelos/01-modelos.pdf)

## Vídeos

 * {{% media url=https://www.youtube.com/watch?v=KDp1tiUsZw8 %}}
 * {{% media url=https://www.youtube.com/watch?v=E43-CfukEgs %}}
 * {{% media url=https://www.youtube.com/watch?v=h_zytOcMwys %}}
 
# Aula 02 - Análise dimensional

 * [Slides da aula 02](../modelos/02-adim.pdf)
 * [Solução de Blasius para a camada limite](../modelos/02b-camada-limite.pdf)

# Aula 03 - Exemplos e aplicações

## Slides usados na aula

 * [Slides da aula 03, parte 1](../modelos/03-exemplos.pdf)
 * [Slides da aula 03, parte 2 - Ensaios em túnel de vento](../modelos/03b-tuneldevento.pdf)

## Artigos referidos
 
   - [Rayleigh, The principle of similutude, 1915](../modelos/rayleigh1915.pdf)
   - [Comentários de Riabouchinsky, sobre The principle of similitude de Rayleigh, 1915](../modelos/riabouchinsky1915.pdf)
   - [Resposta de Rayleigh sobre os comentários de Riabouchinsky, 1915](../modelos/riabouchinsky1915.pdf)
   - [McMahon, Thomas A., "Rowing: A similarity Analysis", Science, pp 349-351, vol 173, Julho de 1971](../modelos/mcmahon1971.pdf)
   


## Notebooks usados
 
* [Notebook Jupyter com código Python usando o pacote `BuckinghamPi`](../modelos/exemplos)
* [Arquivo .ipynb do notebook](../modelos/exemplos.ipynb)
* [Notebook Pluto (Julia) que implementa o método de semelhança por coeficiente de arrasto](../modelos/cdsim/index.src.html)
* [Arquivo fonte do notebook Pluto (Julia) que implementa o método de semelhança por coeficiente de arrasto](../modelos/cdsim.jl)


Para instalar o Pluto, devemos [instalar Julia](https://julialang.org) e em seguida instalar o pacote Pluto:

```
[pjabardo@durruti vento]$ julia
               _
   _       _ _(_)_     |  Documentation: https://docs.julialang.org
  (_)     | (_) (_)    |
   _ _   _| |_  __ _   |  Type "?" for help, "]?" for Pkg help.
  | | | | | | |/ _` |  |
  | | |_| | | | (_| |  |  Version 1.9.3 (2023-08-24)
 _/ |\__'_|_|_|\__'_|  |  Official https://julialang.org/ release
|__/                   |

julia> import Pkg

julia> Pkg.add("Pluto")
```

Para usar o notebook, vá na pasta onde está o o arquivo `cdsim.jl`, execute o programa Julia, carregue o pacote `Pluto` e execute:

```
[pjabardo@durruti notebooks]$ ls
cdsim.jl  exemplos.ipynb
[pjabardo@durruti notebooks]$ julia
               _
   _       _ _(_)_     |  Documentation: https://docs.julialang.org
  (_)     | (_) (_)    |
   _ _   _| |_  __ _   |  Type "?" for help, "]?" for Pkg help.
  | | | | | | |/ _` |  |
  | | |_| | | | (_| |  |  Version 1.9.3 (2023-08-24)
 _/ |\__'_|_|_|\__'_|  |  Official https://julialang.org/ release
|__/                   |

julia> import Pluto; Pluto.run()
```

Vá onde está Opena notebook e clique dentro do quadro. `cdsim.jl` deve aparecer.

   
  


