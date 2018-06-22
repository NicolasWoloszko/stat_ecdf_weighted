# stat_ecdf_weighted
Weigted version of ggplot2 empirical cumulative distribution function (ECDF) 

The current version of stat_ecdf in ggplot2 does not include observation weights. I simply replace the ecdf statistic within the code of ggplot2::stat_ecdf in order to make it possible to use weighted samples. The function works exactly as any other ggplot2 object. Here is an example : 
```
ggplot(d, 
       aes(x,  weight = w)) + 
  stat_ecdf()
```
