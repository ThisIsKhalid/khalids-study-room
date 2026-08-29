# Chemistry --- Pillar 1

# 1.5 Molecular Geometry

> **Goal:** Understand how atoms are arranged in three-dimensional
> space, how electron pairs determine molecular shape, how bond angles
> arise, and how molecular geometry affects polarity and molecular
> behavior.
>
> This topic is especially important for cheminformatics because
> molecules are not only **2D graphs**. Their 3D shape can strongly
> affect molecular interactions, docking, conformations, and biological
> activity.

This lesson follows:

1.  **Layer 1 → Concept:** understand what it means.
2.  **Layer 2 → Problems:** solve basic → intermediate questions.
3.  **Layer 3 → Cheminformatics connection:** understand how the
    chemistry appears later in computational chemistry and
    cheminformatics.

------------------------------------------------------------------------

# 1. Why Molecular Geometry Matters

## Layer 1 → Concept

A molecular formula tells you **which atoms are present**, but it does
not completely tell you how those atoms are arranged in space.

For example:

``` text
H₂O
```

does not mean the molecule is simply:

``` text
H—O—H
```

in a straight line.

Water is actually **bent**.

The arrangement of atoms in 3D is called **molecular geometry**.

Think of the progression as:

``` text
Atoms
  ↓
Bonds
  ↓
Electron distribution
  ↓
3D arrangement
  ↓
Molecular geometry
  ↓
Molecular properties
```

Geometry affects:

-   Molecular polarity
-   Dipole moment
-   Hydrogen bonding
-   Steric interactions
-   Molecular recognition
-   Protein binding
-   Reactivity

### Layer 2 → Problems

**Question:** Does a molecular formula alone tell you the 3D shape?

**Answer:** No.

### Layer 3 → Cheminformatics Connection

A molecular representation may contain:

``` text
2D connectivity
+
3D coordinates
```

For example:

``` text
2D:
C—C—O

3D:
(x₁,y₁,z₁)
(x₂,y₂,z₂)
(x₃,y₃,z₃)
```

The 3D coordinates determine the spatial arrangement of the atoms.

------------------------------------------------------------------------

# 2. VSEPR Theory

## Layer 1 → Concept

**VSEPR** stands for:

**Valence Shell Electron Pair Repulsion**

The central idea is:

> Electron groups around a central atom repel each other and arrange
> themselves as far apart as possible.

Think:

``` text
Electron groups
      ↓
Repel one another
      ↓
Move as far apart as possible
      ↓
Determine electron-domain geometry
```

An electron group can be:

-   A single bond
-   A double bond
-   A triple bond
-   A lone pair

### Important rule

For VSEPR, a double or triple bond counts as **one electron domain**,
even though it contains multiple bonding pairs.

For example:

``` text
O=C=O
```

Carbon has:

``` text
2 electron domains
```

not 4.

### Layer 2 → Problems

**Question:** How many electron domains does carbon have in CO₂?

``` text
O=C=O
```

Answer:

``` text
2
```

Each double bond counts as one domain.

**Question:** How many electron domains does carbon have in CH₄?

``` text
    H
    |
H—C—H
    |
    H
```

Answer:

``` text
4
```

### Layer 3 → Cheminformatics Connection

VSEPR provides a simple chemical explanation for why molecular
structures have particular 3D arrangements.

Computational chemistry later goes beyond VSEPR by calculating molecular
geometries using methods such as:

-   Molecular mechanics
-   Semi-empirical methods
-   Density functional theory
-   Quantum chemistry

VSEPR is therefore a conceptual foundation, not the final computational
method.

------------------------------------------------------------------------

# 3. Electron Domains

## Layer 1 → Concept

An **electron domain** is a region of electron density around a central
atom.

For introductory VSEPR problems, count:

``` text
Single bond → 1 domain
Double bond → 1 domain
Triple bond → 1 domain
Lone pair   → 1 domain
```

Examples:

### CH₄

``` text
4 C—H bonds
```

Therefore:

``` text
4 electron domains
```

### NH₃

``` text
3 N—H bonds
1 lone pair
```

Therefore:

``` text
4 electron domains
```

### H₂O

``` text
2 O—H bonds
2 lone pairs
```

Therefore:

``` text
4 electron domains
```

Notice something important:

``` text
CH₄ → 4 domains
NH₃ → 4 domains
H₂O → 4 domains
```

