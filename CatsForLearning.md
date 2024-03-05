---
marp: true
---
# 🐈🧠🤖 Categorical Learning Algorithms 🐈🧠🤖
Tristan Engst
---
---
# Outline

1. Quick primer on category theory (minimum math to understand the rest)
2. Three Cool Papers
    1. _Backprop as a Functor: A Compositional Perspective on Supervised Learning_
    2. _Categorical Stochastic Processes and Likelihood_
    3. _Categorical Foundations of Gradient-Based Learning_
3. ❓
4. 💰

---
# Category Theory Primer
- A **category** is a collection of **objects** optionally connected by **morphisms**
- _A category is defined by rules governing how its objects combine and the morphisms between them. This allows imposing additional structure_
- **Example.** In **Set**, each object is a set and each morphism a function between sets
- **Functors** are morphisms between categories that respect the structure of the categories they map from and to

---
# Category Theory Primer: Example

---
# Backprop as a Functor
- A neural network is a parameterized function built by composing other parameterized functions (read: they have lots of structure)


---
Preliminaries
- Consider a basic supervised learning setting. We want to approximate $f:A\rightarrow B$ by searching over a set of parameterized functions whose parameters come from a set $P$
- Let $I:P\times A \rightarrow B$ be an  **implementation function**—
- Let $U:P\times A \times B \rightarrow P$ be an **update function**—
- Let $r: