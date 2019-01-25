# Stats

## R et Mathematica

[Mathematica](https://whereislucas.github.io/stats/mathematica)

[R](https://whereislucas.github.io/stats/R)

## Formulaire et autres trucs

### Stat descriptive

mode = modalité à l'effectif maximum

### Espérance, moments, variance et écart-type 

![](http://mathurl.com/yaubmbgt.png)

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/c51e95b59c11e3e53d3b32a95b252d2dbe743c73)

![](http://mathurl.com/yapm3l3d.png)

![](http://mathurl.com/y77p524f.png)

### Fonction de densité et de répartition

l'intégrale de fonction de densité de proba = 1 -> notée f(x)
donc si on doit calculer k pour que ce soit une densité de proba, il faut normaliser la fonction

`Solve[Integrate[k*fonction, {x, -Infinity, Infinity}] == 1]` dans mathematica


la fonction de répartition est l'intégrale de - inf à t de la fonction f(x) -> notée F(t) (elle équivaut à P(X ≤ t))
`Integrate[fonction(t),{t,-Infinity,x}]` 

### Distribution jointe

Pour calculer les marginales, il suffit de sommer les différentes probas
Pour calculer les E[Y | X = x], reprendre dans le grand tableau

distribution marginale de la distribution jointe : 

<img src="https://latex.codecogs.com/gif.latex?f^X&space;(x&space;=&space;)\int_{-\infty}^{\infty}&space;f(x,y)&space;dx" title="f^X (x = )\int_{-\infty}^{\infty} f(x,y) dx" /> 

distribution conditionnelle

<img src="https://latex.codecogs.com/gif.latex?f^{Y|X=x}&space;(y)=&space;\frac{f(x,y)}{f^X(x)}" title="f^{Y|X=x} (y)= \frac{f(x,y)}{f^X(x)}" /> 

Probabilité conditionnelle 

<img src="https://latex.codecogs.com/gif.latex?P(a<=Y<=b|X=x)=\int_a^b&space;f^{Y|[X=x]}(y)dy" title="P(a<=Y<=b|X=x)=\int_a^b f^{Y|[X=x]}(y)dy" />

X et Y sont indépendantes si f (x, y) = fX (x)* fY (y)



