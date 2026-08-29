# Chemistry --- Pillar 1

# 1.2 Atomic Structure

> **Goal:** Rebuild atomic-structure fundamentals from the beginning,
> then connect them to how molecules are represented and processed in
> cheminformatics.

This lesson follows the same three-layer method:

1.  **Layer 1 → Concept:** understand what it means.
2.  **Layer 2 → Problems:** basic → intermediate.
3.  **Layer 3 → Cheminformatics connection:** understand how the
    chemistry appears later in computational chemistry and
    cheminformatics.

------------------------------------------------------------------------

## 1. Atoms

### Layer 1 → Concept

An **atom** is the basic unit of an element that retains the chemical
identity of that element.

An atom contains three major subatomic particles:

  Particle     Charge   Relative mass Location
  ---------- -------- --------------- ----------------
  Proton           +1         \~1 amu Nucleus
  Neutron           0         \~1 amu Nucleus
  Electron         -1    \~1/1836 amu Electron cloud

The atom can be simplified as:

``` text
                 Atom
                  |
          +-------+-------+
          |               |
       Nucleus       Electron cloud
          |               |
     +----+----+          |
     |         |          |
  Protons   Neutrons   Electrons
```

The **nucleus** contains protons and neutrons.

Electrons occupy regions around the nucleus.

### Important idea

The number of **protons** determines which element the atom is.

For example:

``` text
1 proton  → Hydrogen
6 protons → Carbon
7 protons → Nitrogen
8 protons → Oxygen
17 protons → Chlorine
```

Changing the number of protons changes the element itself.

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

An atom contains 6 protons. What element is it?

**Answer:** Carbon.

**Problem 2**

An atom contains 8 protons and 8 neutrons. What element is it?

**Answer:** Oxygen.

The number of protons is 8, so it is oxygen.

**Problem 3**

Can an atom of carbon become oxygen by gaining two electrons?

**Answer:** No.

Changing electrons changes the charge, not the identity of the element.
Carbon must have 6 protons; oxygen must have 8.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

A cheminformatics system needs to know the identity of every atom in a
molecule.

For example:

``` text
C — C — O
```

The computer interprets this as:

``` text
Atom 1 → Carbon
Atom 2 → Carbon
Atom 3 → Oxygen
```

This atomic information becomes part of a molecular graph:

``` text
Carbon —— Carbon —— Oxygen
  Node       Node       Node
```

Later, tools such as **RDKit** use this information to calculate
molecular properties, descriptors, fingerprints, and molecular graphs.

------------------------------------------------------------------------

# 2. Protons

### Layer 1 → Concept

A **proton** is a positively charged particle found in the nucleus.

Its charge is:

``` text
+1
```

The number of protons is called the **atomic number**.

Therefore:

``` text
Atomic number = Number of protons
```

Examples:

``` text
Hydrogen → 1 proton → Z = 1
Carbon   → 6 protons → Z = 6
Nitrogen → 7 protons → Z = 7
Oxygen   → 8 protons → Z = 8
```

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

An element has atomic number 12. How many protons does it have?

**Answer:** 12.

**Problem 2**

An atom has 15 protons. Which element is it?

**Answer:** Phosphorus.

**Problem 3**

An atom has 17 protons. If the number of protons becomes 18, is it still
chlorine?

**Answer:** No. It becomes argon.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

The atomic number identifies the atom type computationally.

A molecular representation must distinguish:

``` text
C ≠ N ≠ O ≠ S ≠ Cl
```

This matters because changing an atom type can dramatically change:

-   Molecular weight
-   Bonding
-   Polarity
-   Hydrogen bonding
-   Reactivity
-   Molecular descriptors
-   Biological activity

------------------------------------------------------------------------

# 3. Neutrons

### Layer 1 → Concept

A **neutron** is a neutral particle found in the nucleus.

Its charge is:

``` text
0
```

Neutrons contribute to the mass of an atom but do not determine its
element.

Atoms of the same element can have different numbers of neutrons. These
are called **isotopes**.

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

Does changing the number of neutrons change the element?

**Answer:** No.

