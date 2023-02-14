#discretemath 
Can we construct the necessary components of [[Boolean Logic]] using [[Sets]]? Indubitably. 

New notation:
R ~> C 
R is represented as C. 
(Everything we want to do with R we can do with C, but maybe if a different way)

F ~> Ø (The empty set)
T ~> {Ø} (The set containing the empty set)

p ∧ q ~> P ⋂ Q
| ⋂ | Ø | {Ø} |
| - | - | - |
| Ø | Ø | Ø |
| {Ø} | Ø | {Ø} |
The set intersection operator behaves like the boolean and operator with our T, F representations. 

p ∨ q ~> P ⋃ Q 
| ⋃ | Ø | {Ø} |
| - | - | - |
| Ø | Ø | {Ø} |
| {Ø} | {Ø} | {Ø} |
The set union operator behaves like the boolean or operator with our T, F representations. 

¬p ~> {Ø} - P 
| {Ø} - P | |
|-|-|
|Ø|{Ø}|
|{Ø}| Ø |
{Ø} - P behaves like the boolean not operator with our T, F representations. 

We can do ¬ ∧ ∨ with sets, so by DeMorgan's Laws, we get functional completeness.
