# Hw4- Lab#2


1.
There is 1852 chocolate bars that are rated.

2.
library(tidyverse)
ggplot(data = choco, aes(x=Review.Date,fill=factor(Rating)))+
  geom_bar()
  
 The bar chart shows that the year 2015 has the most ratings.It also shows that the number of ratings increases until 2015 then decreases.  
 
question we want to investigate: which years did the US has the highest ratings for car brands?

U.S.A <- choco %>% filter(Company.Location == "U.S.A.")
head(U.S.A)
library(tidyverse)

U.S.A %>%
  ggplot( aes(x = Review.Date, fill=factor(Rating)))+
  geom_bar()
  
  The US also has the highest ratings at 2015, as you can see in the graph it is similar to the graph with all of the locations. The ratings total increases until 2015 then decreases again. 
  
1.
library(tidyverse)
ggplot(data = choco, aes(x=Review.Date,fill=factor(Rating)))+
  geom_histogram()
 
 The amount of ratings is distributed throughout the years by what looks like a distribution model almost.

2.
library(tidyverse)
ggplot(data = choco, aes(x= Cocoa.Pct,fill=factor(Rating)))+
  geom_bar()
  
  yes the ratings depend on the percentage. Most of the ratings are near the 50% mark.
  
 3.
 library(tidyverse)
 ggplot(data= choco, aes(x=Company.Location, fill=factor(Rating)))+
  geom_bar()
  
  The U.S. has by far the most amount of ratings compared to canada and France.
  
  