All three have the same **electron-domain geometry**, but different
molecular geometries because the number of lone pairs differs.

### Layer 2 → Problems

Determine the number of electron domains:

  Molecule     Bonding domains   Lone-pair domains   Total
  ---------- ----------------- ------------------- -------
  CH₄                        4                   0       4
  NH₃                        3                   1       4
  H₂O                        2                   2       4
  CO₂                        2                   0       2

### Layer 3 → Cheminformatics Connection

Electron-domain information helps predict molecular geometry from
connectivity and valence information.

A cheminformatics toolkit can use atom properties such as:

``` text
Element
Formal charge
Bond order
Neighbors
Hydrogen count
```

to infer chemically reasonable local structures.

------------------------------------------------------------------------

# 4. Electron-Domain Geometry vs Molecular Geometry

## Layer 1 → Concept

These two terms are related but **not identical**.

### Electron-domain geometry

Includes:

``` text
Bonding pairs
+
Lone pairs
```

### Molecular geometry

Describes the arrangement of the **atoms**.

This distinction becomes very important when lone pairs are present.

## Example: NH₃

Nitrogen has:

``` text
3 bonds
1 lone pair
```

Therefore:

``` text
4 electron domains
```

Electron-domain geometry:

``` text
Tetrahedral
```

But the molecular geometry is:

``` text
Trigonal pyramidal
```

because the lone pair is not an atom.

## Example: H₂O

Oxygen has:

``` text
2 bonds
2 lone pairs
```

Electron-domain geometry:

``` text
Tetrahedral
```

Molecular geometry:

``` text
Bent
```

### Layer 2 → Problems

**Question:** What is the electron-domain geometry of NH₃?

**Answer:** Tetrahedral.

**Question:** What is its molecular geometry?

**Answer:** Trigonal pyramidal.

**Question:** What is the electron-domain geometry of H₂O?

**Answer:** Tetrahedral.

**Question:** What is its molecular geometry?

**Answer:** Bent.

### Layer 3 → Cheminformatics Connection

This distinction helps explain why simply knowing connectivity does not
fully describe a molecule's 3D shape.

A molecular graph:

``` text
O
|
H
|
H
```

does not directly tell you the final spatial coordinates.

Geometry must be generated or calculated.

------------------------------------------------------------------------

# 5. Linear Geometry

## Layer 1 → Concept

A molecule is **linear** when the relevant atoms lie approximately along
a straight line.

Typical VSEPR arrangement:

``` text
2 electron domains
```

Ideal bond angle:

``` text
180°
```

### Example: CO₂

``` text
O=C=O
```

Carbon has two electron domains.

Therefore:

``` text
Electron-domain geometry → Linear
Molecular geometry       → Linear
Bond angle               → 180°
```

### Layer 2 → Problems

**Question:** What is the ideal bond angle for a linear molecule?

**Answer:** 180°.

**Question:** What is the geometry of CO₂ around carbon?

**Answer:** Linear.

### Layer 3 → Cheminformatics Connection

Linear arrangements are represented using 3D coordinates.

For a simplified geometry:

``` text
O —— C —— O
```

the atoms can be placed approximately along one axis.

3D software stores this numerically rather than as a drawing.

------------------------------------------------------------------------

# 6. Trigonal Planar Geometry

## Layer 1 → Concept

A central atom with:

``` text
3 electron domains
```

generally has a **trigonal planar** electron-domain arrangement.

The three domains lie approximately in one plane.

Ideal bond angle:

``` text
120°
```

Visual idea:

``` text
      A
     /
    X
   / \
  B   C
```

All three surrounding atoms are approximately in the same plane.

### Example: BF₃

``` text
      F
     /
F—B
     \
      F
```

The ideal F---B---F angle is approximately:

``` text
120°
```

### Layer 2 → Problems

**Question:** How many electron domains produce trigonal planar
geometry?

**Answer:** 3.

**Question:** What is the ideal bond angle?

**Answer:** 120°.

### Layer 3 → Cheminformatics Connection

Trigonal planar centers occur frequently in:

-   Carbonyl groups
-   Alkenes
-   Aromatic systems
-   Many sp²-hybridized centers

These structural patterns are important for:

-   Substructure searching
-   Molecular descriptors
-   Conformer generation
-   Reaction informatics

------------------------------------------------------------------------

# 7. Tetrahedral Geometry

## Layer 1 → Concept

A central atom with:

``` text
4 electron domains
```

generally has a **tetrahedral electron-domain geometry**.

Ideal bond angle:

``` text
109.5°
```

Example:

``` text
       H
       |
   H — C — H
      /
     H
```

The drawing is only a 2D representation of a 3D arrangement.

Methane, CH₄, is tetrahedral.

### Layer 2 → Problems

**Question:** How many electron domains correspond to tetrahedral
geometry?

**Answer:** 4.

**Question:** What is the ideal tetrahedral bond angle?

**Answer:** Approximately 109.5°.

### Layer 3 → Cheminformatics Connection

Tetrahedral carbon is extremely important in organic and medicinal
chemistry.

It is also important for **stereochemistry**.

A carbon with four different substituents can be a stereocenter:

``` text
       A
       |
B — C — D
       \
        E
```

The exact 3D arrangement matters.

Later you will encounter:

-   R/S configuration
-   Chirality
-   Stereochemical SMILES
-   Isomeric SMILES
-   3D conformers

------------------------------------------------------------------------

# 8. Trigonal Pyramidal Geometry

## Layer 1 → Concept

A central atom with:

``` text
4 electron domains
```

where:

``` text
3 = bonding domains
1 = lone pair
```

has:

``` text
Electron-domain geometry → Tetrahedral
Molecular geometry       → Trigonal pyramidal
```

Example:

``` text
      ..
      N
    / | \
   H  H  H
```

NH₃ is the classic example.

The H---N---H bond angle is approximately:

``` text
107°
```

It is smaller than the ideal tetrahedral angle because the lone pair
occupies more space than a bonding pair.

### Layer 2 → Problems

**Question:** What is the electron-domain geometry of NH₃?

**Answer:** Tetrahedral.

**Question:** What is the molecular geometry?

**Answer:** Trigonal pyramidal.

**Question:** Why is the bond angle smaller than 109.5°?

**Answer:** Lone-pair repulsion is stronger than bonding-pair repulsion,
compressing the bond angles.

### Layer 3 → Cheminformatics Connection

Nitrogen geometry matters greatly in:

-   Amines
-   Amides
-   Heterocycles
-   Drug molecules
-   Protein--ligand interactions

The local geometry of nitrogen can affect molecular shape and
recognition.

------------------------------------------------------------------------

# 9. Bent Geometry

## Layer 1 → Concept

A molecule is **bent** when the central atom has two bonded atoms but
lone pairs cause the bonds to angle rather than form a straight line.

Water is the classic example.

``` text
   ..
H— O
   \
    H
   ..
```

Oxygen has:

``` text
2 bonding domains
2 lone-pair domains
```

Total:

``` text
4 electron domains
```

Therefore:

``` text
Electron-domain geometry → Tetrahedral
Molecular geometry       → Bent
```

The H---O---H bond angle is approximately:

``` text
104.5°
```

### Layer 2 → Problems

**Question:** What is the molecular geometry of H₂O?

**Answer:** Bent.

**Question:** What is its electron-domain geometry?

**Answer:** Tetrahedral.

**Question:** Why isn't water linear?

**Answer:** The two lone pairs on oxygen repel the bonding pairs and
produce a bent arrangement.

### Layer 3 → Cheminformatics Connection

Water demonstrates a critical idea:

``` text
Connectivity alone
      ≠
3D geometry
```

The molecular graph says:

``` text
H—O—H
```

but the actual 3D molecule is bent.

This distinction becomes important when studying:

-   Molecular dynamics
-   Docking
-   3D descriptors
-   Quantum chemistry
-   Hydrogen bonding

------------------------------------------------------------------------

# 10. Trigonal Bipyramidal Geometry

## Layer 1 → Concept

A central atom with:

``` text
5 electron domains
```

has a **trigonal bipyramidal** electron-domain geometry.

There are:

``` text
3 equatorial positions
2 axial positions
```

Ideal angles include:

``` text
Equatorial–equatorial → 120°
Axial–equatorial      → 90°
Axial–axial           → 180°
```

Conceptually:

``` text
       Axial
         |
         X
      /  |  \
     A   B   C
         |
         D
       Axial
```

The exact drawing is only a simplified representation.

### Layer 2 → Problems

**Question:** How many electron domains produce trigonal bipyramidal
geometry?

**Answer:** 5.

**Question:** What is the axial--equatorial angle?

**Answer:** 90°.

**Question:** What is the equatorial--equatorial angle?

