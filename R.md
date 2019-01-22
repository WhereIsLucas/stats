# Fonctions de base pour R

* `mean(x)` moyenne
* `sd(x)` écart type
* `var(x)` variance 
* `quantile(x)`
* `IQR(x)` écart interquartile
* `table(x)` effectifs
* `prop.table(eff)` frequences
* `cumsum(eff)` eff cumulés
* `cumsum(freq)` freq cumulés
* `boxplot(x)`
* `cov(x,y)`
* `cor(x,y)`
* `lm(y ~ x)` // regr lin

# Graphes

* `plot(c(min(x)*.99,unique(sort(x)),max(x)*1.01),c(0,cumsum(prop.table(table(x))),1), xlab="", ylab="Frequences cumulees", main="Répartition empirique", type="s")`
* `plot(c(min(x)*.99,unique(sort(x)),max(x)*1.01),c(0,cumsum(prop.table(table(x))),1), xlab="", ylab="Frequences cumulees", main="Ogive", type="l")`
* `hist(x,breaks=seq(1.5,8.5,by=1), freq=FALSE)`
* `plot(ecdf(x), xlab="Température", ylab="Freq")`
