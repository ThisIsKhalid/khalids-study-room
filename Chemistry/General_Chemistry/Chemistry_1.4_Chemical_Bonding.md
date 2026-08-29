# Chemistry --- Pillar 1

# 1.4 Chemical Bonding

> **Goal:** Rebuild chemical bonding from the beginning and understand
> how atoms combine to form molecular structures. This is one of the
> most important chemistry topics for cheminformatics because
> **molecular structures are fundamentally defined by atoms and the
> bonds connecting them**.

This lesson follows three layers:

1.  **Layer 1 → Concept:** understand what it means.
2.  **Layer 2 → Problems:** solve basic → intermediate questions.
3.  **Layer 3 → Cheminformatics connection:** understand how the
    chemistry appears later in computational chemistry and
    cheminformatics.

------------------------------------------------------------------------

# 1. Chemical Bonds

## Layer 1 → Concept

A **chemical bond** is an attractive interaction that holds atoms
together in a chemical substance.

Atoms bond because the resulting arrangement can be more energetically
favorable than the separated atoms.

The electrons involved in bonding are primarily **valence electrons**.

A simplified picture:

``` text
Atoms
  ↓
Valence electrons interact
  ↓
Chemical bonds form
  ↓
Molecules / compounds form
```

The three broad types of bonding you need to know are:

``` text
Ionic
Covalent
Metallic
```

For cheminformatics, **covalent bonding** is especially important
because most organic and drug-like molecules are represented as networks
of atoms connected by covalent bonds.

### Layer 2 → Problems

**Problem 1**

Which electrons are most important for ordinary chemical bonding?

**Answer:** Valence electrons.

**Problem 2**

Name the three broad types of chemical bonding.

**Answer:**

-   Ionic
-   Covalent
-   Metallic

### Layer 3 → Cheminformatics Connection

A molecular graph represents:

``` text
Atoms → Nodes
Bonds → Edges
```

For example:

``` text
C — C — O
```

can be represented as:

``` text
C ── C ── O
```

where the atoms are nodes and the bonds are edges.

Bond information is essential for:

-   Molecular graphs
-   SMILES
-   MOL/SDF files
-   Molecular fingerprints
-   Molecular descriptors
-   Substructure searching
-   Similarity searching
-   QSAR
-   Molecular machine learning

------------------------------------------------------------------------

# 2. Ionic Bonding

## Layer 1 → Concept

**Ionic bonding** occurs when oppositely charged ions attract each
other.

A simple model is:

``` text
Metal + Nonmetal
      ↓
Electron transfer
      ↓
Cation + Anion
      ↓
Electrostatic attraction
      ↓
Ionic compound
```

Example:

``` text
Na → Na⁺ + e⁻

Cl + e⁻ → Cl⁻
```

Then:

``` text
Na⁺ + Cl⁻ → NaCl
```

The sodium atom loses an electron, while chlorine gains one.

The resulting ions attract because:

``` text
Positive ↔ Negative
```

### Important distinction

Ionic bonding is not best thought of as one isolated "electron pair
bond" like a typical covalent bond.

Instead, ionic compounds form structures stabilized by electrostatic
interactions between ions.

For example, solid NaCl forms an extended crystal lattice.

``` text
Na⁺ Cl⁻ Na⁺ Cl⁻
Cl⁻ Na⁺ Cl⁻ Na⁺
Na⁺ Cl⁻ Na⁺ Cl⁻
```

### Layer 2 → Problems

**Problem 1**

What usually happens to a metal during formation of an ionic compound?

**Answer:** It tends to lose electrons and become a cation.

**Problem 2**

What usually happens to a nonmetal?

**Answer:** It tends to gain electrons and become an anion.

**Problem 3**

What holds Na⁺ and Cl⁻ together?

**Answer:** Electrostatic attraction between opposite charges.

### Layer 3 → Cheminformatics Connection

Ionic compounds are important when chemical databases contain:

-   Salts
-   Counterions
-   Protonated molecules
-   Deprotonated molecules
-   Metal ions

For example, a compound record might contain:

``` text
Drug cation + chloride counterion
```

A cheminformatics workflow may need to determine whether to:

-   Keep the salt as a multi-component structure
-   Separate the components
-   Identify the parent molecule
-   Standardize the charge state

This is a major part of **chemical structure standardization**.

------------------------------------------------------------------------

# 3. Covalent Bonding

## Layer 1 → Concept

A **covalent bond** forms when atoms share electrons.

Covalent bonds are especially common between nonmetal atoms.

Example:

``` text
H + H → H—H
```

Each hydrogen contributes one electron to a shared pair.

Another example:

``` text
H₂O
```

Oxygen shares electrons with two hydrogen atoms.

### Shared electrons

A covalent bond contains a pair of shared electrons.

``` text
A : B
```

can represent a shared electron pair.

More commonly:

``` text
A — B
```

represents a single covalent bond.

### Layer 2 → Problems

**Problem 1**

What happens to electrons in a covalent bond?

**Answer:** They are shared between atoms.

**Problem 2**

Is H₂ a covalent molecule?

**Answer:** Yes.

**Problem 3**

Is C---C a covalent bond?

**Answer:** Yes.

### Layer 3 → Cheminformatics Connection

Covalent bonds form the backbone of most molecular structures in
cheminformatics.

A structure such as:

``` text
CH₃—CH₂—OH
```

is encoded as a graph containing:

``` text
C — C
    |
    O
```

The exact bond connectivity determines the molecule's identity.

This is why **structure representation** is one of the core topics of
cheminformatics.

------------------------------------------------------------------------

# 4. Metallic Bonding

## Layer 1 → Concept

**Metallic bonding** describes bonding in metals where valence electrons
are relatively delocalized throughout the metal structure.

A simplified model is:

``` text
Metal atoms
     ↓
Valence electrons become delocalized
     ↓
Positive metal centers + mobile electrons
```

This helps explain properties such as:

-   Electrical conductivity
-   Thermal conductivity
-   Malleability
-   Ductility

### Layer 2 → Problems

**Problem 1**

Are metallic electrons strongly localized between two particular metal
atoms?

**Answer:** No. They are relatively delocalized throughout the metal.

**Problem 2**

Why do metals conduct electricity?

**Answer:** Their mobile/delocalized electrons can move through the
material.

### Layer 3 → Cheminformatics Connection

Metallic bonding is not usually the central bonding model for ordinary
drug-like molecules.

However, metal chemistry becomes important for:

-   Coordination compounds
-   Catalysts
-   Metalloproteins
-   Organometallic chemistry
-   Metal-containing drugs

------------------------------------------------------------------------

# 5. Lewis Structures

## Layer 1 → Concept

A **Lewis structure** is a diagram that represents valence electrons and
bonding in a molecule or ion.

It shows:

-   Bonds
-   Lone pairs
-   Formal charges when needed

Example: H₂

``` text
H—H
```

The line represents a shared pair of electrons.

Example: H₂O

``` text
  ..
H—O—H
  ..
```

Oxygen has:

-   Two bonding pairs
-   Two lone pairs

Therefore oxygen has four electron pairs around it.

### Why Lewis structures matter

Lewis structures help you determine:

-   How atoms are connected
-   Number of bonds
-   Lone pairs
-   Formal charges
-   Resonance
-   Approximate electron arrangement

### Layer 2 → Problems

Draw the Lewis structure of:

### H₂

``` text
H—H
```

### HCl

``` text
H—Cl
```

Chlorine has three lone pairs.

### H₂O

``` text
  ..
H—O—H
  ..
```

### NH₃

``` text
   H
   |
H—N—H
   :
```

Nitrogen has one lone pair.

### Layer 3 → Cheminformatics Connection

Lewis structures help explain information that molecular software must
represent:

``` text
Atoms
+
Connectivity
+
Bond order
+
Charge
+
Lone-pair-related chemistry
```

They are a bridge between hand-drawn chemistry and computational
molecular representation.

------------------------------------------------------------------------

# 6. Octet Rule

## Layer 1 → Concept

The **octet rule** is a useful introductory rule stating that many atoms
tend to achieve a valence-shell arrangement resembling eight electrons.

For many main-group elements:

``` text
Atoms form bonds
      ↓
Gain / lose / share electrons
      ↓
More stable valence-shell arrangement
```

Examples:

### Sodium

``` text
Na → Na⁺
```

loses one electron.

### Chlorine

``` text
Cl → Cl⁻
```

gains one electron.

### Carbon

Carbon has four valence electrons and commonly forms four covalent
bonds.

``` text
   H
   |
H—C—H
   |
   H
```

This is methane, CH₄.

### Important exceptions

The octet rule is a useful model, not an absolute law.

Important exceptions include:

