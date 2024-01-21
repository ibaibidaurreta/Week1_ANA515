# Week1_ANA515
Week 1 Activity: R Markdown
> library(ggplot2)
> library(dplyr)
> diamonds<- as.data.frame(diamonds)
> head(diamonds, 3)
  carat     cut color clarity depth table price    x    y    z
1  0.23   Ideal     E     SI2  61.5    55   326 3.95 3.98 2.43
2  0.21 Premium     E     SI1  59.8    61   326 3.89 3.84 2.31
3  0.23    Good     E     VS1  56.9    65   327 4.05 4.07 2.31
> {r Datam in
> small<-diamonds %>%
+ filter(carat<=2.2)
> small %>%
+ ggplot(aes(carat))+
+ geom_freqpoly(binwidth=0.01)