**Problem 2**

Two atoms both have 6 protons. One has 6 neutrons and the other has 8
neutrons. Are they the same element?

**Answer:** Yes. Both are carbon.

They are different isotopes of carbon.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Most molecular representations focus on the normal elemental identity,
but isotopic information can also be explicitly represented.

This matters in applications involving:

-   Isotope labeling
-   Mass spectrometry
-   Metabolic tracing
-   Reaction mechanisms
-   Isotope-resolved molecular data

------------------------------------------------------------------------

# 4. Electrons

### Layer 1 → Concept

An **electron** is a negatively charged particle associated with an
atom.

Charge:

``` text
-1
```

Electrons are especially important for chemistry because they
participate in:

-   Chemical bonding
-   Ion formation
-   Chemical reactions
-   Molecular polarity
-   Redox reactions

The nucleus is positively charged because of its protons, while
electrons provide negative charge.

For a neutral atom:

``` text
Number of protons = Number of electrons
```

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

A neutral carbon atom has 6 protons. How many electrons does it have?

**Answer:** 6.

**Problem 2**

A neutral oxygen atom has 8 protons. How many electrons?

**Answer:** 8.

**Problem 3**

An atom has 11 protons and 10 electrons. Is it neutral?

**Answer:** No.

Its net charge is:

``` text
11(+) + 10(-) = +1
```

So it is a +1 ion.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Electron-related information is essential for understanding:

-   Bond orders
-   Formal charge
-   Aromaticity
-   Protonation
-   Ionization
-   Molecular interactions

When you eventually use RDKit, an atom can carry properties such as:

``` text
Element
Atomic number
Formal charge
Aromaticity
Hybridization
Number of hydrogens
```

These properties influence how the molecule is interpreted
computationally.

------------------------------------------------------------------------

# 5. Atomic Number

### Layer 1 → Concept

The **atomic number (Z)** is the number of protons in an atom.

``` text
Z = number of protons
```

Examples:

  Element     Atomic number
  --------- ---------------
  H                       1
  C                       6
  N                       7
  O                       8
  F                       9
  P                      15
  S                      16
  Cl                     17

Atomic number is the element's identity.

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

What is the atomic number of nitrogen?

**Answer:** 7.

**Problem 2**

An atom has 16 protons. Identify it.

**Answer:** Sulfur.

**Problem 3**

An atom has atomic number 8 and 10 electrons. What is its charge?

Protons = 8\
Electrons = 10

``` text
Charge = 8 - 10 = -2
```

**Answer:** 2−.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Atomic number is one of the most fundamental pieces of information in a
molecular graph.

A molecular graph can be thought of as:

``` text
Molecule
   |
   +-- Nodes → atoms
   |           |
   |           +-- atomic number
   |           +-- charge
   |           +-- aromaticity
   |
   +-- Edges → bonds
```

Machine-learning models eventually use this information to learn
molecular representations.

------------------------------------------------------------------------

# 6. Mass Number

### Layer 1 → Concept

The **mass number (A)** is the total number of protons and neutrons in
an atom.

``` text
A = protons + neutrons
```

Therefore:

``` text
Number of neutrons = A - Z
```

Example:

Carbon-12:

``` text
Protons = 6
Neutrons = 6

A = 6 + 6
A = 12
```

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

An atom has 11 protons and 12 neutrons. What is its mass number?

``` text
A = 11 + 12
A = 23
```

**Answer:** 23.

**Problem 2**

An atom has mass number 35 and atomic number 17. How many neutrons?

``` text
Neutrons = 35 - 17
         = 18
```

**Answer:** 18.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Mass information becomes important in analytical chemistry and molecular
data, especially:

-   Mass spectrometry
-   Isotope patterns
-   Molecular formula determination
-   Isotope-labeled compounds

For a molecular formula such as:

``` text
C8H10N4O2
```

a computer can calculate an expected molecular mass from the atomic
masses of the constituent atoms.

------------------------------------------------------------------------

# 7. Isotopes

### Layer 1 → Concept

**Isotopes are atoms of the same element that have the same number of
protons but different numbers of neutrons.**