-   Hydrogen follows a duet rule.
-   Boron and some other atoms can have incomplete octets.
-   Expanded-valence structures occur for some elements in higher
    periods.
-   Odd-electron species can exist.

You do not need to master all exceptions immediately.

### Layer 2 → Problems

**Problem 1**

How many valence electrons does carbon have?

**Answer:** 4.

**Problem 2**

How many covalent bonds does carbon commonly form in simple neutral
molecules?

**Answer:** 4.

**Problem 3**

Does hydrogen need eight electrons?

**Answer:** No. Hydrogen follows a duet rule and is stable with two
electrons in its first shell.

### Layer 3 → Cheminformatics Connection

Valence rules are important in molecular structure validation.

When software reads:

``` text
C—C—O
```

it must determine whether the atoms have chemically plausible valences.

This affects:

-   Structure sanitization
-   SMILES parsing
-   Molecular graph construction
-   Bond-order assignment
-   Structure validation

------------------------------------------------------------------------

# 7. Formal Charge

## Layer 1 → Concept

**Formal charge** is a bookkeeping method used to assign charge to
individual atoms in a Lewis structure.

The common formula is:

``` text
Formal charge
=
Valence electrons
− Nonbonding electrons
− 1/2(Bonding electrons)
```

For an atom in a Lewis structure, you compare:

``` text
How many valence electrons the neutral atom normally has
```

with

``` text
How many electrons are assigned to it in the structure
```

### Example: Ammonium, NH₄⁺

Nitrogen normally has:

``` text
5 valence electrons
```

In NH₄⁺, nitrogen has four bonds and no lone pair.

Assigned electrons:

``` text
0 nonbonding
+ 4 bonding electrons assigned as half of 8
= 4
```

Therefore:

``` text
Formal charge = 5 - 0 - 4
              = +1
```

So nitrogen carries a +1 formal charge.

### Important distinction

**Formal charge is not necessarily the same thing as actual partial
charge.**

Formal charge is a bookkeeping model.

Partial charges describe an unequal distribution of electron density.

### Layer 2 → Problems

**Problem 1**

Calculate the formal charge of hydrogen in H₂.

Hydrogen has 1 valence electron.

It participates in one bond:

``` text
1 - 0 - 1 = 0
```

Answer: **0**

**Problem 2**

What is the total formal charge of a neutral molecule?

**Answer:** 0.

**Problem 3**

What should the sum of formal charges equal for an ion?

**Answer:** The overall charge of the ion.

### Layer 3 → Cheminformatics Connection

Formal charge is directly represented in molecular formats and software.

For example, a molecular graph can store:

``` text
Atom
 ├─ Element: N
 ├─ Formal charge: +1
 └─ Bonds: 4
```

Charge information influences:

-   Molecular descriptors
-   Protonation state
-   Salt identification
-   Similarity
-   Molecular fingerprints
-   Molecular docking
-   Machine-learning features

------------------------------------------------------------------------

# 8. Resonance

## Layer 1 → Concept

**Resonance** occurs when a single Lewis structure cannot adequately
represent the electron distribution of a molecule or ion.

Multiple valid Lewis structures can be drawn.

These are called **resonance contributors**.

The actual molecule is not rapidly switching between structures.

Instead:

``` text
Resonance contributors
        ↓
Actual electron distribution
```

is better described as a **resonance hybrid**.

### Example: Carbonate

Carbonate, CO₃²⁻, can be represented using multiple equivalent Lewis
structures where the location of the double bond changes.

Conceptually:

``` text
   O                 O
   ||                |
O—C—O⁻    ↔      O—C=O
```

The actual electron density is delocalized.

### Another important example: benzene

Benzene is often drawn as:

``` text
   ⌬
```

or using alternating double bonds.

Its π electrons are delocalized around the ring.

### Layer 2 → Problems

**Problem 1**

Does a molecule actually jump between resonance structures?

**Answer:** No.

The resonance structures are alternative representations of one
underlying electron distribution.

**Problem 2**

What does resonance often indicate?

**Answer:** Electron delocalization.

### Layer 3 → Cheminformatics Connection

Resonance is extremely important when software determines:

-   Aromaticity
-   Bond orders
-   Charge placement
-   Molecular equivalence
-   Tautomer/structure representations

A molecule can have multiple chemically reasonable drawings that
represent essentially the same underlying structure.

Cheminformatics must often **standardize** these representations.

------------------------------------------------------------------------

# 9. Bond Polarity

## Layer 1 → Concept

