# Chemistry --- Pillar 1

# 1.1 Matter & Basic Concepts

> **Goal:** Rebuild the basic chemistry foundation needed for a
> Chemoinformatics program.

This lesson follows three layers:

1.  **Layer 1 → Concept:** understand what it means.
2.  **Layer 2 → Problems:** solve basic → intermediate questions.
3.  **Layer 3 → Cheminformatics connection:** understand how the
    chemistry appears later in computational chemistry and
    cheminformatics.

------------------------------------------------------------------------

## 1. Matter

### Layer 1 → Concept

**Matter is anything that has mass and occupies space.**

Examples:

-   Water
-   Oxygen
-   Carbon dioxide
-   Salt
-   Air
-   A drug molecule
-   Proteins
-   Your computer

Examples that are not matter:

-   Light
-   Sound
-   Heat
-   Mathematical numbers

At the microscopic level, matter is made of **atoms and molecules**.

For example:

``` text
Water
  ↓
H₂O
  ↓
2 Hydrogen atoms + 1 Oxygen atom
```

A molecule is a specific arrangement of atoms connected by chemical
bonds.

### Layer 2 → Problems

**Problem 1**

Is oxygen matter?

**Answer:** Yes. It has mass and occupies space.

**Problem 2**

Is light matter?

**Answer:** No. Light is energy/electromagnetic radiation, not matter.

**Problem 3**

Is a drug molecule matter?

**Answer:** Yes. It has mass and occupies space.

### Layer 3 → Cheminformatics Connection

Chemoinformatics works with chemical matter at the molecular level.

The basic progression is:

``` text
Real substance
     ↓
Molecules
     ↓
Atoms + bonds
     ↓
Molecular structure
     ↓
Computer representation
     ↓
Descriptors / fingerprints
     ↓
Machine learning
```

A molecule can eventually be represented computationally as a
**molecular graph**:

``` text
H — O — H

Nodes → atoms
Edges → bonds
```

This graph concept becomes important for:

-   Molecular fingerprints
-   Molecular similarity
-   Molecular descriptors
-   Graph neural networks
-   QSAR

------------------------------------------------------------------------

# 2. States of Matter

### Layer 1 → Concept

The three classical states of matter are:

-   Solid
-   Liquid
-   Gas

Plasma is another state of matter, but the first three are the main
foundation for general chemistry.

### Solid

Particles are closely packed and mainly vibrate around fixed positions.

``` text
● ● ● ●
● ● ● ●
● ● ● ●
```

Characteristics:

-   Fixed shape
-   Fixed volume
-   Particles are closely packed
-   Relatively strong intermolecular interactions

### Liquid

Particles remain relatively close but can move past each other.

``` text
● ●   ●
  ● ●
●    ● ●
```

Characteristics:

-   Fixed volume
-   No fixed shape
-   Takes the shape of its container
-   Can flow

### Gas

Particles are far apart and move freely.

``` text
●          ●

      ●

             ●       ●
```

Characteristics:

-   No fixed shape
-   No fixed volume
-   Highly compressible
-   Particles move freely

### Why do states differ?

The behavior of matter depends on factors including:

-   Particle motion
-   Temperature
-   Intermolecular forces
-   Energy

A simplified sequence is:

``` text
Solid → Liquid → Gas
```

when thermal energy increases enough to overcome intermolecular
interactions.

### Layer 2 → Problems

**Problem 1**

Which state has a fixed volume but no fixed shape?

**Answer:** Liquid.

**Problem 2**

Which state is most easily compressed?

**Answer:** Gas.

**Problem 3**

When liquid water becomes water vapor, has the chemical identity of
water changed?

**Answer:** No. It is still H₂O.

### Layer 3 → Cheminformatics Connection

Cheminformatics usually focuses heavily on molecular structure, but the
physical state of a substance can matter when interpreting experimental
chemical data.

For example:

``` text
Molecule
   ↓
Physical properties
   ↓
Solubility
Melting point
Boiling point
Vapor pressure
```

