#discretemath 
Suppose we know: ¬p ∧ q, r→p, ¬r → s, s → t
Prove t.

| 1. ¬p ∧ q | Given |
|-|-|
| 2. ¬p | Simplify |
| 3.  r→p | Given |
| 4. ¬r | Modus Tollens:2,3 |
| 5. ¬r → s | Given |
| 6. s | Modus Ponens:4,5 |
| 7. s → t | Given |
| 8. t | Modus Ponens:6,7 |

QED
