+++
title = "Computação Científica com Julia"
slug = "scicomp"
date = "2020-04-04 17:26:00 UTC-03:00"
tags = "julia, computação científica"
category = ""
link = ""
description = ""
type = "text"
has_math = true
nocomments = false
+++

# Introdução

Esta página tem o material referente ao curso _Computação Científica com Julia_. Este curso tem por objetivo usar uma abordagem construtiva e prática para programação em Julia de métodos numéricos.

Nestes dias de quarentena e corona virus, o curso não pode ser presencial. Assim está aberto a todos que que desejarem. Para tirar dúvidas, estarei disponível segundas, quartas e sextas das 9:00 às 10:00 em <https://meet.jit.si/iptscicomp>. Do computador, só é necessário o browser. Em telefones e tablets é necessário instalar um app.

# Estrutura do curso

O curso será dado usando screencasts no youtube. Os vídeos podem ser encontrados no canal do youtube <https://www.youtube.com/channel/UCxsN52VZT5QZKDU66lx4XXQ>. Cada aula terá exercícios propostos e a solução dos exercícios será dada, nesta página ao final de uma semana.

A idéia do curso é construir, a partir de elementos básicos como

 * Interpolação
 * Derivadas numéricas
 * Integração
 * Solução de sistemas lineares

um solver de elementos finitos de alta ordem. Se possível, vamos tentar resolver as equações de Navier-Stokes. Vamos ver onde conseguimos ir.

Os interessados já ficam avisados que simplesmente assistir uns vídeos e fazer perguntinhas nas conversas só têm  um resultado: perda de tempo. Este curso pressupõe participação ativa e programação contínua. Se não estiver disposto, nem comece.

Pessoas sábias já disseram que o melhor software é aquele que não precisamos escrever. Neste espírito, acho interessante a cada voluntário escolher algum problema de interesse pessoal e algum software, de preferência livre, e tentar, em paralelo a este curso resolver este problema. Abaixo existem links para diferentes softwares na net.

Paralelo a esse curso, vou também dar um curso mais aprofundado de programação em Julia. A idéia é estudar o manual <https://docs.julialang.org/en/v1/>. Maiores detalhes, ir para a [página do curso de programação em Julia](../julia).

# Preparando o ambiente de programação

Fiz um screecast para instalação do Julia no linux e outro no windows

## Instalação no Linux

 {{% media url=https://www.youtube.com/watch?v=jDq6Iwdi82g %}}


## Instalação no Windows

 {{% media url=https://www.youtube.com/watch?v=IkegcEP3T_M&t=5s %}}

-------
# Aulas

## Introdução à programação em Julia

[Aqui você encontra os links para os screencasts da introdução à programação em Julia](../posts/intro-to-julia).

## Apresentação do curso

# Screencast da aula:

{{% media url=https://www.youtube.com/watch?v=jCxVumCf9CE %}}

# Notebooks

 * [Apresentação do Curso](../sci-comp/apresentacao)
 * [Idéia básica da abordagem do curso](../sci-comp/000-ideia-basica)

## Aula 01: Interpolação e aproximação

[Notebook com as notas de aula sobre interpolação e aproximação](../sci-comp/01-aproximacao)


# Bibliografia

 * [Burden e Faires, Análise Numérica](https://www.amazon.com.br/An%C3%A1lise-num%C3%A9rica-Richard-Burden/dp/8522123403/ref=sr_1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=Burden+Faires&qid=1553869210&s=gateway&sr=8-1-spell)
 * [Karniadakis e Kirby, Parallel Scientific Computing in C++ and MPI](https://www.amazon.com.br/Parallel-Scientific-Computing-MPI-Implementation-ebook/dp/B00FF76QD8/ref=sr_1_fkmrnull_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=Karniadakis+Parallel+Scientific&qid=1553869244&s=gateway&sr=8-1-fkmrnull)
 * [Golub e Van Loan, Matrix Computations](https://www.amazon.com.br/Computations-Hopkins-Studies-Mathematical-Sciences-ebook/dp/B00BD2DVIC/ref=sr_1_fkmr1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=Golub+Van+Load&qid=1553869321&s=gateway&sr=8-1-fkmr1)
 * Recomendação do Gabriel: [Gilbert Strang, Computational Science and Engineering](https://www.amazon.com.br/Computational-Science-Engineering-Gilbert-Strang/dp/0961408812/ref=sr_1_fkmrnull_5?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=Computational+Science+and+Engineering+strang&qid=1553869616&s=gateway&sr=8-5-fkmrnull)

-------





------
 
# Links importantes

Há uma organização do github com os softwares e slides do curso: <https://github.com/iptscicomp>

 * <http://julialang.org>
 * Lista de discussão <https://discourse.julialang.org/>
 * Canal do youtube <https://www.youtube.com/user/JuliaLanguage>
 * Documentação: <https://docs.julialang.org>
 * Junolab, um ambiente baseado no editor [Atom](https://atom.io) para programação em Julia: <https://junolab.org/>
 * GitHub do julia: <https://github.com/JuliaLang>
 * Para chat, existe o Slack Julia oficial: <https://julialang.slack.com/>
 * <http://gen.lib.rus.ec/>
 * <http://sci-hub.tw/>
 
# Trabalho

 Durante o transcorrer do curso, use algum software para resolver um problema concreto:
 
 * [OpenFoam](https://www.openfoam.com/) - CFD
 * [SU2](https://su2code.github.io/) - CFD
 * [CalculiX](http://www.calculix.de/) - Elementos Finitos
 * [Code Saturne](https://www.code-saturne.org/) - CFD
 * [Code Aster](https://www.code-aster.org/) - Elementos Finitos
 * [Fenics](https://fenicsproject.org/) - Elementos Finitos
 * [FreeFem++](https://freefem.org/) - Elementos Finitos
 * [Dedalus Project](http://dedalus-project.org/) - Métodos espectrais
 * [Nektar](https://www.nektar.info/) - Método de elementos espectrais/elementos finitos _hp_
 * [MEEP](https://meep.readthedocs.io/en/latest/) - Eletromagnetismo
 * [LAMMPS](https://lammps.sandia.gov/) - Dinâmica molecular
 

# Editores e ferramentas importantes

 * [Projeto Jupyter](https://jupyter.org/) - principal ambiente de trabalho
 * [Atom](http://atom.io) e [Junolab](http://junolab.org)
 * [Visual Studio Code](https://code.visualstudio.com/)
 * [Emacs - para quem for valente...](https://www.gnu.org/software/emacs/)
 * [Distribuição de Python Anaconda](https://www.anaconda.com/distribution/) - Muito prático no Windows. Já vem com o Jupyter.
 * [Julia Box - use Julia a partir do Browser na web](https://juliabox.com/)
 
