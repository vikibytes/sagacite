# Conditioning and Bayes Rule

## Introduction
- ### Conditioning
    - Revising a model based on new information
    - Enables us to divide and conquer probabilistic problems

- ### Independence
    - describes a situation where the occurence or non-occurence of events is determined by completely unrelated factors.

    - allows us to build complex models out of simple ones.

## Conditional Probability

- Assume two events non-disjoint A & B of a Sample Set S. Now if we know B has occured, what is the probability that A also has occured ?

- It is easy : since we know B occured with a non-zero probability (P__b), and the intersection between A and B is also known (P__aub), then intutively, A must occur with a probability of P__aub / P__b.
![Conditional Probability](images/conditional_prob.png) 

- Conditional Probabilities behave the same as that of ordinary probabilities. All the Probability Axioms apply to Conditional Probabilities as well.
    - Axiom 1: For any event A, P(A|B)≥0
    - Axiom 2: Conditional probability of B
given B is 1, i.e., P(B|B)=1
    - Axiom 3: If A1,A2,A3,⋯
are disjoint events, then P(A1 ∪ A2 ∪ A3⋯|B)=P(A1|B)+P(A2|B)+P(A3|B)+⋯.

- ELI5: The probability of an event (B) happening given that an event (A) has occured is the probability of both the events occuring P(B ∩ A) divided by the probability of the conditioning event. P(A)

### Multiplication Rule
P(A ∩ B) = P(A|B) * P(B)
         = P(B|A) * P(A)

### Total Probability Theorem
-  if you want to find P(A), you can look at a partition of S, and add the amount of probability of A that falls in each partition.

- for any two events A and B, we can write 
    - P(A) = P(A|B) P(B) + P(A|B') P(B').

- can be simplified as  ∑i P(A|Bi) P(Bi), where i is the partition.

### Bayes Rule
- Suppose that we know P(A|B), but we are interested in the probability P(B|A). Using the definition of conditional probability, we have<br/>
P(A|B) P(B) = P(A ∩ B) = P(B|A) P(A).

Dividing the left and right formulas by P(A), we obtain <br/>
P(B|A) = P(A|B) P(B) / P(A),
which is the famous Bayes' rule. 

Often, in order to find P(A) in Bayes' formula we need to use the law of total probability, so sometimes Bayes' rule is stated as<br/>
P(Bj|A) = P(A|Bj) P(Bj)/ ∑iP(A|Bi)P(Bi),<br/>
where B1,B2,⋯,Bn form a partition of the sample space.

- Note that in the Bayes Rule formula, the numerator is what we calculate using the Multiplication Rule and the denominator is what we calculate using the Total Probability Theorem