**Answer:** 120°.

### Layer 3 → Cheminformatics Connection

Five-coordinate geometries become relevant in:

-   Hypervalent compounds
-   Coordination chemistry
-   Inorganic chemistry
-   Some transition-metal complexes

They are less common in ordinary small organic drug molecules but
important for broader chemical informatics.

------------------------------------------------------------------------

# 11. Octahedral Geometry

## Layer 1 → Concept

A central atom with:

``` text
6 electron domains
```

generally has an **octahedral** electron-domain geometry.

Ideal angles:

``` text
Adjacent positions → 90°
Opposite positions → 180°
```

Conceptually:

``` text
        A
        |
        X
      / | \
     B  C  D
        |
        E
```

with another position along the opposite axis.

### Layer 2 → Problems

**Question:** How many electron domains produce octahedral geometry?

**Answer:** 6.

**Question:** What are the common ideal bond angles?

**Answer:** 90° and 180°.

### Layer 3 → Cheminformatics Connection

Octahedral geometry is particularly important in:

-   Coordination chemistry
-   Metal complexes
-   Inorganic compounds
-   Bioinorganic chemistry

Metal-containing compounds require more sophisticated representations
than many ordinary organic molecules.

------------------------------------------------------------------------

# 12. Lone Pairs and Bond Angles

## Layer 1 → Concept

Not all electron domains repel equally.

A useful qualitative order is:

``` text
Lone pair–lone pair
        >
Lone pair–bonding pair
        >
Bonding pair–bonding pair
```

Therefore lone pairs tend to occupy more space and compress bond angles.

Compare:

``` text
CH₄ → 109.5°
NH₃ → ~107°
H₂O → ~104.5°
```

Why?

``` text
CH₄
4 bonding domains
↓
No lone pairs
↓
109.5°
```

``` text
NH₃
3 bonding + 1 lone pair
↓
Angle compressed
↓
~107°
```

``` text
H₂O
2 bonding + 2 lone pairs
↓
More compression
↓
~104.5°
```

### Layer 2 → Problems

Put these in decreasing approximate bond angle:

``` text
CH₄
NH₃
H₂O
```

Answer:

``` text
CH₄ > NH₃ > H₂O
```

### Layer 3 → Cheminformatics Connection

Local geometry affects:

-   Steric accessibility
-   Hydrogen bonding
-   Molecular recognition
-   Conformation
-   3D similarity

This is one reason molecular modeling cannot treat every atom as a
simple point connected by lines.

------------------------------------------------------------------------

# 13. Molecular Polarity

## Layer 1 → Concept

Molecular polarity depends on both:

``` text
Bond polarity
+
Molecular geometry
```

A molecule can contain polar bonds but still be nonpolar overall if the
bond dipoles cancel.

## Example: CO₂

C=O bonds are polar.

But:

``` text
O=C=O
```

is linear.

The dipoles cancel:

``` text
← dipole    dipole →
```

Therefore:

``` text
Overall molecule → nonpolar
```

## Example: H₂O

O---H bonds are polar.

Water is bent:

``` text
  H
   \
    O
   /
  H
```

The dipoles do not cancel.

Therefore:

``` text
Overall molecule → polar
```

### Layer 2 → Problems

**Question:** Is CO₂ polar overall?

**Answer:** No.

**Question:** Is H₂O polar overall?

**Answer:** Yes.

**Question:** What two factors should you consider?

**Answer:**

1.  Bond polarity
2.  Molecular geometry

### Layer 3 → Cheminformatics Connection

Polarity is important for predicting:

-   Solubility
-   Membrane permeability
-   Protein binding
-   Hydrogen bonding
-   Molecular recognition

Many cheminformatics descriptors attempt to capture aspects of molecular
polarity.

------------------------------------------------------------------------

# 14. Molecular Dipole Moment

## Layer 1 → Concept

A **dipole moment** describes separation of positive and negative charge
in a molecule.

It has both:

``` text
Magnitude
+
Direction
```

For a molecule:

``` text
Total dipole
=
vector combination of individual bond dipoles
```

This explains why geometry matters.

For example:

``` text
CO₂

O ← C → O
```

The two bond dipoles cancel.

Water:

``` text
   O
  ↙ ↘
 H   H
```

The dipoles add to produce a net molecular dipole.

### Layer 2 → Problems

**Question:** Why can two polar bonds produce a nonpolar molecule?

