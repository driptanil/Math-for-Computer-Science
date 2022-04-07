### Proof by Contradiction
```ad-important
To prove P is true, we assume P is false (i.e. $\neg$ P is true), then using that hypothesis to derive a false hood or contradiction.
- If $\neg$ P $\Rightarrow$ F is true, $\therefore$  P is true
``` 

```ad-example
Proof $\sqrt{2}$  is irrational.
```ad-note
title: Solution
- Proof by contradiction
- Assume for purpose of contradiction that $\sqrt{2}$ is rational.
  $$\begin{aligned} \Rightarrow \sqrt{2} = \frac{a}{b} \\ \Rightarrow 2 = \frac{a^2}{b^2} \\ \Rightarrow 2b^2 = a^2 \\ \therefore a \ is \ even \ (\frac{2}{a}) \\ \Rightarrow \frac{4}{a^2} \\ \Rightarrow \frac{4}{2b^2} \\ \Rightarrow \frac{2}{b^2} \\ \therefore b\ is \ even \end{aligned}$$
- If a, b are both even, $\therefore \frac{a}{b}$ is not in lowest terms
- $\therefore$  Contradiction
 ```ad-success
 ```
 
 
## Induction
```ad-help
title: Inference Rule
A rule (modus ponens) says that a proof of P together with proof of P $\Rightarrow$ Q is a proof of Q.
```

 ```ad-important
  Let P(n) be a predicate. If P(0) is true and $\forall$ n $\in$ N (P(n) $\Rightarrow$ P(n + 1)) is true. Then $\forall$ n $\in$ N is true. If P(0), P(1) $\Rightarrow$ P(2), P(2) $\Rightarrow$ P(3) ..., then P(0), P(1), P(2) ... is true
  ``` 
```ad-warning
Induction often does not give answer, and it just only proves or disproves the answer.
```
```ad-example
$$\begin{aligned} \forall \  n \geq 0, 1+ 2+3+4+ ... +n = \frac{n(n + 1)}{2} = \sum _{i=1}^n i = \sum^{1 \ \leq i \ \leq n} i =  \sum_{1 \ \leq i \ \leq n}i\end{aligned}$$
 ```ad-note
 title: Solution
 Proof by Induction
  Let P(n) be the proposition, $$P(n) =\sum _{i=1}^n i = \frac{n(n + 1)}{2}$$
  Base Case: P(0) is true, $$\sum _{i=1}^0 i = \frac{0(0 + 1)}{2} = 0$$
Inductive Step: For n $\geq$ 0, show P(n) $\Rightarrow$ P(n + 1) is true.
    Assume P(n) is true for purposes of induction. (i.e. assume 1+2+ ... +n = n (n + 1) / 2)
    and need to show 1+2+ ... + (n + 1) = (n + 1)(n + 2) / 2.
    $$\begin{aligned} 1+2+ ... + (n + 1) = \frac{(n + 1)(n + 2)}{2} 
    \\ \Rightarrow \frac{n(n + 1)}{2} + (n + 1) = \frac{(n+1)(n+2)}{2} \\ \Rightarrow \frac{n^2 + 3n + 2}{2}= \frac{(n+1)(n+2)}{2}\end{aligned}$$
    $\therefore$ $\forall$ n $\geq$  0, P(n) $\Rightarrow$ P(n + 1) (proved)
 ```ad-success
 ```
 
 
```ad-example
   $$\forall \ n \in N, \ \frac{3}{n^3 -n}$$
```ad-note
title: Solution
Proof by Induction,
Let P(n) be the proposition, $$P(n) = \frac{3}{n^3-n}$$
Base Condition: P(0), $$P(0)=\frac{3}{0-0} = 0$$
Induction Step, $\forall$ n $\geq$ 0, show P(n) $\Rightarrow$ P(n + 1) is true
  Assume P(n) is true, i.e. P(n) = $\frac{3}{n^3-n}$ 
  and need to show, 
  $$\begin{align*}
P(n+1)=\frac{3}{(n+1)^3-(n+1)}\\
=\frac{3}{n^3+3n^2+3n+1-(n-1)}\\
=\frac{3}{n^3+3n^2+2n}\\
=\frac{3}{n^3-n+3n^2+3n}
\end{align*}$$
 $\therefore$ $\forall$ n $\geq$  0, P(n) $\Rightarrow$ P(n + 1) (proved)
 ```ad-success
 ```
 
 
#### False Proof
````ad-example
All hourses are the same colour
````ad-note
title: Solution
 Proof by induction,
 Let P(n) be 
> Any set of n horses, the horses are all the same colour

Base Case: P(1) is true as there is only one horse

Induction step: Assume P(n) to prove P(n + 1)
	Consider a set of n + 1 horses $H_1+H_2+...+H_{n+1}$
	Since $H_1+H_2+...+H_{n}$ are the same colour,
	$\therefore$ colour($H_1$) = colour($H_2+...+H_{n}$) = colour($H_{n+1}$)

$\therefore$ P(n) $\Rightarrow$ P(n + 1)
```ad-failure
```
```ad-warning
P(1) $\Rightarrow$ P(2), need to proved first
Let P(1) be $H_1$ and P(2) be $H_1+H_2$,
$\Rightarrow$ colour($H_1$)=colour( $\phi$ ) = colour($H_2$)
$\therefore$ Base Case Fails
````
### Using Induction to find solution
````ad-example
$\forall$ n, there is way to tile a $Z^{n}*Z^{n}$ region with a center square missing, using L shaped tiles (for bill).

````ad-note
title: Solution
Base Case: P(1) is true
Inductive Step: For n $\geq$ 0, assume P(n) to verify, that P(n + 1) is true.
Consider a $2^{n+1}*2^{n+1}$
![300](images/tilemissing.png)

```ad-fail
```
```ad-hint
When any induction hypothesis fails, making the hypothesis more stronger, makes it easier to proof.

$\forall$ n, there is way to tile a $Z^{n}*Z^{n}$ region with **any** square missing, using L shaped tiles (for bill).

(makes it much easier to proof)
````
