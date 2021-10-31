_page 185_
#### Discrete Probability
- marginal probability: $X$ takes the value $x$ irrespective to the value of random variable $Y$; respect to the total number--> written as $p(x)$ 
- conditional probability: $X=x$ and the fraction of instances $Y=y$ --> written as $p(x|y)$

_example 6.2_
_Marginal Probability_
$$P(X=x_{i})=\frac{c_{i}}{N}=\frac{\sum_{j=1}^{3}n_{ij}}{N}$$
and
$$P(Y=y_{j})=\frac{r_{j}}{N}=\frac{\sum_{i=1}^{5}n_{ij}}{N}$$
- state $X=x_{i}$ and $Y=y_{j}$
- number of events from the states: $n_{ij}$
- total number of events $N$
- $c_{i}$ and $r_{j}$ are the sum of $i$th column and $j$th row of the probability table 

_Conditional Probability_
ex: probability of $Y$ given $X$
$$P(Y=y_{j}|X=x_{i})=\frac{n_{ij}}{c_{i}}$$


*put picture of the probability table here*

_Use in machine learning_: model categorical variables => variables that take a finite set of unordered values

_[[code example]]_