**Answer:** Their dipoles can cancel because of molecular geometry.

**Question:** Why does water have a net dipole?

**Answer:** Its bent geometry prevents the two O---H bond dipoles from
canceling.

### Layer 3 → Cheminformatics Connection

Dipole-related properties influence:

-   Molecular interactions
-   Solvation
-   Protein binding
-   Electrostatic complementarity

More advanced computational chemistry can calculate charge distributions
and molecular electrostatic properties.

------------------------------------------------------------------------

# 15. Molecular Geometry and Hybridization --- Introductory Connection

You will encounter **hybridization** in organic chemistry.

For now, learn the common simplified relationships:

``` text
2 electron domains → sp
3 electron domains → sp²
4 electron domains → sp³
```

Common geometries:

``` text
sp   → linear
sp²  → trigonal planar
sp³  → tetrahedral
```

Examples:

``` text
CO₂ carbon → sp → linear
BF₃ boron  → sp² → trigonal planar
CH₄ carbon → sp³ → tetrahedral
```

This is an introductory model and should not be treated as a complete
description of modern electronic structure.

### Layer 2 → Problems

Identify the simplified hybridization:

**CO₂ carbon**

``` text
2 domains
→ sp
```

**BF₃ boron**

``` text
3 domains
→ sp²
```

**CH₄ carbon**

``` text
4 domains
→ sp³
```

### Layer 3 → Cheminformatics Connection

Hybridization can be stored or inferred by cheminformatics toolkits.

It is useful for identifying local structural environments and
calculating molecular descriptors.

------------------------------------------------------------------------

# 16. Molecular Geometry and Stereochemistry

## Layer 1 → Concept

A molecule's 3D arrangement can create **stereoisomers**.

Two molecules may have:

``` text
Same atoms
+
Same connectivity
```

but different 3D arrangements.

This is a major concept in medicinal chemistry.

A tetrahedral carbon attached to four different groups can be
**chiral**.

The two possible configurations can be related as mirror images.

``` text
      A
      |
B — C — D
      \
       E
```

The actual 3D arrangement determines stereochemical identity.

### Layer 2 → Problems

**Question:** Can two molecules have the same connectivity but different
3D arrangements?

**Answer:** Yes.

**Question:** Why does this matter in drug discovery?

**Answer:** Different stereoisomers can have different biological
interactions and activities.

### Layer 3 → Cheminformatics Connection

Cheminformatics must represent stereochemistry explicitly.

You will later encounter:

-   Chiral centers
-   R/S configuration
-   E/Z configuration
-   Stereochemical SMILES
-   Isomeric SMILES
-   Stereochemical descriptors

For example, two SMILES strings can represent different stereochemical
forms even when their basic connectivity is the same.

------------------------------------------------------------------------

# 17. 2D Molecular Structure vs 3D Molecular Structure

## Layer 1 → Concept

A 2D structure mainly communicates:

``` text
Which atoms are connected?
What are the bond orders?
```

A 3D structure additionally communicates:

``` text
Where are the atoms in space?
```

Compare:

``` text
2D

H—O—H
```

with:

``` text
3D

      H
       \
        O
       /
      H
```

The second representation communicates the bent geometry.

### Layer 2 → Problems

**Question:** What information does a 2D molecular graph primarily
capture?

**Answer:** Atom connectivity and bond information.

**Question:** What additional information does a 3D structure contain?

**Answer:** Spatial coordinates and molecular geometry.

### Layer 3 → Cheminformatics Connection

This distinction is fundamental.

## 2D representation

Often used for:

-   SMILES
-   Molecular graphs
-   Fingerprints
-   Substructure searching

## 3D representation

Used for:

-   Docking
-   Molecular dynamics
-   3D similarity
-   Conformer analysis
-   Quantum chemistry
-   Structure-based drug discovery

------------------------------------------------------------------------

# 18. Molecular Conformation

## Layer 1 → Concept

A molecule can sometimes adopt different spatial arrangements without
breaking covalent bonds.

These different arrangements are called **conformations**.

For example, rotation around a single bond can produce different
conformations:

``` text
C—C
```

The atoms can rotate around the C---C bond.

This produces different spatial arrangements.

Important distinction:

``` text
Conformation
→ changes by bond rotation without changing connectivity

Configuration
→ stereochemical arrangement that generally requires bond breaking to interconvert
```

You will study this more deeply later.