These properties can appear as targets in chemical databases and
machine-learning datasets.

------------------------------------------------------------------------

# 3. Elements

### Layer 1 → Concept

An **element** is a pure substance consisting of atoms with the same
number of protons.

The number of protons is the **atomic number**.

Examples:

``` text
Hydrogen → 1 proton
Carbon   → 6 protons
Nitrogen → 7 protons
Oxygen   → 8 protons
Chlorine → 17 protons
```

Therefore:

``` text
Atomic number = Number of protons
```

An element cannot be converted into another element by ordinary chemical
reactions because chemical reactions do not change the nucleus.

### Layer 2 → Problems

**Problem 1**

An atom has 8 protons. What element is it?

**Answer:** Oxygen.

**Problem 2**

An atom has 17 protons. What element is it?

**Answer:** Chlorine.

**Problem 3**

Can changing the number of electrons turn carbon into oxygen?

**Answer:** No.

Carbon has 6 protons. Oxygen has 8 protons.

Changing electrons changes the charge, not the elemental identity.

### Layer 3 → Cheminformatics Connection

A computer must distinguish different atom types:

``` text
C ≠ N ≠ O ≠ S ≠ Cl
```

Atomic identity affects:

-   Molecular weight
-   Valence
-   Bonding
-   Polarity
-   Hydrogen bonding
-   Reactivity
-   Molecular descriptors

When working with molecular structures in software such as RDKit, each
atom has an elemental identity represented computationally.

------------------------------------------------------------------------

# 4. Compounds

### Layer 1 → Concept

A **compound** is a substance made from two or more different elements
chemically bonded together in a definite ratio.

Examples:

### Water

``` text
H₂O
```

Contains:

-   Hydrogen
-   Oxygen

### Carbon dioxide

``` text
CO₂
```

Contains:

-   Carbon
-   Oxygen

### Sodium chloride

``` text
NaCl
```

Contains:

-   Sodium
-   Chlorine

The important distinction is:

``` text
Element
  ↓
one type of atom

Compound
  ↓
different elements
chemically bonded
```

### Layer 2 → Problems

**Problem 1**

Is O₂ an element or compound?

**Answer:** Element.

It contains only oxygen atoms.

**Problem 2**

Is H₂O an element or compound?

**Answer:** Compound.

It contains hydrogen and oxygen.

**Problem 3**

Is CO₂ a compound?

**Answer:** Yes.

Carbon and oxygen are chemically bonded in a fixed ratio.

### Layer 3 → Cheminformatics Connection

A chemical database may store a compound as:

``` text
Molecular structure
      ↓
Atoms
      +
Bonds
      ↓
Molecular graph
```

From that representation, software can calculate:

-   Molecular formula
-   Molecular weight
-   Hydrogen-bond donors
-   Hydrogen-bond acceptors
-   Topological polar surface area
-   LogP
-   Fingerprints

------------------------------------------------------------------------

# 5. Mixtures

### Layer 1 → Concept

A **mixture** contains two or more substances that are physically
combined rather than chemically bonded into a new compound.

Examples:

-   Air
-   Salt water
-   Seawater
-   Soil
-   Tea

For example:

``` text
Salt water
    ↓
H₂O + NaCl
```

The water and salt retain their chemical identities.

Compare:

``` text
Compound:
H₂ + O₂ → H₂O
        chemical reaction

Mixture:
H₂O + NaCl
        physical combination
```

## Homogeneous Mixture

A homogeneous mixture is uniform throughout.

Example:

``` text
Salt dissolved in water
```

## Heterogeneous Mixture

A heterogeneous mixture is not uniform throughout.

Example:

``` text
Sand + water
```

### Layer 2 → Problems

**Problem 1**

Is air an element, compound, or mixture?

**Answer:** Mixture.

Air contains several gases.

**Problem 2**

Is pure H₂O a mixture?

**Answer:** No. Pure H₂O is a compound.

**Problem 3**

Is salt water a mixture?

**Answer:** Yes.

### Layer 3 → Cheminformatics Connection