A covalent bond can be:

-   Nonpolar
-   Polar

depending on how equally the bonding electrons are shared.

The key concept is **electronegativity**.

If two atoms have similar electronegativities:

``` text
A — B
```

the electrons are shared more equally.

If one atom is substantially more electronegative:

``` text
Aδ+ — Bδ−
```

the bonding electrons are pulled toward B.

### Example: C---O

Oxygen is more electronegative than carbon.

Therefore:

``` text
Cδ+ — Oδ−
```

### Example: O---H

Oxygen is much more electronegative than hydrogen.

Therefore:

``` text
Hδ+ — Oδ−
```

### Layer 2 → Problems

**Problem 1**

Which side of C---O carries the partial negative character?

**Answer:** Oxygen.

**Problem 2**

Why?

**Answer:** Oxygen is more electronegative than carbon.

**Problem 3**

Is a C---C bond strongly polar?

**Answer:** No. The two carbon atoms have the same electronegativity.

### Layer 3 → Cheminformatics Connection

Bond polarity affects:

-   Molecular dipole
-   Hydrogen bonding
-   Solubility
-   Protein interactions
-   Reactivity
-   Lipophilicity

This is why atom-level properties matter when predicting molecular
behavior.

------------------------------------------------------------------------

# 10. Electronegativity

## Layer 1 → Concept

**Electronegativity** is the tendency of an atom in a chemical bond to
attract shared electrons toward itself.

A useful general trend is:

``` text
Electronegativity increases ↑
Electronegativity increases →
```

Fluorine is the most electronegative element.

For common organic elements, a useful simplified ranking is:

``` text
F > O > N > C > H
```

### Why it matters

Electronegativity differences help determine:

``` text
Bond polarity
     ↓
Charge distribution
     ↓
Molecular polarity
     ↓
Intermolecular interactions
```

### Layer 2 → Problems

**Problem 1**

Which is more electronegative: O or C?

**Answer:** O.

**Problem 2**

Which is more electronegative: N or O?

**Answer:** O.

**Problem 3**

Which is more electronegative: F or O?

**Answer:** F.

### Layer 3 → Cheminformatics Connection

Electronegativity contributes to the behavior of:

-   Functional groups
-   Hydrogen-bond donors/acceptors
-   Polar molecules
-   Charged molecules
-   Drug--target interactions

It is one of the chemical ideas underlying many molecular-property
differences.

------------------------------------------------------------------------

# 11. Bond Strength

## Layer 1 → Concept

**Bond strength** describes how strongly atoms are held together by a
chemical bond.

A useful quantitative measure is **bond dissociation energy (BDE)**: the
energy required to break a bond homolytically in the gas phase under
specified conditions.

In general:

``` text
Stronger bond
     ↓
More energy required to break it
```

Bond strength depends on factors such as:

-   Bond order
-   Bond length
-   Atom identity
-   Molecular environment

A simplified relationship is:

``` text
Higher bond order
      ↓
Generally stronger bond
```

For example:

``` text
C—C    single
C=C    double
C≡C    triple
```

Generally:

``` text
C≡C > C=C > C—C
```

in bond strength.

This is a useful generalization, not a universal rule for every
molecular environment.

### Layer 2 → Problems

**Problem 1**

Which is generally stronger: C---C or C=C?

**Answer:** C=C.

**Problem 2**

Which generally requires more energy to break: a single or triple bond
between comparable atoms?

**Answer:** Triple bond.

### Layer 3 → Cheminformatics Connection

Bond strength is relevant to:

-   Chemical stability
-   Reactivity
-   Reaction prediction
-   Bond-breaking/forming transformations
-   Molecular degradation
-   Metabolism

In reaction informatics, a reaction can be thought of computationally
as:

``` text
Break bond(s)
      +
Form bond(s)
      ↓
Product structure
```

------------------------------------------------------------------------

# 12. Bond Length

## Layer 1 → Concept

**Bond length** is the average distance between the nuclei of two bonded
atoms.

For comparable atoms:

``` text
Higher bond order
      ↓
Shorter bond
```

Example:

``` text
C—C    longer
C=C    shorter
C≡C    shortest
```

Again, the exact values depend on the atoms and molecular environment.

### Why?

Higher bond order generally means greater electron density between the
nuclei, which strengthens the interaction and pulls the atoms closer
together.

### Layer 2 → Problems

**Problem 1**

Which is generally shorter: C---C or C=C?

**Answer:** C=C.

**Problem 2**

Which is generally shorter: C=C or C≡C?

**Answer:** C≡C.

### Layer 3 → Cheminformatics Connection

Bond lengths are fundamental to **3D molecular structure**.

A molecular structure can contain:

``` text
Atom identity
+
Connectivity
+
Bond order
+
3D coordinates
```

3D coordinates are important for:

-   Molecular mechanics
-   Molecular dynamics
-   Docking
-   3D similarity
-   Quantum chemistry
-   Structure-based drug discovery

------------------------------------------------------------------------

# 13. Coordinate Covalent Bonds

## Layer 1 → Concept

A **coordinate covalent bond**, also called a **dative bond**, is a
covalent bond in which both electrons in the shared pair are initially
supplied by the same atom.

Conceptually:

``` text
Lewis base with lone pair
          ↓
      donates pair
          ↓
Lewis acid / electron acceptor
```

Example:

``` text
NH₃ + H⁺ → NH₄⁺
```

Nitrogen uses its lone pair to form a bond with H⁺.

It can be illustrated as:

``` text
NH₃ → H⁺
```

After the bond forms, it is generally treated as an ordinary covalent
bond in the resulting structure.

### Another example

Metal coordination:

``` text
Ligand with lone pair
        ↓
      Metal
```

For example:

``` text
NH₃ → Cu²⁺
```

This type of chemistry becomes important in coordination complexes.

### Layer 2 → Problems

**Problem 1**

Who supplies both electrons in a coordinate covalent bond?

**Answer:** The donor atom or ligand supplies both electrons.

**Problem 2**

What type of species typically accepts the electron pair?

**Answer:** An electron-deficient species such as a Lewis acid or metal
center.

**Problem 3**

In NH₃ + H⁺ → NH₄⁺, which atom donates the electron pair?

**Answer:** Nitrogen.

### Layer 3 → Cheminformatics Connection

Coordinate bonding matters in:

-   Metal complexes
-   Metalloproteins
-   Catalysts
-   Drug--metal interactions
-   Bioinorganic chemistry

It can be challenging for cheminformatics systems because coordination
chemistry does not always fit neatly into the ordinary organic
single/double/triple-bond model.

------------------------------------------------------------------------

# 14. Single, Double, and Triple Bonds

## Layer 1 → Concept

Covalent bonds can have different **bond orders**.

### Single bond

``` text
A—B
```

One shared electron pair.

Bond order:

``` text
1
```

### Double bond

``` text
A=B
```

Two shared electron pairs.

Bond order:

``` text
2
```

### Triple bond

``` text
A≡B
```

Three shared electron pairs.

Bond order:

``` text
3
```

Generally:

``` text
Bond order ↑
     ↓
Bond strength ↑
     ↓
Bond length ↓
```

This is a useful general relationship.

### Layer 2 → Problems

**Problem 1**

What is the bond order of C=O?

**Answer:** 2.

**Problem 2**

What is the bond order of N≡N?

**Answer:** 3.

**Problem 3**

Which is generally shorter: C---C or C≡C?

**Answer:** C≡C.

### Layer 3 → Cheminformatics Connection

Bond order is a core part of molecular representation.

For example:

``` text
C-C
C=C
C#C
```

represent different connectivity/bond-order information.

A SMILES representation can encode these differences:

``` text
C-C
C=C
C#C
```

This affects molecular identity, fingerprints, descriptors, and reaction
transformations.

------------------------------------------------------------------------

# 15. Polar vs Nonpolar Molecules

## Layer 1 → Concept

A **polar bond** does not automatically mean the whole molecule is
polar.

Molecular polarity depends on:

1.  Bond polarities
2.  Molecular geometry

Example:

### CO₂

Each C=O bond is polar:

``` text
Oδ−=Cδ+=Oδ−
```

But CO₂ is linear:

``` text
O=C=O
```

The bond dipoles point in opposite directions and cancel.

Therefore the molecule is overall **nonpolar**.

### H₂O

The O---H bonds are polar and the molecule is bent:

``` text
  O
 / \
H   H
```

The dipoles do not cancel.

Therefore water is **polar**.

### Layer 2 → Problems

**Problem 1**

Does a polar bond always mean the molecule is polar?

**Answer:** No.

**Problem 2**

Why is CO₂ overall nonpolar?

**Answer:** Its linear geometry causes the two bond dipoles to cancel.

**Problem 3**