### Layer 2 → Problems

**Question:** Can a molecule have multiple conformations?

**Answer:** Yes.

**Question:** Does changing conformation necessarily break covalent
bonds?

**Answer:** No.

### Layer 3 → Cheminformatics Connection

Conformers are extremely important in:

-   Molecular docking
-   Molecular dynamics
-   3D similarity
-   Binding-pose prediction
-   Molecular mechanics

A cheminformatics workflow may generate many conformers for the same
molecule:

``` text
Molecule
   ↓
Conformer generation
   ↓
3D structure 1
3D structure 2
3D structure 3
...
```

------------------------------------------------------------------------

# 19. Geometry → Molecular Properties

The major chain to remember is:

``` text
Electron distribution
        ↓
Bonding
        ↓
Molecular geometry
        ↓
Charge distribution
        ↓
Polarity
        ↓
Intermolecular interactions
        ↓
Physical / biological properties
```

For example:

``` text
H₂O

O—H bonds
    ↓
Polar bonds
    ↓
Bent geometry
    ↓
Dipoles do not cancel
    ↓
Polar molecule
    ↓
Strong interactions with other polar species
```

This is the kind of chemistry reasoning you will repeatedly use in
cheminformatics.

------------------------------------------------------------------------

# 20. Geometry Summary Table

  Electron Domains   Electron-Domain Geometry   Typical Ideal Angles
  ------------------ -------------------------- ----------------------
  2                  Linear                     180°
  3                  Trigonal planar            120°
  4                  Tetrahedral                109.5°
  5                  Trigonal bipyramidal       90°, 120°, 180°
  6                  Octahedral                 90°, 180°

Remember:

``` text
Electron-domain geometry
≠ always molecular geometry
```

because lone pairs are included in electron-domain geometry but not
counted as atoms in molecular geometry.

------------------------------------------------------------------------

# 21. Common Molecule Examples

  -------------------------------------------------------------------------
  Molecule              Electron Domains Electron-Domain   Molecular
                                         Geometry          Geometry
  ---------------- --------------------- ----------------- ----------------
  CO₂                                  2 Linear            Linear

  BF₃                                  3 Trigonal planar   Trigonal planar

  CH₄                                  4 Tetrahedral       Tetrahedral

  NH₃                                  4 Tetrahedral       Trigonal
                                                           pyramidal

  H₂O                                  4 Tetrahedral       Bent

  PCl₅                                 5 Trigonal          Trigonal
                                         bipyramidal       bipyramidal

  SF₆                                  6 Octahedral        Octahedral
  -------------------------------------------------------------------------

These examples are worth memorizing.

------------------------------------------------------------------------

# 22. Practice --- Basic

Try these before checking the answers.

### Question 1

What does VSEPR stand for?

### Question 2

What is the central idea of VSEPR theory?

### Question 3

How many electron domains does a double bond count as?

### Question 4

What is the ideal bond angle for linear geometry?

### Question 5

What is the ideal bond angle for trigonal planar geometry?

### Question 6

What is the ideal bond angle for tetrahedral geometry?

### Question 7

What is the molecular geometry of CH₄?

### Question 8

What is the molecular geometry of NH₃?

### Question 9

What is the molecular geometry of H₂O?

### Question 10

What are the two main factors determining molecular polarity?

------------------------------------------------------------------------

# 23. Answers --- Basic

### 1

Valence Shell Electron Pair Repulsion.

### 2

Electron groups around a central atom repel one another and arrange
themselves as far apart as possible.

### 3

One electron domain.

### 4

180°.

### 5

120°.

### 6

109.5°.

### 7

Tetrahedral.

### 8

Trigonal pyramidal.

### 9

Bent.

### 10

Bond polarity and molecular geometry.

------------------------------------------------------------------------

# 24. Practice --- Intermediate

### Question 1

Determine the electron-domain geometry and molecular geometry of NH₃.

### Question 2

Determine the electron-domain geometry and molecular geometry of H₂O.

### Question 3

Why is the H---O---H angle smaller than the H---C---H angle in CH₄?

### Question 4

Why is CO₂ nonpolar even though its C=O bonds are polar?

### Question 5

Why is H₂O polar?

### Question 6

How many electron domains are around carbon in CO₂?

### Question 7

How many electron domains are around carbon in CH₄?

### Question 8

What is the difference between electron-domain geometry and molecular
geometry?

### Question 9