Chemical records can contain multiple components, such as:

``` text
Drug molecule
+
Counterion
+
Solvent
+
Other components
```

This becomes important when cleaning chemical datasets.

Later you will encounter:

-   Salts
-   Counterions
-   Fragments
-   Solvents
-   Multicomponent records
-   Structure standardization

A cheminformatics pipeline may need to decide whether a database record
represents one molecular entity or multiple components.

------------------------------------------------------------------------

# 6. Physical Properties

### Layer 1 → Concept

A **physical property** can be observed or measured without changing the
chemical identity of a substance.

Examples:

-   Color
-   Density
-   Melting point
-   Boiling point
-   Solubility
-   Electrical conductivity
-   Molecular mass

For example:

``` text
Water boiling point ≈ 100°C
```

Measuring its boiling point does not change water into a different
chemical substance.

### Layer 2 → Problems

Classify each as physical or chemical:

**1. Melting point**

Answer: **Physical**

**2. Density**

Answer: **Physical**

**3. Solubility**

Answer: **Physical**

**4. Color**

Answer: **Physical**

**5. Boiling point**

Answer: **Physical**

### Layer 3 → Cheminformatics Connection

Many molecular properties are used as inputs or prediction targets.

For example:

``` text
Molecular structure
       ↓
Descriptors
       ↓
Property prediction
       ↓
Solubility / LogP / Melting point / etc.
```

This is related to **QSPR --- Quantitative Structure--Property
Relationships**.

------------------------------------------------------------------------

# 7. Chemical Properties

### Layer 1 → Concept

A **chemical property** describes how a substance behaves when it
undergoes a chemical reaction or chemical transformation.

Examples:

-   Flammability
-   Reactivity with oxygen
-   Reactivity with acids
-   Reactivity with bases
-   Oxidation tendency
-   Chemical stability

The key question is:

> Does the property describe how the substance chemically reacts or
> transforms?

If yes, it is a chemical property.

### Layer 2 → Problems

**1. Flammability**

Answer: **Chemical**

**2. Reactivity with oxygen**

Answer: **Chemical**

**3. Ability to react with an acid**

Answer: **Chemical**

**4. Density**

Answer: **Physical**

### Layer 3 → Cheminformatics Connection

Chemical reactivity is important in:

-   Reaction informatics
-   Drug metabolism
-   Toxicology
-   Retrosynthesis
-   Reaction prediction

A cheminformatics system can represent:

``` text
Reactants
   ↓
Chemical reaction
   ↓
Products
```

------------------------------------------------------------------------

# 8. Physical Changes

### Layer 1 → Concept

A **physical change** changes the form, state, or appearance of a
substance without changing its chemical identity.

Examples:

-   Melting
-   Freezing
-   Evaporation
-   Condensation
-   Cutting
-   Crushing
-   Grinding
-   Dissolving

Example:

``` text
Ice → Water → Steam
```

All are still H₂O.

The molecular identity remains:

``` text
H₂O
```

### Layer 2 → Problems

**1. Ice melting**

Answer: Physical change.

**2. Water boiling**

Answer: Physical change.

**3. Crushing a tablet**

Answer: Physical change.

**4. Cutting paper**

Answer: Physical change.

**5. Water freezing**

Answer: Physical change.

### Layer 3 → Cheminformatics Connection

A physical change does not normally require changing the molecular
connectivity in a molecular structure representation.

For example:

``` text
H₂O(l)
   ↓
H₂O(g)
```

The molecule is still H₂O.

------------------------------------------------------------------------

# 9. Chemical Changes

### Layer 1 → Concept

A **chemical change** produces one or more new chemical substances.

Examples:

``` text
Iron + Oxygen → Iron oxide
```

and

``` text
CH₄ + O₂ → CO₂ + H₂O
```

The original substances have undergone chemical transformations.

Common signs of a chemical change can include:

-   Formation of a new substance
-   Gas formation
-   Precipitate formation
-   Color change associated with reaction
-   Energy change

However, a visible sign alone is not always proof of a chemical
reaction.

### Layer 2 → Problems

Classify:

**1. Iron rusting**

Answer: Chemical change.

**2. Wood burning**

Answer: Chemical change.

**3. Food being digested**

Answer: Chemical change.

**4. Water boiling**

Answer: Physical change.

**5. Sugar caramelizing**

Answer: Chemical change.

### Layer 3 → Cheminformatics Connection

Chemical changes are represented computationally through **chemical
reactions**.

``` text
Reactant structures
       ↓
Reaction transformation
       ↓
Product structures
```

This is the foundation of reaction informatics and is also important
for:

-   Reaction prediction
-   Retrosynthesis
-   Synthesis planning
-   Reaction databases

------------------------------------------------------------------------

# 10. Units and Measurements

### Layer 1 → Concept

Chemistry is quantitative. You will constantly measure and calculate:

-   Mass
-   Volume
-   Temperature
-   Amount of substance
-   Concentration
-   Energy
-   Pressure

Common units:

  Quantity              Common units
  --------------------- ---------------
  Mass                  g, kg, mg
  Volume                L, mL
  Temperature           °C, K
  Amount of substance   mol
  Energy                J, kJ
  Pressure              atm, Pa, mmHg

## Important Conversions

### Mass

``` text
1 kg = 1000 g
1 g = 1000 mg
```

### Volume

``` text
1 L = 1000 mL
```

### Temperature

``` text
K = °C + 273.15
```

Example:

``` text
25°C + 273.15 = 298.15 K
```

### Layer 2 → Problems

**Problem 1**

Convert 2.5 g to mg.

``` text
2.5 g × 1000 mg/g
= 2500 mg
```

**Answer:** 2500 mg.

**Problem 2**

Convert 750 mL to L.

``` text
750 mL × 1 L/1000 mL
= 0.750 L
```

**Answer:** 0.750 L.

**Problem 3**

Convert 27°C to K.

``` text
27 + 273.15
= 300.15 K
```

**Answer:** 300.15 K.

### Layer 3 → Cheminformatics Connection

Chemical datasets contain numerical measurements with units.

For example:

``` text
Compound A
Solubility = 25 mg/L
Temperature = 298 K
Molecular weight = 342.41 g/mol
```

When combining datasets, units must be standardized.

``` text
Different datasets
       ↓
Unit conversion
       ↓
Standardized values
       ↓
Clean dataset
       ↓
ML model
```

Incorrect units can produce incorrect scientific conclusions.

------------------------------------------------------------------------

# 11. Significant Figures

### Layer 1 → Concept

**Significant figures** communicate the precision of a measured value.

Compare:

``` text
5 g
5.0 g
5.00 g
```

These do not communicate the same measurement precision.

## Basic Rules

### Rule 1 --- Non-zero digits are significant

``` text
123
```

has **3 significant figures**.

### Rule 2 --- Zeros between non-zero digits are significant

``` text
1002
```

has **4 significant figures**.

### Rule 3 --- Leading zeros are not significant

``` text
0.0025
```

has **2 significant figures**.

### Rule 4 --- Trailing zeros after a decimal are significant

``` text
2.500
```

has **4 significant figures**.

### Layer 2 → Problems

**Problem 1**

How many significant figures are in:

``` text
0.00450
```

Answer: **3**

Significant digits:

``` text
4, 5, 0
```

**Problem 2**

How many significant figures are in:

``` text
120.0
```

Answer: **4**

**Problem 3**

How many significant figures are in:

``` text
0.00302
```

Answer: **3**

### Layer 3 → Cheminformatics Connection

Chemical datasets often contain experimental measurements.

For example:

``` text
Solubility = 10.0
```

does not necessarily mean the value is known to unlimited precision.

Experimental data contains:

-   Measurement uncertainty
-   Experimental error
-   Precision limits
-   Noise

These become important when doing:

-   Dataset curation
-   Regression
-   Model validation
-   Uncertainty analysis

------------------------------------------------------------------------

# 12. Dimensional Analysis