Why is H₂O polar?

**Answer:** It has polar O---H bonds and a bent molecular geometry, so
the dipoles do not cancel.

### Layer 3 → Cheminformatics Connection

Molecular polarity influences:

-   Solubility
-   Membrane permeability
-   Protein binding
-   Hydrogen bonding
-   Distribution in biological systems

This is highly relevant to drug discovery.

A cheminformatics workflow may calculate descriptors that capture
aspects of molecular polarity, such as:

-   TPSA
-   H-bond donor count
-   H-bond acceptor count
-   Partial-charge-related descriptors

------------------------------------------------------------------------

# 16. Bonding and Molecular Structure

Put the concepts together:

``` text
Valence electrons
        ↓
Atoms interact
        ↓
Chemical bonds
        ↓
Bond type
        ↓
Bond order
        ↓
Connectivity
        ↓
Molecular structure
        ↓
3D geometry
        ↓
Molecular properties
```

For example:

``` text
Carbon + Oxygen
       ↓
C—O bond
       ↓
Different electronegativities
       ↓
Polar bond
       ↓
Charge distribution
       ↓
Molecular properties
```

This chain of reasoning is extremely important for your future chemistry
and cheminformatics study.

------------------------------------------------------------------------

# 17. Chemistry → Cheminformatics Bridge

This topic is one of the most direct bridges between chemistry and
cheminformatics.

## Chemistry view

``` text
Atoms
 ↓
Valence electrons
 ↓
Chemical bonding
 ↓
Molecular structure
 ↓
Molecular properties
```

## Computer view

``` text
Atoms → Nodes
Bonds → Edges
Bond order → Edge attributes
Charge → Atom attributes
Aromaticity → Atom/bond attributes
3D coordinates → Geometry
```

Therefore:

``` text
Chemical molecule
       ↓
Molecular graph
       ↓
Computer-readable representation
```

For example:

``` text
Ethanol

CH₃—CH₂—OH
```

can be viewed computationally as:

``` text
C ── C ── O
```

with additional information about:

``` text
Atom types
Hydrogens
Bond orders
Charges
Aromaticity
Coordinates
```

This is the foundation for molecular informatics.

------------------------------------------------------------------------

# 18. Why Bonding Matters for SMILES

SMILES is one of the most important molecular representations you will
encounter.

For simple examples:

``` text
Ethane:
CC

Ethene:
C=C

Ethyne:
C#C
```

Notice that changing the bond changes the chemical structure.

``` text
CC
C=C
C#C
```

These are different molecules.

Therefore, a cheminformatics program must understand both:

``` text
Which atoms?
+
How are they connected?
+
What are the bond orders?
```

This is why chemical bonding comes before serious work with SMILES.

------------------------------------------------------------------------

# 19. Why Bonding Matters for Molecular Fingerprints

A molecular fingerprint encodes structural patterns.

Conceptually:

``` text
Molecule
   ↓
Atoms + bonds
   ↓
Structural patterns
   ↓
Fingerprint
   ↓
Similarity calculation
```

For example, these molecules differ in connectivity/bonding:

``` text
CCO
C=CO
CC=O
```

Even when they contain similar atoms, their structures are different.

Their fingerprints can therefore be different.

This is fundamental to:

-   Molecular similarity
-   Virtual screening
-   Compound clustering
-   Library analysis
-   QSAR

------------------------------------------------------------------------

# 20. Why Bonding Matters for Reactions

A chemical reaction changes molecular connectivity.

Conceptually:

``` text
Reactant
   ↓
Bond breaking
+
Bond formation
   ↓
Product
```

For example:

``` text
A—B + C
      ↓
A—C + B
```

Reaction informatics tries to represent and predict these
transformations computationally.

This becomes important later for:

-   Reaction databases
-   Reaction prediction
-   Retrosynthesis
-   Synthesis planning
-   Reaction-center detection

------------------------------------------------------------------------

# 21. Practice --- Basic

Try these before checking the answers.

### Question 1

What are the three broad types of chemical bonding?

### Question 2

What happens to electrons in a covalent bond?

### Question 3

What happens to electrons when a typical metal forms a cation?

### Question 4

What is a Lewis structure?

### Question 5

What does the octet rule describe?

### Question 6

What is formal charge?

### Question 7

What is resonance?

### Question 8

What determines bond polarity?

### Question 9

What is bond order?

### Question 10

What is a coordinate covalent bond?

