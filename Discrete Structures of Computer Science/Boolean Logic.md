#discretemath
Propositions-- Expressions that are true or false.

Variables-- True or false values.

| Operators | (connectives) |
| - | - |
|¬p| not p |
|p∧q|p and q|
|p∨q|p or q|
|p⊕q|p [[Exclusive Or]] q|
|p→q|p [implies](Implication.md) q |
|p↔q|p is equivalent to|

### Order of Operations
1. ¬
2. ∧
3. ∨
4. →
5. ↔

### Truth Tables
[[Example- Equivalence Test|All situations can be shown with truth tables.]]
n variables means 2^n rows in the truth table.

| p | q | ¬p|p∧q|p∨q|p⊕q|p→q|p↔q|
|-|-|-|-|-|-|-|-|
|F|F|T|F|F|F|T|T|
|F|T|T|F|T|T|T|F|
|T|F|F|F|T|T|F|F|
|T|T|F|F|T|F|T|T|

#### Constructing Propositions from Truth Tables
Sum of Products Form
1. If no row is T, s≡F
2. Visit all rows with T values. Build a term (conjuctions using ∧ ) If a variable v is true, add v to term and ¬v if false.
3. Add the terms together with ∨

[[Example- Sum of Products]]

### Definitions
Suppose s is a proposition...

S is *satisfiable* if it's true for at least one assignment to its variables.
a ∨ b

s is *unsatisfiable* if it's never true 
¬p ∧ p

s is a *tautology* if it's true for all assignments to it's variables
p ∨ ¬p

s is a *contradiction* if it's not satisfiable.

### Functional Completeness
Some sets of connectives are *functionally complete*; they can create any proposition.
¬∧∨ are functionally complete by themselves, so are ¬∧ and ¬∨.

Additionally, NAND is functionally complete.

### Logical Equivalences
There are several rules for manipulating propositions. We can prove things about propositions using these identities ([[Logical Equivalences]]). 

Examples: [[Example - Two Column Proofs]]

### Rules of Inference "If-Them"
A1
A2 <-- Antecedents
...
An
C <-- Consequents

**Modus Ponens, "Method of Putting"**
p
p→q
q

**Modus Tollens, "Method of Removing"**
¬q
p→q
¬p

**Hypothetical Syllogism**
p→q
q→r
p→r

**Simplification**
p∧q
p

**Conjunction**
p
q
p ∧ q

[[Example- Rules of Inference]]

### Other Relevence 

- [[Boolean Algebra in Terms of Sets]]