### Layer 1 → Concept

**Dimensional analysis** uses units as part of the calculation.

It is especially useful for converting units and checking whether a
calculation makes sense.

Example:

Convert 2 kg to grams.

``` text
2 kg × 1000 g
       ─────
        1 kg
```

The kg units cancel:

``` text
2 × 1000 g
= 2000 g
```

The units help guide the calculation.

## Why this matters

Instead of memorizing many conversion formulas, you can construct the
calculation so unwanted units cancel.

### Layer 2 → Problems

**Problem 1**

Convert 5.2 kg to g.

``` text
5.2 kg × 1000 g/kg
= 5200 g
```

**Answer:** 5200 g.

**Problem 2**

Convert 3500 mg to g.

``` text
3500 mg × 1 g/1000 mg
= 3.5 g
```

**Answer:** 3.5 g.

**Problem 3**

Convert 2.5 L to mL.

``` text
2.5 L × 1000 mL/L
= 2500 mL
```

**Answer:** 2500 mL.

## Intermediate Example

A sample has a mass of:

``` text
0.250 g
```

Its molar mass is:

``` text
50.0 g/mol
```

Find the number of moles.

``` text
0.250 g × 1 mol
        ───────
        50.0 g
```

The grams cancel:

``` text
= 0.00500 mol
```

Therefore:

``` text
5.00 × 10⁻³ mol
```

This type of calculation becomes extremely important when we study
**stoichiometry**.

### Layer 3 → Cheminformatics Connection

Dimensional analysis becomes important when processing experimental
chemical data.

A data pipeline might look like:

``` text
Experimental data
       ↓
Check units
       ↓
Convert units
       ↓
Standardize data
       ↓
Build dataset
       ↓
Train ML model
```

A model trained on inconsistent units can learn meaningless
relationships.

------------------------------------------------------------------------

# 13. Physical vs Chemical --- Master This Distinction

This distinction will appear repeatedly throughout chemistry.

  Physical                            Chemical
  ----------------------------------- ---------------------------
  Does not change chemical identity   Changes chemical identity
  Melting                             Burning
  Freezing                            Rusting
  Boiling                             Digestion
  Crushing                            Reaction with acid
  Cutting                             Oxidation
  Evaporation                         Combustion

A useful question is:

> **Did the substance's chemical identity change?**

If **no** → physical change.

If **yes** → chemical change.

------------------------------------------------------------------------

# 14. Element vs Compound vs Mixture

Memorize this comparison:

  Type       What it contains                          Example
  ---------- ----------------------------------------- ------------
  Element    One type of atom                          C
  Compound   Different elements chemically bonded      H₂O
  Mixture    Multiple substances physically combined   Salt water

Think:

``` text
Element
   ↓
same atom type

Compound
   ↓
different atoms
+
chemical bonds

Mixture
   ↓
different substances
+
physical combination
```

------------------------------------------------------------------------

# 15. Cheminformatics Big Picture

Everything in this chapter prepares you for a much larger pipeline.

``` text
                CHEMISTRY
                    |
                    ↓
              Matter
                    |
                    ↓
                 Atoms
                    |
                    ↓
           Elements / Compounds
                    |
                    ↓
            Chemical structure
                    |
                    ↓
             Atoms + Bonds
                    |
                    ↓
          Molecular representation
                    |
        +-----------+-----------+
        |                       |
      SMILES                  SDF/MOL
        |                       |
        +-----------+-----------+
                    ↓
             Molecular graph
                    ↓
        +-----------+-----------+
        |                       |
   Descriptors              Fingerprints
        |                       |
        +-----------+-----------+
                    ↓
              ML / AI models
                    ↓
          Property prediction
          Similarity / QSAR
          Drug discovery
```

The purpose of learning these basic chemistry concepts is not simply to
memorize definitions.

You are building the foundation for understanding **what the chemical
structures that computers manipulate actually mean**.

------------------------------------------------------------------------

# 16. Mastery Checklist

Before moving to **1.2 Atomic Structure**, you should be comfortable
with all of these:

## Concepts

-   [ ] Define matter
-   [ ] Explain the three common states of matter
-   [ ] Explain the difference between solid, liquid, and gas
-   [ ] Define element
-   [ ] Define compound
-   [ ] Define mixture
-   [ ] Distinguish homogeneous and heterogeneous mixtures
-   [ ] Define physical property
-   [ ] Define chemical property
-   [ ] Distinguish physical and chemical changes

## Quantitative Skills

-   [ ] Convert kg ↔ g ↔ mg
-   [ ] Convert L ↔ mL
-   [ ] Convert °C ↔ K
-   [ ] Identify significant figures
-   [ ] Perform basic dimensional analysis
-   [ ] Use units correctly in calculations

## Chemoinformatics Thinking

You should understand:

``` text
Atom
 ↓
Chemical structure
 ↓
Molecular representation
 ↓
Molecular data
 ↓
Descriptors / fingerprints
 ↓
Machine learning
```

And you should understand why chemistry knowledge is necessary before
working seriously with cheminformatics.

------------------------------------------------------------------------

# 17. Final Practice Test

Try these without looking at the answers.

### Question 1

Define matter.

### Question 2

What is the difference between an element and a compound?

### Question 3

Is air a compound or a mixture? Explain.

### Question 4

Is boiling water a physical or chemical change?

### Question 5

Is burning methane a physical or chemical change?

### Question 6

Classify each:

-   Density
-   Flammability
-   Melting point
-   Reactivity with oxygen
-   Solubility

### Question 7

Convert:

``` text
4.5 kg → g
```

### Question 8

Convert:

``` text
2500 mg → g
```

### Question 9

Convert:

``` text
35°C → K
```

### Question 10

How many significant figures are in:

``` text
0.005060
```

### Question 11

Explain why dimensional analysis is useful.

### Question 12

Explain this cheminformatics pipeline:

``` text
Atoms → Bonds → Molecular structure → Molecular representation → Descriptors → ML
```

------------------------------------------------------------------------

# 18. Answers

### 1

Matter is anything that has mass and occupies space.

### 2

An element consists of one type of atom. A compound contains different
elements chemically bonded in a definite ratio.

### 3

Air is a **mixture** because it contains multiple gases that are
physically combined.

### 4

Physical change.

The H₂O molecules remain H₂O.

### 5

Chemical change.

New substances are produced.

### 6

``` text
Density                → Physical
Flammability           → Chemical
Melting point          → Physical
Reactivity with oxygen → Chemical
Solubility             → Physical
```

### 7

``` text
4.5 kg × 1000 g/kg
= 4500 g
```

### 8

``` text
2500 mg × 1 g/1000 mg
= 2.5 g
```

### 9

``` text
35 + 273.15
= 308.15 K
```

### 10

``` text
0.005060
```

has **4 significant figures**:

``` text
5 0 6 0
```

### 11

Dimensional analysis lets you use units to perform conversions and check
calculations by making unwanted units cancel.

### 12

Atoms form bonds to create molecular structures. Those structures can be
represented computationally using formats such as SMILES or molecular
graphs. Software can then derive descriptors and fingerprints, which can
be used as numerical inputs for machine-learning models.

------------------------------------------------------------------------

# 19. What Comes Next

## 1.2 Atomic Structure

Next, study:

``` text
Atoms
 ↓
Protons
 ↓
Neutrons
 ↓
Electrons
 ↓
Atomic number
 ↓
Mass number
 ↓
Isotopes
 ↓
Ions
 ↓
Cations / Anions
 ↓
Atomic mass
 ↓
Average atomic mass
 ↓
Electron shells
 ↓
Subshells
 ↓
Orbitals
 ↓
Quantum numbers
 ↓
Electron configurations
 ↓
Valence electrons
```

These concepts will then lead naturally into:

``` text
1.3 Periodic Table
        ↓
1.4 Chemical Bonding
        ↓
1.5 Molecular Geometry
        ↓
...
        ↓
Cheminformatics
```
