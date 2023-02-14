#discretemath 

Suppose we know: ∃<sub>x</sub> C(x) ∧ ¬B(x), ∀<sub>x</sub> C(x) → P(x)
Prove: ∃<sub>x</sub> P(x) ∧ ¬B(x)

| 1. ∃<sub>x</sub> C(x) ∧ ¬B(x) | Given. |
|-|-|
| 2. C(a) ∧ ¬B(a) | Existential Instantiation:1 |
| 3. C(a) | Simplication:2 |
| 4. ∀<sub>x</sub> C(x) → P(x) | Given. |
| 5. C(a) → P(a) | Universial Instantiation:4 |
| 6. P(a) | Modus Ponens:3,5 |
| 7. ¬B(a) | Simplification:2 |
| 8. P(a) ∧ ¬B(a) | Conjunction:6,7 |
| 9. ∃<sub>x</sub> P(x) ∧ ¬B(x) | Existential Generalization:8 |

QED