Example:

Carbon:

``` text
Carbon-12
6 protons
6 neutrons

Carbon-13
6 protons
7 neutrons

Carbon-14
6 protons
8 neutrons
```

All three are carbon because all have 6 protons.

They differ in mass because they have different numbers of neutrons.

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

Carbon-13 has 6 protons. How many neutrons?

``` text
13 - 6 = 7
```

**Answer:** 7.

**Problem 2**

An isotope has atomic number 8 and mass number 18. How many neutrons?

``` text
18 - 8 = 10
```

**Answer:** 10.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Isotopes appear in:

-   Mass spectrometry
-   Isotope labeling
-   Drug metabolism studies
-   Molecular tracing
-   Structure databases

In cheminformatics, isotope information may need to be preserved when
converting between molecular representations.

------------------------------------------------------------------------

# 8. Ions

### Layer 1 → Concept

An **ion** is an atom or group of atoms with a net electrical charge.

An ion forms when electrons are gained or lost.

``` text
Lose electrons → positive ion
Gain electrons → negative ion
```

------------------------------------------------------------------------

# 9. Cations

A **cation** is a positively charged ion.

It forms when an atom loses electrons.

Example:

``` text
Na → Na⁺ + e⁻
```

Sodium:

``` text
11 protons
10 electrons
```

Net charge:

``` text
+1
```

Other examples:

``` text
K⁺
Mg²⁺
Ca²⁺
Al³⁺
```

------------------------------------------------------------------------

# 10. Anions

An **anion** is a negatively charged ion.

It forms when an atom gains electrons.

Example:

``` text
Cl + e⁻ → Cl⁻
```

Chloride has:

``` text
17 protons
18 electrons
```

Net charge:

``` text
-1
```

Other examples:

``` text
F⁻
O²⁻
S²⁻
```

------------------------------------------------------------------------

## Layer 2 → Ion Problems

### Problem 1

A magnesium atom has 12 protons and loses 2 electrons.

How many electrons remain?

``` text
12 - 2 = 10
```

Charge:

``` text
12 - 10 = +2
```

**Answer: Mg²⁺**

### Problem 2

An oxygen atom has 8 protons and gains 2 electrons.

Electrons:

``` text
8 + 2 = 10
```

Charge:

``` text
8 - 10 = -2
```

**Answer: O²⁻**

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Charge is extremely important in molecular informatics.

The same chemical structure can exist in different protonation/charge
states.

For example:

``` text
Neutral form
     ↓
Protonation/deprotonation
     ↓
Charged form
```

Charge affects:

-   Solubility
-   Lipophilicity
-   Hydrogen bonding
-   Molecular interactions
-   Binding
-   Docking
-   Molecular descriptors

This is why **protonation states** become an important topic later.

------------------------------------------------------------------------

# 11. Atomic Mass

### Layer 1 → Concept

Atomic mass describes the mass of an atom.

The masses of atoms are commonly expressed in **atomic mass units
(amu)** or **daltons (Da)**.

A proton and neutron each have approximately 1 amu, while an electron is
much lighter.

In real chemistry, atomic masses are not always whole numbers because
naturally occurring elements often exist as mixtures of isotopes.

For example, the periodic-table atomic mass of carbon is approximately:

``` text
12.01 amu
```

rather than exactly 12 amu.

------------------------------------------------------------------------

# 12. Average Atomic Mass

### Layer 1 → Concept

The periodic-table atomic mass is a **weighted average** of the
naturally occurring isotopes of an element.

Conceptually:

``` text
Average atomic mass
=
Σ(isotope mass × fractional abundance)
```

For a simplified example:

Suppose an element has:

``` text
Isotope A:
mass = 10 amu
abundance = 20%

Isotope B:
mass = 11 amu
abundance = 80%
```

Then:

``` text
Average mass
= (10 × 0.20) + (11 × 0.80)
= 2.0 + 8.8
= 10.8 amu
```

------------------------------------------------------------------------

### Layer 2 → Problems

An element has two isotopes:

``` text
Mass 20 amu → 75%
Mass 22 amu → 25%
```

