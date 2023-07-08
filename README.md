# Probability and Stats Cheat Sheet

This section summary is a work in progress.

![YAP](https://media.giphy.com/media/B5a9bkLouElOM/giphy.gif)

## Contents

### Probability 
- [Probability basics](#Probability-basics)
- [Random Experiments and Outcome Space](#Random-Experiments-and-Outcome-Space)
- [Events and Properties of Probability](#Events-and-Properties-of-Probability)
- [Conditional Probability](#Conditional-Probability)

### Stats
- Coming soon

## Probability basics
| Name | Symbol | Description |
|------|--------|-------------|
| Sample space | S | a list of possible outcomes (make sure they are unique values) |
| A specific event | (A, B, C,...) | a subcollection of outcomes in S |
| Simple event | A capital letter (A, B, C,...) | an event that contains one outcome that cannot be broken down any further |
| Compound event | S | an event that contains more than one outcome |
| Complementary event | A′ | an event that contains all outcomes not in the original event (A′ contains all outcomes not in A) |
| Union of 2 events (A or B)| A ∪ B | an event that contains all outcomes in A, B, or both (make sure not to double-count outcomes) |
| Intersection of 2 events (A and B) | A ∩ B | an event that contains only the outcomes in both A and B |
| The probability of A | P(A) | the chance of event A has occured: P(A) = number of outcomes in A / number of equally-likely outcomes in S |

## Random Experiments and Outcome Space
    - Probability theory considers experiements events for which outcomes are not certain, but stochastic 
    - Know the different outcome space when flip a coin 3 times and flip 3 coins at once
    - The random experiment is to roll a dice once S={1,2,..,6}
    
## Events and Properties of Probability
    - Probability is a function for each event A: P(A) 
    - The function P satisfies:
        1. P(A) >= 0 for any A <= S
        2. P(S) = 1
        3. If A1, A2, A3 ... are a sequence of mutually exclusive events, then P(all events A)=sum(P(Ai))
    - Theorem 1: For any event A,
        P(A) = 1 - P(A')
    - Theorem 2: 
        P(Ø)=0
    - Theorem 3: if A <= B, then
        P(A) <= P(B)
    - Theorem 4: for all A, P(A) <= 1
    - Theorem 5: P(A ∪ B)=P(A) + P(B) - P(A ∩ B)
    - Theorem 6: P(A ∪ B ∪ C)=P(A) + P(B) + P(C) - P(A ∩ B) - P(A ∩ C) - P(B ∩ C) + P(A(A ∩ B ∩ C)
    - Theorem 7: Let S be a discrete and finite sample space, i.e S= sum of n events then P(Si)=1/n

## Conditional Probability
    - P(B|A) = “probability of B given A”
    - P(B|A) = P(A ∩ B)/P(A)
    - This formula gives the proportion of outcomes in A that are also in B
    - Confusion of the inverse: P(B|A) ≠ P(A|B)
    
        
