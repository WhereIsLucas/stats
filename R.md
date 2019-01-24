# Fonctions de base pour R

* `x<-c(données)` pour encoder des données dans x
* `table(x)` modalités et effectifs
* `mean(x)` moyenne de x
* `sd(x)` écart type de x
* `var(x)` variance  de x
* `quantile(x)` donne les quantiles de x
* `IQR(x)` écart interquartile
* `prop.table(table(x))` frequences
* `cumsum(table(x))` eff cumulés
* `cumsum(prop.table(table(x)))` freq cumulés
* `cov(x,y)`
* `cor(x,y)`
* `lm(y ~ x)` // regr lin

# Graphes

* `plot(c(min(x)*.99,unique(sort(x)),max(x)*1.01),c(0,cumsum(prop.table(table(x))),1), xlab="", ylab="Frequences cumulees", main="Répartition empirique", type="s")` fonction de répartition empirique
* `plot(c(min(x)*.99,unique(sort(x)),max(x)*1.01),c(0,cumsum(prop.table(table(x))),1), xlab="", ylab="Frequences cumulees", main="Ogive", type="l")` ogive
* `hist(x,freq=FALSE)` diagramme en baton
* `plot(ecdf(x))` fonction de répartition
* `boxplot(x)` boite à moustache
* `plot(x,y)` scatter plot