Calculate the average atomic mass.

``` text
(20 × 0.75) + (22 × 0.25)

= 15 + 5.5

= 20.5 amu
```

**Answer: 20.5 amu**

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Atomic mass is used to calculate:

-   Molecular mass
-   Molecular weight
-   Molecular formula mass
-   Expected mass spectra
-   Isotope patterns

For example:

``` text
H₂O
```

can be calculated from the atomic masses of:

``` text
2 × H + 1 × O
```

This becomes useful when processing chemical structures computationally.

------------------------------------------------------------------------

# 13. Electron Shells

### Layer 1 → Concept

Electrons occupy regions of space around the nucleus called **electron
shells** or principal energy levels.

They are associated with the principal quantum number:

``` text
n = 1, 2, 3, 4, ...
```

The farther the shell is from the nucleus, generally the higher its
energy.

Simplified:

``` text
             n = 3
          ┌─────────┐
          │         │
          │  n = 2  │
          │ ┌─────┐ │
          │ │n = 1│ │
          │ │ ●   │ │
          │ └─────┘ │
          └─────────┘
             nucleus
```

------------------------------------------------------------------------

### Layer 2 → Problems

Which shell generally has higher energy?

**n = 3** has higher energy than **n = 2**.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Electron arrangement helps explain why atoms:

-   Form particular bonds
-   Have particular valences
-   Prefer certain oxidation states
-   Form particular molecular geometries

These chemical rules eventually determine the molecular structures that
cheminformatics software represents.

------------------------------------------------------------------------

# 14. Subshells

### Layer 1 → Concept

Each principal shell contains subshells.

The four types are:

``` text
s
p
d
f
```

Their general capacities are:

  Subshell     Number of orbitals   Maximum electrons
  ---------- -------------------- -------------------
  s                             1                   2
  p                             3                   6
  d                             5                  10
  f                             7                  14

Therefore:

``` text
s → 2 electrons
p → 6 electrons
d → 10 electrons
f → 14 electrons
```

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

How many electrons can a p subshell hold?

**Answer:** 6.

**Problem 2**

How many orbitals are in a d subshell?

**Answer:** 5.

**Problem 3**

What is the maximum number of electrons in an f subshell?

**Answer:** 14.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Subshells are part of the foundation for understanding:

-   Valence electrons
-   Bonding
-   Hybridization
-   Molecular orbitals
-   Electronic properties

Later, these concepts help you understand why different atoms behave
differently in molecular structures.

------------------------------------------------------------------------

# 15. Orbitals

### Layer 1 → Concept

An **orbital** is a region of space where there is a high probability of
finding an electron.

An orbital is not a physical circular path like a planet orbiting the
Sun.

Important orbital types:

### s orbital

Approximately spherical.

``` text
      ___
   /       \
  |    ●    |
   \       /
      ‾‾‾
```

### p orbitals

Have two lobes.

There are three p orbitals:

``` text
pₓ
pᵧ
p𝓏
```

They point along different spatial directions.

A p subshell contains 3 orbitals and can hold 6 electrons.

------------------------------------------------------------------------

### Layer 2 → Problems

How many orbitals are in:

-   s subshell → **1**
-   p subshell → **3**
-   d subshell → **5**
-   f subshell → **7**

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Orbital concepts help explain molecular:

-   Geometry
-   Bonding
-   Hybridization
-   Electronic distribution
-   Reactivity

These properties ultimately affect molecular descriptors and chemical
behavior.

------------------------------------------------------------------------

# 16. Quantum Numbers

### Layer 1 → Concept

Quantum numbers describe the state of an electron in an atom.

There are four:

``` text
n  → principal quantum number
l  → angular momentum quantum number
mₗ → magnetic quantum number
mₛ → spin quantum number
```

------------------------------------------------------------------------

## 16.1 Principal Quantum Number --- n

Describes the main energy level.

``` text
n = 1, 2, 3, 4, ...
```

------------------------------------------------------------------------

## 16.2 Angular Momentum Quantum Number --- l

Describes the subshell.

Relationship:

``` text
l = 0 → s
l = 1 → p
l = 2 → d
l = 3 → f
```

------------------------------------------------------------------------

## 16.3 Magnetic Quantum Number --- mₗ

Describes orbital orientation.

For a given `l`:

``` text
mₗ = -l ... 0 ... +l
```

Examples:

For s:

``` text
l = 0
mₗ = 0
```

For p:

``` text
l = 1
mₗ = -1, 0, +1
```

Therefore p has 3 orbitals.

------------------------------------------------------------------------

## 16.4 Spin Quantum Number --- mₛ

An electron has one of two possible spin states:

``` text
+1/2
-1/2
```

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

What subshell corresponds to:

``` text
l = 2
```

**Answer:** d.

**Problem 2**

What values can `mₗ` have when:

``` text
l = 1
```

**Answer:**

``` text
-1, 0, +1
```

**Problem 3**

What possible values can electron spin have?

**Answer:**

``` text
+1/2 or -1/2
```

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Quantum numbers are not usually directly entered into everyday
cheminformatics workflows.

However, they provide the foundation for understanding:

``` text
Electron structure
      ↓
Chemical bonding
      ↓
Molecular structure
      ↓
Molecular properties
      ↓
Computational representation
```

You don't need to calculate quantum numbers every time you use RDKit,
but understanding the chemistry underneath molecular structure is
valuable.

------------------------------------------------------------------------

# 17. Electron Configurations

### Layer 1 → Concept

An **electron configuration** describes how electrons are distributed
among orbitals.

The main filling order begins approximately as:

``` text
1s
2s
2p
3s
3p
4s
3d
4p
5s
4d
5p
...
```

Three important rules:

### Aufbau principle

Electrons generally occupy lower-energy orbitals before higher-energy
orbitals.

### Pauli exclusion principle

An orbital can contain a maximum of two electrons, and they must have
opposite spins.

### Hund's rule

Electrons occupy degenerate orbitals singly before pairing.

------------------------------------------------------------------------

## Example: Hydrogen

Hydrogen has 1 electron:

``` text
1s¹
```

## Example: Helium

Helium has 2 electrons:

``` text
1s²
```

## Example: Carbon

Carbon has 6 electrons:

``` text
1s² 2s² 2p²
```

## Example: Oxygen

Oxygen has 8 electrons:

``` text
1s² 2s² 2p⁴
```

------------------------------------------------------------------------

### Layer 2 → Problems

Write the electron configuration of:

### Hydrogen

**1s¹**

### Carbon

**1s² 2s² 2p²**

### Nitrogen

**1s² 2s² 2p³**

### Oxygen

**1s² 2s² 2p⁴**

### Neon

**1s² 2s² 2p⁶**

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Electron configuration helps explain why:

``` text
C → commonly forms 4 bonds
N → commonly forms 3 bonds
O → commonly forms 2 bonds
H → commonly forms 1 bond
```

These patterns are fundamental to molecular structure.

When cheminformatics software validates or interprets molecular
structures, chemical valence rules are important.

------------------------------------------------------------------------

# 18. Valence Electrons

### Layer 1 → Concept

**Valence electrons** are electrons in the outermost occupied shell that
are important in chemical bonding.

For many main-group elements, valence electrons strongly influence:

-   Bond formation
-   Reactivity
-   Oxidation states
-   Molecular geometry

Examples:

``` text
H → 1 valence electron
C → 4
N → 5
O → 6
F → 7
```

This helps explain common bonding patterns.

------------------------------------------------------------------------

## Example: Carbon

Carbon:

``` text
1s² 2s² 2p²
```

The outer shell is:

``` text
2s² 2p²
```

Total valence electrons:

``` text
2 + 2 = 4
```

Carbon therefore commonly forms four covalent bonds.

------------------------------------------------------------------------

## Example: Oxygen

Oxygen:

``` text
1s² 2s² 2p⁴
```

Valence electrons:

``` text
2 + 4 = 6
```

Oxygen commonly forms two bonds and has two lone pairs in many common
neutral structures.

------------------------------------------------------------------------

### Layer 2 → Problems