What is the relationship between molecular geometry and 3D molecular
representation?

### Question 10

Why is stereochemistry important in cheminformatics?

------------------------------------------------------------------------

# 25. Answers --- Intermediate

### 1

NH₃:

``` text
3 bonds + 1 lone pair
→ 4 domains
→ tetrahedral electron-domain geometry
→ trigonal pyramidal molecular geometry
```

### 2

H₂O:

``` text
2 bonds + 2 lone pairs
→ 4 domains
→ tetrahedral electron-domain geometry
→ bent molecular geometry
```

### 3

Oxygen has two lone pairs, while carbon in CH₄ has no lone pairs. Lone
pairs repel more strongly and compress the bond angle.

### 4

CO₂ is linear, so the two C=O bond dipoles cancel.

### 5

Water has polar O---H bonds and bent geometry, so its bond dipoles do
not cancel.

### 6

2 electron domains.

### 7

4 electron domains.

### 8

Electron-domain geometry considers both bonding pairs and lone pairs.
Molecular geometry describes the arrangement of atoms.

### 9

Molecular geometry determines how atoms are positioned in 3D space,
which is represented computationally using coordinates.

### 10

Different 3D arrangements can produce different stereoisomers, which can
have different chemical and biological behavior.

------------------------------------------------------------------------

# 26. Cheminformatics Mini-Exercise

Consider three molecules:

``` text
CO₂
NH₃
H₂O
```

## Step 1 --- Identify electron domains

``` text
CO₂ → 2
NH₃ → 4
H₂O → 4
```

## Step 2 --- Determine geometry

``` text
CO₂
→ linear

NH₃
→ trigonal pyramidal

H₂O
→ bent
```

## Step 3 --- Consider polarity

``` text
CO₂
→ polar bonds
→ linear
→ dipoles cancel
→ nonpolar overall

NH₃
→ polar N—H bonds
→ trigonal pyramidal
→ polar overall

H₂O
→ polar O—H bonds
→ bent
→ polar overall
```

## Step 4 --- Think computationally

A cheminformatics system needs to distinguish:

``` text
Connectivity
+
Bond order
+
Charge
+
Geometry
+
3D coordinates
```

This is the beginning of understanding **3D molecular informatics**.

------------------------------------------------------------------------

# 27. Important Relationships to Memorize

## VSEPR

``` text
Electron domains repel
        ↓
Maximum separation
        ↓
Predict geometry
```

## Electron domains

``` text
Single bond → 1
Double bond → 1
Triple bond → 1
Lone pair   → 1
```

## Main geometries

``` text
2 → Linear → 180°

3 → Trigonal planar → 120°

4 → Tetrahedral → 109.5°

5 → Trigonal bipyramidal
    → 90°, 120°, 180°

6 → Octahedral
    → 90°, 180°
```

## Lone pairs

``` text
Lone pair repulsion
>
Bonding pair repulsion
```

Therefore:

``` text
CH₄ → ~109.5°
NH₃ → ~107°
H₂O → ~104.5°
```

## Polarity

``` text
Bond polarity
+
Geometry
↓
Molecular polarity
```

## Cheminformatics

``` text
2D graph
   ↓
Atoms + bonds + connectivity
   ↓
3D structure
   ↓
Coordinates
   ↓
Conformations
   ↓
Molecular interactions
```

------------------------------------------------------------------------

# 28. Mastery Checklist

Before moving to **1.6 Chemical Formulas & Nomenclature**, make sure you
can:

## Molecular Geometry

-   [ ] Explain why molecular geometry matters
-   [ ] Explain VSEPR
-   [ ] Identify electron domains
-   [ ] Distinguish electron-domain geometry from molecular geometry
-   [ ] Recognize linear geometry
-   [ ] Recognize trigonal planar geometry
-   [ ] Recognize tetrahedral geometry
-   [ ] Recognize trigonal pyramidal geometry
-   [ ] Recognize bent geometry
-   [ ] Recognize trigonal bipyramidal geometry
-   [ ] Recognize octahedral geometry
-   [ ] Know common ideal bond angles
-   [ ] Explain lone-pair repulsion
-   [ ] Predict basic molecular polarity
-   [ ] Understand the relationship between geometry and dipole moment
-   [ ] Understand the basic idea of hybridization
-   [ ] Understand the difference between 2D and 3D molecular
    representations
-   [ ] Understand the basic difference between conformation and
    configuration
