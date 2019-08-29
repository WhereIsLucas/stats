# Mathematica 

Coefficient binomial (C_n^m) : `Binomial[n, m]` 

Utiliser `Solve` est pratique



Fonction de porte est la fonction `Boole`

Probabilité x=0, distribution de poisson  `Probability[ x == 0 , x \[Distributed] PoissonDistribution[2.5]]`

Variance d'une distribution de poisson `Variance[PoissonDistribution[2.5]]`

Ecart-type ´`StandardDeviation[PoissonDistribution[2.5]]`

Espérance`Expectation[x, x \[Distributed] PoissonDistribution[2.5]]`

Réorganisons les données afin de pouvoir réaliser la régression linéaire 

`data = Table[{x[[i]], y[[i]]}, {i, 1, Length[x]}]`

Régréssion 

`LM = LinearModelFit[data, t, t]`

`LM[x] ` pour estimer

En vrac : 
```
Probability[]
PDF[]
CDF[]
Mean[]
Variance[]
PoissonDistribution[]
BinomialDistribution[]
NormalDistribution[]
ExponentialDistribution[]
Solve[]
```

# Statistique descriptive

Ecart inter quartil `InterquartileRange[distr]`

Quartiles `Quartiles[distr]`

Moyenne `Mean[]`


! Mathematica définit sa Distribution normale avec l'écart type, nous avec la variance! 

Pour avoir le symbole de distribution il faut encoder \[Distributed]

