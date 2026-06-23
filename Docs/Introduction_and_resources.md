# Introduction and Resources

This file provides a brief introduction to quantum computing and quantum error
correction. It is based on the resources listed below and is meant to support the
course notebooks.

## Recommended Resources

- **Quantum mechanics, quantum gates, and notation**
  - A nice introductory [blog](https://quantum.country/qcvc) gives an intuitive overview of the basic ideas behind quantum mechanics, quantum gates, and the notation used in quantum computing.

- **Main textbook**
  - Nielsen and Chuang, *Quantum Computation and Quantum Information*:
    [PDF link](https://profmcruz.wordpress.com/wp-content/uploads/2017/08/quantum-computation-and-quantum-information-nielsen-chuang.pdf)
  - Chapters of this course, which were used for the exercises: **Chapters 4, and 10**.
  - The book contains many exercises.

- **Quantum computers in the real world**
  - For a practical explanation of real quantum computers, including the large
    refrigerators used to cool quantum hardware, see:
    [What is quantum computing?](https://www.techtarget.com/whatis/definition/quantum-computing)

- **Quantum error correction**
  - Introductory motivation:
    [Why do we need quantum error correction?](https://quantum.microsoft.com/en-us/insights/education/concepts/quantum-error-correction)
  - More detailed explanation:
    [Why do quantum computers need QEC?](https://www.riverlane.com/blog/why-do-quantum-computers-need-qec)

- **Amazing resources to learn**
  - Interactive playground [playground](https://davidbkemp.github.io/QuantumComputingArticle/) 
  - Nice collection of resources and communities on [this git page](https://github.com/FerjaniMY/Quantum_Computing_resources#learning). (Some of the links are outdated)


---
# General theoretical background

## Why Do We Need Quantum Computers?

Classical computers are extremely powerful, but some important problems require
so much time and memory that solving realistic versions of them becomes
practically impossible.

Quantum computers offer a different model of computation. They use quantum
effects such as **superposition** and **interference** to process information in
new ways.

> **Important:** Quantum computers are not faster for every task. Their value is
> that, for certain problems, they can provide major speedups over the best known
> classical methods.

Two important examples show this potential:

- **Shor's algorithm**
  - Factors large numbers and solves related mathematical problems much faster
    than the best known classical methods.
  - This has important consequences for cryptography.

- **Grover's algorithm**
  - Searches unordered data more efficiently than classical brute-force search.
  - Provides a **quadratic speedup** for search-based problems.
  - Can help with optimization, pattern finding, and testing possible solutions.

In short, quantum computers may make some problems feasible that are far too
resource-intensive for classical computers.

Potential application areas include:

- Cryptography
- Data search
- Optimization
- Scientific computation
- Simulation of quantum systems

---

## From Classical Bits to Qubits

To understand how quantum advantages are achieved, we need to connect the
abstract idea of quantum computation with the physical systems that implement it.

A classical computer stores information in **bits**, which can only take one of
two values:

- `0`
- `1`

A quantum computer uses **qubits** instead. Qubits are physical quantum systems,
such as:

- The spin of an electron
- The energy levels of an atom or ion
- States in a superconducting circuit

## Superposition

A qubit can represent more than one possible state because quantum systems can
exist in a **superposition**.

Before measurement, a qubit is described as a combination of the states
`|0>` and `|1>`, rather than being fixed as only one of them.

For example, an electron's spin may be used to encode `|0>` and `|1>`, while a
superposition describes a state where both possibilities are present in a
controlled quantum way.

> **Key idea:** Quantum gates act on the full quantum state, including
> superpositions. This allows useful outcomes to be amplified and unwanted
> outcomes to be reduced through interference.

When a qubit is measured, it gives one classical result:

- `0`, or
- `1`

Before measurement, however, its quantum state contains **probability
amplitudes**.

> **Reminder:** Qubits are quantum states. Their evolution is described by
> **unitary operations**, which preserve the structure and normalization of the
> state.

---

## Quantum Circuits

An efficient and powerful language for describing quantum algorithms is the
language of **quantum circuits**.

Quantum circuits describe computations as assemblies of discrete components,
usually called **gates**. This construction helps us quantify the cost of an
algorithm using quantities such as:

- The total number of gates required
- The circuit depth
- The number of qubits used

The circuit model also provides a useful toolbox for algorithm design. It makes
abstract quantum operations easier to visualize, compare, and reason about.

# How to proceed next

The educational notebooks presented in this repositories are covering the following topics:

-  Quantum computing stack, qubits, and quantum states **0.0_quantum_states.ipynb**
-  Quantum gates **0.1_quantum_gates.ipynb**
-  Quantum circuits **1.0_quantum_circuits.ipynb**

Each notebook contains a set of exercises accompanied with theoretical explanation and background.