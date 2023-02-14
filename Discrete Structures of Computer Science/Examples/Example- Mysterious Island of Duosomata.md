#discretemath 
On the mysterious island of Duosomata there are 2 kinds of people, tall and short. 

x ∈ all possible things
person(x)
tall(x)
short(x)
taller(x,y)

∃<sub>x</sub> person(x) - "Some things are people."
∀<sub>x</sub> person(x) - "All things are people."
∀<sub>x</sub> person(x) → (tall(x) ∨ short(x)) - "Each person is tall or short."
∀<sub>x</sub>∀<sub>y</sub> (person(x) ∧ person(y) ∧ tall(x) ∧ short(y)) → taller(x, y) - "Tall people are taller than short people."

¬∃<sub>x</sub> person(x) ∧ tall(x) ∧ short(x) -- No person is tall and short
≡
∀<sub>x</sub> ¬person(x) ∨ ¬tall(x) ∨ ¬short(x)
≡
∀<sub>x</sub> person(x) → (¬tall(x) ∨ ¬short(x))

∀<sub>x</sub>∃<sub>y</sub> (person(x) ∧ person(y)) → (tall(x) ∧ short(y)) - "For each tall person, there exists at least one short person"

∃<sub>x</sub>∀<sub>y</sub> person(x) ∧ person(y) → taller(x, y) - "There is at least one tallest person"

