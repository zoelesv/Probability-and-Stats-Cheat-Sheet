# Probability and Stats Cheat Sheet

This section summary is a work in progress.

![YAP](https://media.giphy.com/media/B5a9bkLouElOM/giphy.gif)

## Contents

### Probability 
- [Probability basics](#Probability-basics)
- [Random Experiments and Outcome Space](#Random-Experiments-and-Outcome-Space)
- [Events and Properties of Probability](#Events-and-Properties-of-Probability)
- [Conditional Probability](#Conditional-Probability)
- [Independent events](#Independent-events)
- [Bayes's Theorem](#Bayes's-Theorem)

### Stats
- Coming soon

## Probability basics
| Name | Symbol | Description |
|------|--------|-------------|
| Sample space | S | a list of possible outcomes (make sure they are unique values) |
| A specific event | A, B, C,... | a subcollection of outcomes in S |
| Simple event | A, B, C,... | an event that contains one outcome that cannot be broken down any further |
| Compound event | S | an event that contains more than one outcome |
| Complementary event | A', Ac | an event that contains all outcomes not in the original event (A′ contains all outcomes not in A) |
| Union of 2 events (A or B)| A ∪ B | an event that contains all outcomes in A, B, or both (make sure not to double-count outcomes) |
| Intersection of 2 events (A and B) | A ∩ B | an event that contains only the outcomes in both A and B |
| The probability of A | P(A) | the chance of event A has occured: P(A) = number of outcomes in A / number of equally-likely outcomes in S |
| A belongs to B| A ∈ B ||
| Null set | ∅ | Empty set |
| Universal set | Ω, S | a set that contains all the elements or objects of other sets, including its own elements |
| Atom, singleton | ω, s | |
| Proper subset | ⊂ | A ⊂ B if set B contains at least one element that is not present in set B |
| Subset | ⊆ | A ⊆ B if all elements of A are also elements of B |

## Random Experiments and Outcome Space

* Probability theory considers experiements events for which outcomes are not certain, but stochastic 
* Know the different outcome space when flip a coin 3 times and flip 3 coins at once
* The random experiment is to roll a dice once S={1,2,..,6}
    
## Events and Properties of Probability

* Probability is a function for each event A: P(A) 
* The function P satisfies 3 axioms:
  
        1. P(A) ≥ 0  for any A ⊆ S
        2. P(S) = 1
        3. If A1, A2, A3 ... are a sequence of mutually exclusive events <br>(Ai ∩ Aj = ∅, ∀i≠j), then P(all events A)=sum(P(Ai))
* Theorem 1: The complement rule for any event A
  
        P(A) = 1 - P(A')
* Theorem 2: Probability of the empty set

        P(Ø)=0
* Theorem 3: Monotonicity
  
        if A ⊆ B, then P(A) ≤ P(B)
* Theorem 4: The numeric bound

        0 ≤ P(A) ≤ 1 , ∀A
* Theorem 5: Inclusion-Exclusion Principal
  
        P(A ∪ B)=P(A) + P(B) - P(A ∩ B)
* Theorem 6:
  
        P(A ∪ B ∪ C)=P(A) + P(B) + P(C) - P(A ∩ B) - P(A ∩ C) - P(B ∩ C) + P(A(A ∩ B ∩ C)
* Theorem 7: Equally Likely Theorem
  
        Let S be a discrete and finite sample space, i.e S= sum of n events then P(Si)=1/n

## Conditional Probability

* P(B|A) = “probability of B given A”
* P(B|A) = P(A ∩ B)/P(A)
* This formula gives the proportion of outcomes in A that are also in B
* Confusion of the inverse: P(B|A) ≠ P(A|B)
    
## Independent events

* Events are independent if the occurrence of one event does not affect the probability of occurrence for the other events.
* B is independent from A if P(B|A) = P(B)
* Multiplication rule for independent events: P(A and B) = P(A) x P(B)
* Sampling or without reolacement:
  1. Without replacement:
        Selectiion probabilities are not independent
  3. With replacement:
        Put the first selection back so it's available for the second selection
  4. 5% rule
        if your sample is less than 5%, you can approximate these events as independent
  
## Bayes's Theorem

* Bayes's Theorem --> Bayesian Inference
    to use the prior information  (P(cancer)) and posterior information (P(test|cancer)) to predict new observation's outcome. (P(cancer|test)new patient)
* Bayes's Theorem
    1. P(B|A) = P(B)P(A|B)/P(A)
       P(B|A) represents the probability of hypothesis B given evidence A
       P(A|B) denotes the probability of observing evidence A given the hypothesis B
       P(B) is the prior probability of hypothesis B
       P(A) represents the probability of observing evidence A

    2. P(Bk|A) = P(Bk).P(A|Bk)/P(A) = P(Bk).P(A|Bk)/ Sum of P(A ∩ Bi) = P(Bk)P(A|Bk)/Sum of P(Bi)P(A|Bi)
  
