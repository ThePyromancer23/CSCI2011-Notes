#discretemath

Show ¬(p ∨ (¬p ∧ q)) ≡ ¬p ∧ ¬q

| ¬(p ∨ (¬p ∧ q)) | Given |
|-|-|
| ¬p ∧ ¬(¬p ∧ q) | DeMorgan |
| ¬p ∧ (¬¬p ∨ ¬q) | DeMorgan |
| ¬p ∧ (p ∨ ¬q) | Double Negation |
|(¬p ∧ p) ∨ (¬p ∧ ¬q) | Distribution |
| F ∨ (¬p ∧ ¬q) | Contradiction |
| ¬p ∧ ¬q | F ∨ x ≡ x |

QED.

Show (p ∧ q) → (p ∨ q) is a tautology

|(p ∧ q) → (p ∨ q) | Given |
|-|-|
| ¬(p ∧ q) ∨ (p ∨ q) | Definition of Implication |
| (¬p ∨ ¬q) ∨ (p ∨ q) | DeMorgan |
| (¬p ∨ p) ∨ (¬q ∨ q) | Commutes & Associates |
| T ∨ T | Negation |
| T | Definition of ∨ |

