#discretemath 
"An unordered collection of distinct objects (elements)"

{ a, b, c } = { b, a, c } = { c, a, b }

- Sets could be to construct other mathematical objects.
- Set theory has paradoxes.
- Naive Set Theory- Set theory without paradoxes.

### Set Notation
Set A:
a ∈ A: a is an element of A
a $\notin$ A: a is not an element of A

Set Comprehension / Set Builder Notation
A = { x | P(x) } 

Ex. A  = { x | int(x) ∧ -10 $\le$ x $\le$ 10 } 

(Some P(x) lead to paradoxes)

Predefined sets:
**N** - natural numbers {0, 1, 2, ... }
ℚ - rational numbers {$\frac{a}{b}$, ...}
ℤ - integers
ℝ - reals
ℂ - complex

### Set Operations

**Membership**
x ∈ S - if x is an element of S

**Subset**
S<sub>1</sub> ⊆ S<sub>2</sub> - S<sub>1</sub> is a **subset** of S<sub>2</sub> if every element of S<sub>1</sub> is also an element of S<sub>2</sub>;
≡ ∀<sub>x</sub> x ∈ S<sub>1</sub> → x ∈ S<sub>2</sub> 
Every set has Ø (empty set) and itself as a subset.

**Proper Subset**
S<sub>1</sub> ⊂ S<sub>2</sub> - If S<sub>1</sub> $\neq$ S<sub>2</sub> ∧ S<sub>1</sub> ⊆ S<sub>2</sub> then it is called a "Proper Subset"

Ex. { a, b } ⊂ { a, b, c }

**Powerset**
ℙ(s) = { s' | s' ⊆ s } - A set of all the subsets of s. 

Ex. s = { a, b }, 2 elements = 2<sup>2</sup> = 4 elements
ℙ(s) = { Ø, {a}, {b}, {a, b} }
| ℙ | = 2<sup>| s |</sup> = The number of subsets

#### Familiar Set Operations

**Intersection**
S<sub>1</sub> ⋂ S<sub>2</sub> = { x |  x ∈ S<sub>1</sub> ∧ x ∈ S<sub>2</sub> }
Set of all elements in both sets. Looks/functions like ∧.

**Union**
S<sub>1</sub> ⋃ S<sub>2</sub> = { x |  x ∈ S<sub>1</sub> ∨ x ∈ S<sub>2</sub> }
Set of all elements in either set. Looks/functions like ∨.

**Set Difference**
S<sub>1</sub> - S<sub>2</sub> { x |  x ∈ S<sub>1</sub> ∧ x $\notin$ S<sub>2</sub> }
Set of all elements in S<sub>1</sub> but not S<sub>2</sub>. Basically subtraction.

**Universal Complement**
$\bar{S}$ = U - S 
Set of all elements in a universal set U but not S, assuming U is some defined/known set. 

### Paradoxes
Some sets do not exist, which is different from being an empty set.

#### Russel's Paradox
The set of all sets can be listed as: 
A = { s | set(s) }

Does A ∈ A? That would be problematic.

The set of all sets not containing themselves: 
A' = { s | sets(s) ∧ s $\notin$ s } 

If A' is in the set, then it cannot be in the set. If it isn't in the set, it must be in the set. 
This paradox means that A' does not exist.

This is similar to the barber's paradox- "A barber shaves all men who do not shave themselves. Does the barber shave himself?"

#### Application to Python
type(x) is a function that returns t of object x. What's the type of t?
Types are sets of all possible values and t is a set of types. 

type(t) is a set of all sets. 

Workarounds for this problem:
- Zermelo-Frenkel 
- Carefully construct a class so it's a set of classes. 

### Other Applications

- [[Boolean Algebra in Terms of Sets]]
- [[Represent Natural Numbers as Sets]]
- [[Represent Sets of Natural Numbers in a Computer]]




