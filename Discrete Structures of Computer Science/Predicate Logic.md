#discretemath
Predicate -- Function that may take various arguments and always return T or F. Choose predicates to build up a formal theory of something.


### Quantifiers
Quantifiers -- Prefix on an expression that introduces a variable (any kind of value)

##### Types
∀<sub>x</sub> P(x) - The universal quantifier "for all". X is chosen from a set of all possible values (assumed).
P(x) is true for all these x's. Related to ∧:

∀<sub>x</sub> P(x) ≡ P(x1) ∧ P(x2) ∧ ... ∧ P(xn)

∃x P(x) - The existential quantifier "for some", X is chosen from a set of all possible values and P(x) is true for at least one of them. Related to ∨:

∃<sub>x</sub> P(x) ≡ P(x1) ∨ P(x2) ∨ ... ∨ P(xn)

Ex. ∀<sub>x</sub> (even(x) ∨ odd(x)), ¬∃x (even(x))

##### "Element Of" Notation
If x is chosen from some implicit set of values (s), it would be written as ∀x∈s P(x) or ∃x∈s P(x)
The ∈ symbol means "element of"

##### DeMorgan's Law for Quantifiers
¬∀<sub>x</sub> P(X) ≡ ¬(P(x1) ∧ (Px2) ∧ ... ∧ P(xn))
			  ≡ ¬P(x1) ∨ ¬(Px2) ∨ ... ∨ ¬P(xn))
			  ≡ ∃<sub>x</sub> ¬P(x)

¬∃<sub>x</sub> P(X) ≡ ¬(P(x1) ∨ (Px2) ∨ ... ∨ P(xn))
			  ≡ ¬P(x1) ∧ ¬(Px2) ∧ ... ∧ ¬P(xn))
			  ≡ ∀<sub>x</sub> ¬P(x)

##### Nesting Quantifiers
You can nest quantifiers of different kinds:

∀<sub>x</sub>∃<sub>y</sub> P(x, y) - "For all x there exists a y such that P(x,y)"
≡
∀<sub>x</sub> P(x, f(x)) <--- Skolem function

[[Example- Mysterious Island of Duosomata]]

##### Extensions
∃!<sub>x</sub> P(x) - There is exactly one x for which P(x) is true.
Ex. ∃!<sub>x</sub> int(x) ∧ zero(x)

∃!<sub>x</sub> P(x) - There is exactly n items x for which P(x) is true.
ex. ∃2 x int(x) ∧ | x | = 1

### Rules for Quantified Expressions
A<sub>1</sub>  <--- Antecedents
A<sub>2</sub>
C   <--- Consequent

**Universal Instantiation**
∀<sub>x</sub> P(x)
P(c), where c is an arbitrary constant member of x, we don't know it's value.

**Universal Generalization**
P(c), for some constant c
∀<sub>x</sub> P(x)

**Existential Instantiation**
∃<sub>x</sub> P(x)
P(c), where c is an arbitrary constant member of x, we don't know it's value.

**Existential Generalization**
P(c), for some constant c
∃<sub>x</sub> P(x)

**Universal Modus Ponens**
∀<sub>x</sub> P(x) → Q(x)
P(a)
Q(a)

**Universal Modus Tollens**
∀<sub>x</sub> P(x) → Q(x)
¬Q(a)
¬P(a)

[[Example- Rules for Quantified Expressions]]