**Problem 1**

How many valence electrons does carbon have?

**Answer:** 4.

**Problem 2**

How many valence electrons does oxygen have?

**Answer:** 6.

**Problem 3**

How many valence electrons does nitrogen have?

**Answer:** 5.

**Problem 4**

How many valence electrons does chlorine have?

**Answer:** 7.

------------------------------------------------------------------------

### Layer 3 → Cheminformatics Connection

Valence electrons connect directly to one of the most important concepts
you'll learn next:

``` text
Valence electrons
       ↓
Chemical bonding
       ↓
Lewis structures
       ↓
Bond orders
       ↓
Molecular structure
       ↓
SMILES / SDF / Molecular graph
       ↓
RDKit
```

This is one of the most important bridges between basic chemistry and
cheminformatics.

------------------------------------------------------------------------

# 19. Putting Atomic Structure Together

You should now be able to connect all the pieces:

``` text
                    ATOM
                      |
             +--------+--------+
             |                 |
          Nucleus         Electron cloud
             |                 |
       +-----+-----+       Shells
       |           |          |
    Protons     Neutrons   Subshells
       |           |          |
       |           |       s p d f
       |           |          |
       |           |       Orbitals
       |           |          |
       +-----+-----+       Electrons
             |
       Atomic number
             |
       Mass number
```

Then:

``` text
Electron configuration
        ↓
Valence electrons
        ↓
Chemical bonding
        ↓
Molecular structure
        ↓
Molecular representation
        ↓
Cheminformatics
```

------------------------------------------------------------------------

# 20. Essential Relationships to Memorize

These are the relationships you should know without hesitation.

### Atomic number

``` text
Z = number of protons
```

### Mass number

``` text
A = protons + neutrons
```

### Neutrons

``` text
N = A - Z
```

### Neutral atom

``` text
protons = electrons
```

### Ion charge

``` text
Charge = protons - electrons
```

### Cation

``` text
Lose electrons → positive
```

### Anion

``` text
Gain electrons → negative
```

### Subshell capacity

``` text
s → 2
p → 6
d → 10
f → 14
```

### Orbital count

``` text
s → 1 orbital
p → 3 orbitals
d → 5 orbitals
f → 7 orbitals
```

### Quantum numbers

``` text
n  → energy level
l  → subshell
mₗ → orbital orientation
mₛ → electron spin
```

------------------------------------------------------------------------

# 21. Mixed Practice --- Basic

Try these yourself before checking the answers.

### Question 1

An atom has:

``` text
Z = 12
A = 24
```

Find:

-   Protons
-   Neutrons
-   Electrons for a neutral atom

### Question 2

An ion has:

``` text
17 protons
18 electrons
```

What is its charge?

### Question 3

An atom has:

``` text
8 protons
10 electrons
```

What is its charge?

### Question 4

How many electrons can a d subshell contain?

### Question 5

How many orbitals are in a p subshell?

### Question 6

What is the electron configuration of carbon?

### Question 7

How many valence electrons does oxygen have?

### Question 8

Two atoms have the same number of protons but different numbers of
neutrons. What are they?

------------------------------------------------------------------------

# 22. Answers

### 1

``` text
Protons = 12
Neutrons = 24 - 12 = 12
Electrons = 12
```

### 2

``` text
17 - 18 = -1
```

**Answer: 1−**

### 3

``` text
8 - 10 = -2
```

**Answer: 2−**

### 4

**10 electrons**

### 5

**3 orbitals**

### 6

``` text
1s² 2s² 2p²
```

### 7

**6**

### 8

**Isotopes**

------------------------------------------------------------------------

# 23. Intermediate Practice

### Question 1

An ion has:

``` text
Atomic number = 16
Mass number = 32
Charge = 2−
```

Find:

-   Protons
-   Neutrons
-   Electrons

### Question 2

An ion has:

``` text
19 protons
18 electrons
```

Identify:

-   Element
-   Charge
-   Cation or anion

### Question 3

An isotope has:

``` text
Mass number = 40
Atomic number = 20
```

Find the number of:

-   Protons
-   Neutrons
-   Electrons in the neutral atom

### Question 4

Explain why changing the number of electrons does not change the
identity of an element.

### Question 5

Explain the relationship between:

``` text
Valence electrons
→ Bonding
→ Molecular structure
```

------------------------------------------------------------------------

# 24. Answers to Intermediate Practice

### 1

Atomic number = 16:

``` text
Protons = 16
```

Neutrons:

``` text
32 - 16 = 16
```

A 2− charge means two extra electrons:

``` text
Electrons = 16 + 2 = 18
```

Therefore:

``` text
Protons  = 16
Neutrons = 16
Electrons = 18
```

------------------------------------------------------------------------

### 2

19 protons means:

**Potassium (K)**

Charge:

``` text
19 - 18 = +1
```

Therefore:

**K⁺, a cation**

------------------------------------------------------------------------

### 3

``` text
Protons = 20
Neutrons = 40 - 20 = 20
Electrons = 20
```

------------------------------------------------------------------------

### 4

The number of protons determines the element.

Changing electrons changes the electrical charge:

``` text
Atom → Ion
```

but does not change the element.

------------------------------------------------------------------------

### 5

Valence electrons are involved in chemical bonding.

``` text
Valence electrons
       ↓
How atoms interact
       ↓
Chemical bonds
       ↓
Molecular geometry
       ↓
3D molecular structure
```

That structure is what we eventually represent computationally.

------------------------------------------------------------------------

# 25. Cheminformatics Connection --- The Big Picture

This is the most important section for your long-term goal.

In traditional chemistry:

``` text
Atoms
 ↓
Electrons
 ↓
Bonding
 ↓
Molecules
```

In cheminformatics:

``` text
Atoms
 ↓
Bonds
 ↓
Molecular structure
 ↓
SMILES / MOL / SDF
 ↓
Molecular graph
 ↓
Descriptors / fingerprints
 ↓
Numerical representation
 ↓
Machine Learning
```

For example, consider ethanol:

``` text
CH₃—CH₂—OH
```

A computer needs to know:

``` text
Atoms:
C, C, O, H...

Bonds:
C-C
C-O
O-H
...
```

From this structural information, software can calculate properties such
as:

-   Molecular weight
-   Hydrogen-bond donors
-   Hydrogen-bond acceptors
-   Rotatable bonds
-   TPSA
-   LogP
-   Fingerprints

Then ML can use those representations for:

``` text
Molecular structure
       ↓
Features
       ↓
ML model
       ↓
Predicted property
```

So **atomic structure is not just basic chemistry you need to pass an
exam**. It is the foundation underneath computational molecular
representation.

------------------------------------------------------------------------

# 26. What You Need to Master Before 1.3

Before moving to **1.3 Periodic Table**, make sure you can do these
without looking at notes:

-   Explain what an atom is
-   Identify protons, neutrons, and electrons
-   Calculate atomic number
-   Calculate mass number
-   Calculate number of neutrons
-   Calculate ion charge
-   Distinguish cations and anions
-   Explain isotopes
-   Calculate average atomic mass
-   Understand electron shells
-   Understand s, p, d, f subshells
-   Know orbital capacities
-   Understand the four quantum numbers
-   Write basic electron configurations
-   Identify valence electrons
-   Explain why valence electrons matter for bonding
-   Connect atoms → bonds → molecules → computational representation

## Mastery checkpoint

You should be able to look at:

``` text
³⁵₁₇Cl⁻
```

and immediately determine:

``` text
Element       → Chlorine
Atomic number → 17
Mass number   → 35
Protons       → 17
Neutrons      → 18
Electrons     → 18
Charge        → -1
Type          → Anion
```

That is the level of comfort I want you to have before we move on.

------------------------------------------------------------------------

## Source note

The uploaded source establishes **chemistry fundamentals as a
prerequisite for cheminformatics**, but it does not itself provide the
detailed atomic-structure teaching above. The detailed explanations and
problems here are an expanded **general-chemistry lesson** based on the
Chemistry pillar we created from that source. The source's broader
framing is available here: fileciteturn0file0
