#discretemath 
A proof is a mathematical argument that convinces the reader.

### Logical Proofs
S<sub>1</sub>, S<sub>2</sub>, S<sub>n</sub> (finite series of steps)
Each step is either given or deduced from previous steps by using [[Discrete Math Rules|rules]].

[[Example - Two Column Proofs]]

### Direct Proofs
p→q, assume p is true and use rules (informally) to show q is true. 

Ex. If n is odd, then n<sup>2</sup> is odd. 
∀n odd(n) → odd(n<sup>2</sup>)
Assume n is odd, n = 2k +1, n<sup>2</sup> must be (2k+1) * (2k+1) = n<sup>2</sup>
n<sup>2</sup> = 2(2k<sup>2</sup> + 2k) + 1 (Same form as odd number) so 
n<sup>2</sup> is odd, QED. 

### Contraposition
p→q ≡ ¬q→¬p, Assume ¬q and prove ¬p.

Ex. n is an int, 3n+2 is odd, show n is odd. 
Assume n is even. n = 2k, 3(2k)+2 = 6k+2 = 2(3k+1)
So 3n+2 must be even, the opposite of what we want to prove, the original must be true, QED.

### Vacuous Proofs
Hardly counts as a proof at all. p→q, but p is false. What we're trying to prove can't happen.

Ex. Suppose n>1 and n<sup>2</sup>>n 
P(n) ≡ n>1 → n<sup>2</sup>>n 
Show P(0) is true.

### Proof by Contradiction
Assume that what you want to prove is false. Reason forward from that unti lyou get a contradiction ($\neg$r $\wedge$ r). If you only assume that what you want to prove is false, a contradiction must mean it is true. 
$\neg$p$\rightarrow$(r $\wedge \space \neg$r) ≡ ¬(¬p) ∨ (r ∧ ¬r) ≡ ¬(¬p) ≡ p

Ex. $\sqrt(2)$ is irrational, rational numbers can be written as $\frac{a}{b}$ where a and b are integers. b $\neq$ 0; a, b have no common factors/divisors.
Assume $\sqrt(2)$ is rational $\sqrt(2)$ = $\frac{a}{b}$, so 2 = $\frac{a^2}{b^2}$ 
2b<sup>2</sup> = a<sup>2</sup>, a<sup>2</sup> is even, a must be even. a must be 2c. 
2b<sup>2</sup> = 4c<sup>2</sup>, b<sup>2</sup> = 2c<sup>2</sup>
2 divides into both a and b, so $\sqrt(2)$ is irrational.

### Counterexample
Show ¬∀<sub>x</sub> P(x). Find an a for which ¬P(a).

Ex. Every positive integer is the sum of squares of two integers.
For 3, numbers < 3 are 0<sup>2</sup> = 0, 1<sup>2</sup> = 1, 2<sup>2</sup> = 4
1+1 $\neq$ 3, so it must be false.

### Proof by Cases (Proof by Exhaustion)
(P<sub>1</sub>∨P<sub>2</sub>∨...∨P<sub>n</sub>) → q ≡ (P<sub>1</sub>→q)∧(P<sub>2</sub>→q)∧...∧(P<sub>n</sub>→q). Break large proof into smaller proofs, prove each one separately.

Ex. Prove (n+1)<sup>2</sup> $\ge$ 3<sup>n</sup> if n is positive integer such that n $\le$ 4
n = 1, 2, 3, 4
2<sup>3</sup> $\ge$ 3<sup>1</sup>, 3<sup>3</sup> $\ge$ 3<sup>2</sup>, etc. 

"Without loss of generality" - cases overlap; sometimes when you prove p<sub>i</sub>, you've also proven p<sub>j</sub>, 
i $\neq$ j, consider the most general case.

### Existence Proofs
∃<sub>x</sub> P(x). 
Sometimes we can simply construct x (find a value for x). "Constructive existence proof"
Sometimes we can show that x exists without knowing its value. "Nonconstructive existence proof"

Ex. Prove there are infinite primes. 
Primes have 2 divisors 1 and themselves, primes include 2, 3, 5, 7, 11, 13, ... P<sub>n</sub>
Given a finite list of all primes, multiply every prime together and add 1:
(2 * 3 * 5 * 7 * 11 ... P<sub>n</sub>) + 1
If it's prime, then the finite list of primes is false. If it isn't prime, it must have a prime divisor that isn't in the list. This is nonconstructive because we haven't shown how to construct primes.

Ex. There are irrational numbers x and y such that x<sup>y</sup> is rational.
If  $\sqrt{2}^\sqrt{2}$ is irrational, let x = $\sqrt{2}^\sqrt{2}$, y = $\sqrt{2}$
With that configuration, $\sqrt{2}^2$ = 2. 
This is a constructive existence proof because a specific value has been found that satisfies P(x). 

### Forward and Backward
Working backward: Start with the equation and try to decude a true statement. 
Working forward: Start with the assumed rules and deduce what we want to prove.

Ex. Suppose x $\neq$ y, x > 0, y > 0. 
Is (x+2)/2 > $\sqrt{xy}$ 
Backward Proof:
(x+2)/2 > $\sqrt{xy}$
(x+2)<sup>2</sup>/4 > xy
(x+y)<sup>2</sup> > 4xy
x<sup>2</sup> + 2xy + y<sup>2</sup> > 4xy
x<sup>2</sup> - 2xy + y<sup>2</sup> > 0
(x-y)<sup>2</sup> > 0, true when x >0, y > 0, x $\neq$ y






