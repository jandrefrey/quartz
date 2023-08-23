---
title: "Probability"
---
The common misunderstanding of the LLN is that random processes are supposed to compensate for whatever happened in the past; this is just not true and is also called gambler’s fallacy (or law of averages).

**Sample space** is the collection of all possible outcomes of a trial.

## Disjoint events
Disjoint or mutually exclusive events($P(A)\cap P(B) = 0$) cannot both happen at the same time.
P(A or B or C) = P(A) + P(B) + P(C)

## Non-disjoint events
Events can occur simultaneously
P(A or B) = P(A) + P(B) - P(A and B)

## Probability Distribution
List of all possible disjoint outcomes and their probabilities.
- Outcomes must be disjoint
- Each probability must be between 0 and 1.
- The probabilities must total 1.

## Complimentary events
Mutually exclusive events whose probabilities that add up to 1.
Compliment: $P(A')$
$P(A) = 1-P(A')$

## Independence
Two processes are independent if knowing one provides no useful information in understanding the other. Multiplication rule:
- P(A and B) = P(A) x P(B)

If P(A occurs, given that B is true) = P(A | B) = P(A),  (knowing that B is true provides no info about A)
then A and B are independent.

## Probability trees
- If a probability is based on a single variable, it is a marginal probability. The probability of outcomes for two or more variables or processes is called a joint probability. The proportion of times the outcome would occur if we observed the random process an infinite number of times.
- Conditional probability: likelihood of an event or outcome occurring, based on the occurrence of a previous event or outcome. We generally separate the text inside our probability notation into the outcome of interest and the condition with a vertical bar


The conditional probability of outcome A given condition B is computed as the following:
$$P(A|B) = \frac{P(A and B)}{P(B)}$$

> **General multiplication rule**
> If A and B represent two outcomes or events, then:
> $P(AandB) = P(A|B)\times P(B)$
> It is useful to think of A as the outcome of interest and B as the condition.

### Bayes' Theorem:
Consider the following conditional probability for variable 1 and variable 2 :
$P$ (outcome $A_1$ of variable 1 | outcome $B$ of variable 2 )
Bayes' Theorem states that this conditional probability can be identified as the following fraction:
$$
\frac{P\left(B \mid A_1\right) P\left(A_1\right)}{P\left(B \mid A_1\right) P\left(A_1\right)+P\left(B \mid A_2\right) P\left(A_2\right)+\cdots+P\left(B \mid A_k\right) P\left(A_k\right)}
$$
where $A_2, A_3, \ldots$, and $A_k$ represent all other possible outcomes of the first variable.

1. First identify the marginal probabilities of each possible outcome of the first variable: $P\left(A_1\right)$, $P\left(A_2\right), \ldots, P\left(A_k\right)$.
2. Then identify the probability of the outcome $B$, conditioned on each possible scenario for the first variable: $\left.P\left(B \mid A_1\right)\right), P\left(B \mid A_2\right), \ldots, P\left(B \mid A_k\right)$.
3. Apply Formula.

## Continuous Distribution
![[Pasted image 20230221212825.png|350]]
Here the bins are so slim we find a smooth **continuous** line, presenting a probability density function (also called a density or distribution). The total area under the density's curve is 1.
The probability of a specific range of data can be taken as the area under that curve in the range.