------------------------------------------------------------------------

# 22. Answers --- Basic

### 1

``` text
Ionic
Covalent
Metallic
```

### 2

They are shared between atoms.

### 3

The metal generally loses electrons.

### 4

A diagram showing valence electrons, bonds, lone pairs, and relevant
formal charges.

### 5

The tendency of many atoms to achieve a valence-shell arrangement
resembling eight electrons.

### 6

A bookkeeping charge assigned to an atom in a Lewis structure.

### 7

Multiple valid Lewis structures that represent different
electron-distribution contributors for one underlying species.

### 8

Primarily the difference in electronegativity between bonded atoms.

### 9

The number of shared electron pairs represented between two bonded
atoms.

### 10

A covalent bond in which both electrons in the shared pair are initially
supplied by one atom.

------------------------------------------------------------------------

# 23. Practice --- Intermediate

### Question 1

Why does NaCl form an ionic compound?

### Question 2

Why is C---O polar?

### Question 3

Why is C---C essentially nonpolar?

### Question 4

Which bond is generally shorter?

``` text
C—C
C=C
C≡C
```

### Question 5

Which bond is generally strongest?

``` text
C—C
C=C
C≡C
```

### Question 6

Why is CO₂ overall nonpolar even though C=O bonds are polar?

### Question 7

Why is H₂O polar?

### Question 8

Why is formal charge not the same as partial charge?

### Question 9

Why is resonance important in cheminformatics?

### Question 10

Why does bond order matter in a molecular graph?

------------------------------------------------------------------------

# 24. Answers --- Intermediate

### 1

Sodium tends to lose an electron and chlorine tends to gain one:

``` text
Na → Na⁺
Cl → Cl⁻
```

The oppositely charged ions attract.

### 2

Oxygen is more electronegative than carbon, so the bonding electrons are
pulled toward oxygen.

### 3

Both atoms have the same electronegativity, so the electrons are shared
approximately equally.

### 4

Generally:

``` text
C≡C
```

is shortest.

### 5

Generally:

``` text
C≡C
```

is strongest.

### 6

CO₂ is linear, so the two C=O bond dipoles point in opposite directions
and cancel.

### 7

Water has polar O---H bonds and a bent geometry, so the bond dipoles do
not cancel.

### 8

Formal charge is a bookkeeping assignment based on an idealized
electron-sharing model. Partial charge describes an actual or estimated
uneven distribution of electron density.

### 9

Different resonance drawings can represent the same underlying chemical
species. Cheminformatics systems may need to recognize equivalent
representations and handle bond orders and charges consistently.

### 10

Bond order changes the chemical identity and properties of a structure.

For example:

``` text
C—C
```

and

``` text
C=C
```

are chemically different.

------------------------------------------------------------------------

# 25. Cheminformatics Mini-Exercise

Consider:

``` text
Ethanol

CH₃—CH₂—OH
```

Identify:

### Atoms

``` text
C
C
O
H
```

### Main heavy-atom bonds

``` text
C—C
C—O
```

### Bond orders

``` text
C—C → 1
C—O → 1
```

### Polarity

``` text
C—O → polar
C—C → essentially nonpolar
```

### Molecular graph

``` text
C ── C ── O
```

This simple example demonstrates the basic information a cheminformatics
program needs.

------------------------------------------------------------------------

# 26. Important Relationships to Memorize

## Bond type

``` text
Ionic
→ electron transfer / ion attraction

Covalent
→ electron sharing

Metallic
→ delocalized electrons in metals
```

## Bond order

``` text
Single → 1
Double → 2
Triple → 3
```

## General bond-order relationship

``` text
Bond order ↑
     ↓
Bond strength ↑
     ↓
Bond length ↓
```

## Polarity

``` text
Electronegativity difference
          ↓
Unequal electron sharing
          ↓
Bond polarity
```

## Molecular polarity

``` text
Bond polarity
      +
Molecular geometry
      ↓
Overall molecular polarity
```

## Molecular graph

``` text
Atoms → Nodes
Bonds → Edges
```

------------------------------------------------------------------------

# 27. Mastery Checklist

Before moving to **1.5 Molecular Geometry**, make sure you can:

## Chemical Bonding

