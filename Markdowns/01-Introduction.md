# Introduction

## Proof
```ad-info
Proof is method of obtaining / ascertaining a truth.
```
```ad-example
1. Experimentation
2. Observation
3. Sampling & Counter examples
4. Judge & Juries
5. Religion (Word of God)
6. Word of Boss
```


```ad-important
In mathematics, a mathematical proof is a verification of a __proposition__ by a chain of __logical deductions__ from a set of __axioms__.
```

## Proposition
```ad-important
A **proposition** is statement which is **either true or false**. 
- For this proposition to be to, the predicate has to come true.  
```
```ad-example
$$\forall  n \in N, \ n^2 + n + 41 \ is \ the \ prime \ numbers$$   is called the predicate (depends on the value of variable).
```ad-note
title: Solution
- for the 1 to 39 -> true
- but, 40 and 41 -> false
```ad-failure
```
````ad-example
$$a^4 + b^4+c^4+d^4 \ has \ no \ positive \ solutions$$
```ad-note
title: Solution
- But for some 6 digit value, this proposition becomes false, and there exists a solution.
- $$ \exists \  a^4 + b^4+c^4+d^4 \ has \ no \ positive \ solutions$$
- But for some exists propositions, of which finding the shortest smallest counter example of > 1000 digits. 
```ad-failure
```
- factoring of 1000 digits is useful Crypto-systems works.
````
#### Not
```ad-important
|  p  | $\neg$ p |
|:---:|:------:|
|  T  |   F    |
|  F  |   T    |
```
#### And
```ad-important
|  p  |  q  | p $\land$ q |
|:---:|:---:|:-------:|
|  T  |  T  |    T    |
|  T  |  F  |    F    |
|  F  |  T  |    F    |
|  F  |  F  |    F    | 
```
#### Or
```ad-important
|  p  |  q  | p$\lor$q |
|:---:|:---:|:------:|
|  T  |  T  |   T    |
|  T  |  F  |   T    | 
|  F  |  T  |   T    |
|  F  |  F  |   F    |
```
#### Exclusive Or (xor)
```ad-important
|  p  |  q  | p $\oplus$ q |
|:---:|:---:|:------:|
|  T  |  T  |   F    |
|  T  |  F  |   T    | 
|  F  |  T  |   T    |
|  F  |  F  |   F    |
```
#### Implies
```ad-important
An Implication $p \Rightarrow \ q$  is true, when p is false or q is true.

|  p  |  q  | p $\Rightarrow$ q | q $\Rightarrow$ p | p $\iff$ q |
|:---:|:---:|:-----------------:|:-----------------:|:----------:|
|  T  |  T  |         T         |         T         |     T      |
|  T  |  F  |         F         |         T         |     F      |
|  F  |  T  |         T         |         F         |     F      |
|  F  |  F  |         T         |         T         |     T      |
```
```ad-example
"If pigs fly, I would be king" is true.
```
#### if and only if (iff)
```ad-important
- either both true or both false

|  p  |  q  | p $\iff$ q |
|:---:|:---:|:-------:|
|  T  |  T  |    T    |
|  T  |  F  |    F    |
|  F  |  T  |    F    |
|  F  |  F  |    T    |

```ad-example
$$x^2-4\geq0 \iff |x|\geq2$$
```

## Conjecture
```ad-important
Conjecture is an opinion or conclusion formed on the basis of incomplete information.
```
## Axiom
```ad-important
  An **axiom** is a **proposition that is assumed to be true.**
```
```ad-example
- In Euclidean Geometry, Given a line L and a point P not on line L, there is exactly one line through P || L.
- In Euclidean Geometry, Given a line L and a point P not on line L, there is no line through P || L.
- In Hyperbolic Geometry, Given a line L and a point P not on line L, there is infinite lines through P || L.
```
```ad-attention
- Axioms should be consistent and complete
- A set of Axioms is said to be **consistent if no proposition can be proved to be both true and false**.
- A set of Axioms are said to be **complete if it can be used to prove every proposition is either true or false**.
```
```ad-tip
title: Notations
- $\forall$  (for all)
- $\exists$  (ther exists)
- $\in$  (belongs to)
```