-   [ ] Understand why stereochemistry matters

## Cheminformatics

You should understand:

``` text
Molecular graph
      ↓
Connectivity
      ↓
Local geometry
      ↓
3D coordinates
      ↓
Conformations
      ↓
3D molecular behavior
```

------------------------------------------------------------------------

# 29. Final Mastery Test

Try these without notes.

### 1.

What does VSEPR stand for?

### 2.

What is an electron domain?

### 3.

How many electron domains does a triple bond represent?

### 4.

What is the electron-domain geometry for four electron domains?

### 5.

What is the molecular geometry of NH₃?

### 6.

What is the molecular geometry of H₂O?

### 7.

Why are NH₃ and H₂O not tetrahedral in molecular geometry even though
both have four electron domains?

### 8.

What is the ideal bond angle of trigonal planar geometry?

### 9.

What is the ideal bond angle of tetrahedral geometry?

### 10.

Why is H₂O polar?

### 11.

Why is CO₂ nonpolar overall?

### 12.

What is the difference between electron-domain geometry and molecular
geometry?

### 13.

What is the difference between a 2D molecular graph and a 3D molecular
structure?

### 14.

What is a conformer?

### 15.

Why is molecular geometry important for drug discovery?

------------------------------------------------------------------------

# 30. Final Answers

### 1

Valence Shell Electron Pair Repulsion.

### 2

A region of electron density around a central atom; in basic VSEPR, each
bond or lone pair counts as one domain.

### 3

One electron domain.

### 4

Tetrahedral.

### 5

Trigonal pyramidal.

### 6

Bent.

### 7

Because molecular geometry counts the arrangement of atoms, while
electron-domain geometry also includes lone pairs.

### 8

120°.

### 9

109.5°.

### 10

It has polar O---H bonds and a bent geometry, so the dipoles do not
cancel.

### 11

Its two polar C=O bonds are arranged linearly and their dipoles cancel.

### 12

Electron-domain geometry includes bonding pairs and lone pairs.
Molecular geometry describes the arrangement of the atoms.

### 13

A 2D graph primarily represents connectivity and bond information. A 3D
structure additionally represents the spatial positions of atoms.

### 14

A conformer is one of the different spatial arrangements a molecule can
adopt without changing its covalent connectivity, commonly through bond
rotation.

### 15

Because 3D shape affects molecular interactions, binding,
stereochemistry, conformation, and biological activity.

------------------------------------------------------------------------

# 31. One-Page Memory Sheet

## VSEPR

``` text
Electron groups repel
        ↓
Spread apart
        ↓
Determine geometry
```

## Geometry

``` text
2 domains
→ Linear
→ 180°

3 domains
→ Trigonal planar
→ 120°

4 domains
→ Tetrahedral
→ 109.5°

5 domains
→ Trigonal bipyramidal
→ 90° / 120° / 180°

6 domains
→ Octahedral
→ 90° / 180°
```

## Important Examples

``` text
CO₂ → Linear

BF₃ → Trigonal planar

CH₄ → Tetrahedral

NH₃ → Trigonal pyramidal

H₂O → Bent
```

## Lone Pairs

``` text
More lone pairs
      ↓
More repulsion
      ↓
Smaller bond angles
```

## Polarity

``` text
Polar bonds
+
Geometry
↓
Molecular polarity
```

## Cheminformatics

``` text
Atoms
 ↓
Bonds
 ↓
2D molecular graph
 ↓
3D coordinates
 ↓
Conformations
 ↓
Molecular interactions
```

------------------------------------------------------------------------

# 32. Sources

-   OpenStax, **Chemistry 2e --- Molecular Geometry and Polarity**:
    https://openstax.org/books/chemistry-2e/pages/7-6-molecular-structure-and-polarity
-   Chemistry LibreTexts, **VSEPR Theory**:
    https://chem.libretexts.org/Bookshelves/General_Chemistry/Map%3A_Chemistry\_-*The_Molecular_Science*%28Moore_et_al.%29/06%3A_Chemical_Bonding_and_Molecular_Geometry/6.04%3A_VSEPR_Theory
-   IUPAC Gold Book, **Molecular geometry / chemical terminology**:
    https://goldbook.iupac.org/

> **Study note:** The geometry and angle values in this lesson are
> introductory VSEPR idealizations. Real molecular geometries can
> deviate from ideal angles, and computational chemistry provides more
> accurate structures.