-   [ ] Explain why chemical bonds form
-   [ ] Explain ionic bonding
-   [ ] Explain covalent bonding
-   [ ] Explain metallic bonding
-   [ ] Draw simple Lewis structures
-   [ ] Understand the octet rule
-   [ ] Recognize important octet-rule exceptions
-   [ ] Calculate simple formal charges
-   [ ] Explain resonance
-   [ ] Explain bond polarity
-   [ ] Use electronegativity to predict bond polarity
-   [ ] Explain bond strength
-   [ ] Explain bond length
-   [ ] Understand coordinate covalent bonds
-   [ ] Distinguish single, double, and triple bonds
-   [ ] Understand bond order

## Cheminformatics

You should understand:

``` text
Atom
 ↓
Bond
 ↓
Connectivity
 ↓
Molecular graph
 ↓
SMILES
 ↓
Descriptors / fingerprints
```

And you should understand why:

``` text
Changing a bond
      ↓
Changes molecular structure
      ↓
Can change molecular properties
      ↓
Can change biological activity
```

------------------------------------------------------------------------

# 28. Final Mastery Test

Try these without notes.

### 1.

Explain the difference between ionic and covalent bonding.

### 2.

Why does Na become Na⁺?

### 3.

Why does Cl become Cl⁻?

### 4.

Draw the Lewis structure of H₂O.

### 5.

How many lone pairs are on oxygen in H₂O?

### 6.

What is the formal charge of nitrogen in NH₄⁺?

### 7.

What is resonance?

### 8.

Why is C---O polar?

### 9.

Why is CO₂ nonpolar overall?

### 10.

Which is generally shorter: C---C or C=C?

### 11.

Which is generally stronger: C=C or C≡C?

### 12.

What is a coordinate covalent bond?

### 13.

In a molecular graph, what do nodes represent?

### 14.

In a molecular graph, what do edges represent?

### 15.

Why does bond order matter in cheminformatics?

------------------------------------------------------------------------

# 29. Final Answers

### 1

Ionic bonding involves attraction between oppositely charged ions,
typically after electron transfer. Covalent bonding involves sharing
electrons between atoms.

### 2

Sodium commonly loses one valence electron, producing a +1 ion.

### 3

Chlorine commonly gains one electron, producing a −1 ion.

### 4

``` text
  ..
H—O—H
  ..
```

### 5

Two lone pairs.

### 6

+1.

### 7

Resonance is the use of multiple valid Lewis structures to represent
different electron-distribution contributors for the same underlying
species.

### 8

Oxygen is more electronegative than carbon and attracts the shared
electrons more strongly.

### 9

Its linear geometry causes the two bond dipoles to cancel.

### 10

C=C.

### 11

C≡C, generally.

### 12

A bond where both electrons in the shared pair are initially supplied by
one atom.

### 13

Atoms.

### 14

Bonds.

### 15

Because different bond orders represent different molecular structures
and chemical behavior. Bond order is therefore essential for correctly
representing molecules computationally.

------------------------------------------------------------------------

# 30. One-Page Memory Sheet

## Three Bond Types

``` text
Ionic
→ ions + electrostatic attraction

Covalent
→ shared electrons

Metallic
→ delocalized electrons
```

## Bond Order

``` text
Single  → 1
Double  → 2
Triple  → 3
```

## General Relationship

``` text
Higher bond order
       ↓
Stronger bond
       ↓
Shorter bond
```

## Polarity

``` text
Electronegativity difference
          ↓
Unequal sharing
          ↓
Polar bond
```

But:

``` text
Polar bonds ≠ necessarily polar molecule
```

Molecular geometry determines whether dipoles cancel.

## Lewis Structures

Remember:

``` text
Bonds
+
Lone pairs
+
Formal charges
```

## Resonance

``` text
Multiple Lewis contributors
          ↓
Electron delocalization
```

## Cheminformatics

``` text
Atoms → Nodes
Bonds → Edges
Bond order → Bond attribute
Charge → Atom attribute
Connectivity → Molecular identity
```

------------------------------------------------------------------------

# 31. Next Topic

## 1.5 Molecular Geometry

The next topic builds directly on chemical bonding:

``` text
Lewis structures
      ↓
Electron domains
      ↓
VSEPR theory
      ↓
Molecular geometry
      ↓
Bond angles
      ↓
Linear
Trigonal planar
Tetrahedral
Trigonal pyramidal
Bent
Trigonal bipyramidal
Octahedral
      ↓
Molecular polarity
      ↓
3D molecular structure
      ↓
Cheminformatics / molecular modeling
```

This is especially important because cheminformatics eventually moves
from **2D connectivity** to **3D molecular structure**.
