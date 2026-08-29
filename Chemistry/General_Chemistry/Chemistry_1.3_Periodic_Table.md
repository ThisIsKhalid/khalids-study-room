# Chemistry --- Pillar 1

# 1.3 Periodic Table

> **Goal:** Rebuild your understanding of the periodic table from the
> beginning and learn the trends that explain how elements behave. This
> is especially important for cheminformatics because atomic properties
> strongly influence molecular structure, bonding, polarity, reactivity,
> and computational descriptors.

This lesson follows three layers:

1.  **Layer 1 → Concept:** understand what it means.
2.  **Layer 2 → Problems:** solve basic → intermediate questions.
3.  **Layer 3 → Cheminformatics connection:** understand how the
    chemistry appears later in computational chemistry and
    cheminformatics.

------------------------------------------------------------------------

# 1. Periodic Law

## Layer 1 → Concept

The **periodic law** states that the physical and chemical properties of
elements show a repeating pattern when elements are arranged according
to increasing **atomic number**.

The modern periodic table is therefore organized primarily by:

``` text
Atomic number
      ↓
Periodic arrangement
      ↓
Repeating chemical properties
```

For example, elements in the same column often have similar chemical
behavior because they have related valence-electron configurations.

### Why is it called "periodic"?

Because properties repeat in a regular pattern.

A simplified idea is:

``` text
Atomic number increases
        ↓
Electron configuration changes
        ↓
Valence-electron patterns repeat
        ↓
Chemical properties repeat
```

### Layer 2 → Problems

**Problem 1**

What quantity is used to order the modern periodic table?

**Answer:** Atomic number.

**Problem 2**

Why do some elements have similar chemical properties?

**Answer:** Elements in the same group often have similar
valence-electron configurations.

### Layer 3 → Cheminformatics Connection

A cheminformatics system needs elemental information to understand
molecular structures.

For example:

``` text
C
N
O
S
Cl
```

are not interchangeable.

Their different periodic properties influence:

-   Bonding
-   Atomic size
-   Electronegativity
-   Charge distribution
-   Hydrogen bonding
-   Reactivity
-   Molecular descriptors

------------------------------------------------------------------------

# 2. Groups

## Layer 1 → Concept

A **group** is a vertical column in the periodic table.

There are **18 groups**.

Elements in the same group often have similar chemical properties
because they have related valence-electron configurations.

For example:

``` text
Group 1
H
Li
Na
K
...
```

and:

``` text
Group 17
F
Cl
Br
I
...
```

### Important groups

  Group   Common name             Typical feature
  ------- ----------------------- ------------------------------
  1       Alkali metals           Very reactive metals
  2       Alkaline earth metals   Reactive metals
  17      Halogens                Reactive nonmetals
  18      Noble gases             Very low chemical reactivity

### Layer 2 → Problems

**Problem 1**

Are groups horizontal or vertical?

**Answer:** Vertical.

**Problem 2**

How many groups are in the modern periodic table?

**Answer:** 18.

**Problem 3**

Which group contains chlorine?

**Answer:** Group 17.

### Layer 3 → Cheminformatics Connection

Group information helps predict an atom's likely:

-   Valence
-   Bonding behavior
-   Charge
-   Reactivity

These chemical rules are important when software interprets molecular
structures.

------------------------------------------------------------------------

# 3. Periods

## Layer 1 → Concept

A **period** is a horizontal row in the periodic table.

There are **7 periods**.

As you move across a period:

``` text
Atomic number increases
        ↓
Electrons are added
        ↓
Valence-electron configuration changes
        ↓
Chemical properties change
```

Example:

``` text
Period 2:

Li → Be → B → C → N → O → F → Ne
```

### Layer 2 → Problems

**Problem 1**

Are periods horizontal or vertical?

**Answer:** Horizontal.

**Problem 2**

How many periods are in the periodic table?

**Answer:** 7.

**Problem 3**

Which period contains carbon?

**Answer:** Period 2.

### Layer 3 → Cheminformatics Connection

Period and group information provide a compact way to reason about
elemental behavior.

For example:

``` text
Carbon
Group 14
Period 2
```

This helps explain why carbon commonly forms four covalent bonds and is
so important in organic molecules.

------------------------------------------------------------------------

# 4. Metals

## Layer 1 → Concept

**Metals** occupy most of the left and central regions of the periodic
table.

Typical metallic properties include:

-   Good electrical conductivity
-   Good thermal conductivity
-   Malleability
-   Ductility
-   Metallic luster
-   Tendency to form positive ions

Examples:

``` text
Na
Mg
Al
Fe
Cu
Zn
```

Metals often lose electrons:

``` text
Metal → positive ion + electrons
```

### Layer 2 → Problems

**Problem 1**

Are sodium and magnesium metals?

**Answer:** Yes.

**Problem 2**

Do metals generally tend to lose or gain electrons?

**Answer:** Lose electrons.

### Layer 3 → Cheminformatics Connection

Metal-containing molecules and complexes require special treatment in
cheminformatics.

Examples include:

-   Metal-containing drugs
-   Coordination compounds
-   Organometallic compounds
-   Metalloproteins

Their bonding can be more complicated than ordinary organic molecules.

------------------------------------------------------------------------

# 5. Nonmetals

## Layer 1 → Concept

**Nonmetals** are mainly located on the upper-right side of the periodic
table, with hydrogen as an important exception.

Examples:

``` text
H
C
N
O
F
P
S
Cl
```

Nonmetals commonly:

-   Form covalent bonds
-   Have relatively high electronegativities
-   Gain electrons in some ionic compounds

Many biologically important elements are nonmetals:

``` text
C, H, N, O, P, S
```

These six elements are especially important in organic and biological
chemistry.

### Layer 2 → Problems

**Problem 1**

Is oxygen a metal or nonmetal?

**Answer:** Nonmetal.

**Problem 2**

Is sulfur a metal or nonmetal?

**Answer:** Nonmetal.

**Problem 3**

Name the six especially important elements commonly encountered in
biological molecules.

**Answer:**

``` text
C, H, N, O, P, S
```

### Layer 3 → Cheminformatics Connection

These elements dominate many chemical and drug-discovery datasets.

For example, a typical drug molecule may contain:

``` text
C + H + N + O + S + halogens
```

Understanding their periodic behavior helps you understand molecular
properties later.

------------------------------------------------------------------------

# 6. Metalloids

## Layer 1 → Concept

**Metalloids** have properties intermediate between metals and
nonmetals.

Common examples include:

``` text
B
Si
Ge
As
Sb
Te
```

Their properties can vary depending on the context.

### Layer 2 → Problems

**Problem 1**

Is silicon generally classified as a metalloid?

**Answer:** Yes.

**Problem 2**

Are metalloids simply another name for metals?

**Answer:** No.

They have characteristics intermediate between metals and nonmetals.

### Layer 3 → Cheminformatics Connection

Metalloids are less common than C, N, O, etc. in many drug-like
datasets, but they appear in:

-   Materials chemistry
-   Inorganic chemistry
-   Medicinal chemistry
-   Organosilicon chemistry

------------------------------------------------------------------------

# 7. Main-Group Elements

## Layer 1 → Concept

The **main-group elements** are found primarily in groups:

``` text
1, 2, 13, 14, 15, 16, 17, 18
```

They include the s-block and p-block elements.

For introductory chemistry, main-group elements are especially useful
because their valence-electron patterns are relatively straightforward.

For example:

``` text
Group 14 → commonly 4 valence electrons
Group 15 → commonly 5
Group 16 → commonly 6
Group 17 → commonly 7
Group 18 → commonly 8
```

There are exceptions and special cases, especially for the first-row
elements.

### Layer 2 → Problems

**Problem 1**

Which group usually has 6 valence electrons?

**Answer:** Group 16.

**Problem 2**

Which group contains the halogens?

**Answer:** Group 17.

### Layer 3 → Cheminformatics Connection

Main-group valence patterns help explain the common bonding patterns
that molecular software must handle.

For example:

``` text
C → commonly 4 bonds
N → commonly 3 bonds
O → commonly 2 bonds
F → commonly 1 bond
```

These are simplified rules, but they are extremely useful foundations.

------------------------------------------------------------------------

# 8. Transition Metals

## Layer 1 → Concept

**Transition metals** occupy the central d-block of the periodic table.

Examples:

``` text
Fe
Co
Ni
Cu
Zn
```

They can have:

-   Multiple oxidation states
-   Complex coordination chemistry
-   Variable bonding behavior
-   Distinct magnetic properties

For example, iron commonly occurs as:

``` text
Fe²⁺
Fe³⁺
```

### Layer 2 → Problems

**Problem 1**

Where are transition metals located?

**Answer:** In the central d-block.

**Problem 2**

Can a transition metal have multiple oxidation states?

**Answer:** Yes.

Iron commonly forms Fe²⁺ and Fe³⁺.

### Layer 3 → Cheminformatics Connection

Transition metals become important when working with:

-   Metalloproteins
-   Metal-containing drugs
-   Catalysts
-   Coordination complexes
-   Organometallic chemistry

Representing metal coordination correctly can be difficult for
cheminformatics software because metal-ligand interactions do not always
behave like ordinary organic covalent bonds.

------------------------------------------------------------------------

# 9. Periodic Trends

## Layer 1 → Concept

A **periodic trend** is a predictable pattern in an atomic property as
you move through the periodic table.

The major trends you need to master are:

``` text
Atomic radius
Ionic radius
Ionization energy
Electron affinity
Electronegativity
Metallic character
```

The two directions you should constantly visualize are:

``` text
        ↑
        |
        |
←-------+-------→
        |
        |
        ↓
```

Different properties increase or decrease in different directions.

Do not memorize them as isolated facts. Understand **why** they change.

------------------------------------------------------------------------

# 10. Atomic Radius

## Layer 1 → Concept

**Atomic radius** is a measure of the size of an atom.

A useful general trend is:

``` text
Atomic radius increases ↓
Atomic radius increases ←
```

So:

-   Going **down a group** → atoms generally get larger.
-   Going **left across a period** → atoms generally get larger.

### Why does atomic radius increase down a group?

Each new period adds another occupied electron shell.

Example:

``` text
Li
Na
K
Rb
```

As you move downward, atoms have more electron shells.

Therefore:

``` text
More shells
   ↓
Larger atomic size
```

### Why does atomic radius generally decrease across a period?

Across a period, proton number increases while electrons are added to
the same principal shell.

The increasing nuclear charge pulls electrons more strongly toward the
nucleus.

Therefore:

``` text
Increasing nuclear charge
        ↓
Stronger attraction
        ↓
Smaller atomic radius
```

### Layer 2 → Problems

**Problem 1**

Which is larger: Li or K?

**Answer:** K.

K is lower in the same group.

**Problem 2**

Which is larger: Na or Cl?

**Answer:** Na.

They are in the same period, and atomic radius generally decreases from
left to right.

**Problem 3**

Which direction generally increases atomic radius?

**Answer:**

``` text
Down
and
Left
```

### Layer 3 → Cheminformatics Connection

Atomic size influences:

-   Bond lengths
-   Molecular geometry
-   Steric effects
-   Packing
-   Reactivity

A larger substituent can create greater steric crowding in a molecule.

This becomes especially important in:

-   Molecular modeling
-   Conformation analysis
-   Docking
-   Structure--activity relationships

------------------------------------------------------------------------

# 11. Ionic Radius

## Layer 1 → Concept

**Ionic radius** describes the size of an ion.

Ions can be:

``` text
Cations → positive
Anions  → negative
```

### Cations are generally smaller than their neutral atoms

Example:

``` text
Na → Na⁺
```

Sodium loses an electron, reducing electron-electron repulsion and
sometimes removing an entire outer shell.

Therefore:

``` text
Na⁺ < Na
```

### Anions are generally larger than their neutral atoms

Example:

``` text
Cl → Cl⁻
```

Adding an electron increases electron-electron repulsion.

Therefore:

``` text
Cl⁻ > Cl
```

### Layer 2 → Problems

**Problem 1**

Which is generally larger: Na or Na⁺?

**Answer:** Na.

**Problem 2**

Which is generally larger: Cl or Cl⁻?

**Answer:** Cl⁻.

**Problem 3**

Why are cations usually smaller than their neutral atoms?

**Answer:** They lose electrons, reducing electron-electron repulsion
and potentially removing an occupied shell.

### Layer 3 → Cheminformatics Connection

Ionic size matters in:

-   Salt formation
-   Ionic interactions
-   Molecular recognition
-   Coordination chemistry
-   Protein--ligand interactions

It also helps explain why charged molecules can behave very differently
from their neutral forms.

------------------------------------------------------------------------

# 12. Ionization Energy

## Layer 1 → Concept

**Ionization energy** is the energy required to remove an electron from
a gaseous atom.

Conceptually:

``` text
Atom → positive ion + electron
```

requires energy.

### General trend

Ionization energy generally:

``` text
increases ↑
increases →
```

So:

-   Higher up a group → generally higher ionization energy.
-   Further right across a period → generally higher ionization energy.

### Why?

Smaller atoms with stronger nuclear attraction hold their electrons more
tightly.

Therefore:

``` text
Stronger attraction
       ↓
Harder to remove electron
       ↓
Higher ionization energy
```

### Layer 2 → Problems

**Problem 1**

Which generally has higher ionization energy: Li or K?

**Answer:** Li.

K is lower in the group and its outer electron is farther from the
nucleus.

**Problem 2**

Which generally has higher ionization energy: Na or Cl?

**Answer:** Cl.

Ionization energy generally increases across the period.

### Layer 3 → Cheminformatics Connection

Ionization behavior helps explain:

-   Cation formation
-   Molecular charge
-   Protonation/deprotonation behavior
-   Redox chemistry

Charge state is extremely important when predicting molecular properties
and molecular interactions.

------------------------------------------------------------------------

# 13. Electron Affinity

## Layer 1 → Concept

**Electron affinity** describes the energy change associated with adding
an electron to a gaseous atom.

Conceptually:

``` text
Atom + electron → anion
```

Electron affinity is more complicated than some other periodic trends
because the exact values can have exceptions.

A useful introductory trend is that electron affinity generally becomes
more favorable toward the upper-right region of the periodic table, with
important exceptions.

Halogens have a strong tendency to gain an electron because doing so
brings them closer to a filled valence shell.

Example:

``` text
Cl + e⁻ → Cl⁻
```

### Layer 2 → Problems

**Problem 1**

Which type of elements strongly tend to gain an electron?

**Answer:** Many nonmetals, especially halogens.

**Problem 2**

What happens when chlorine gains an electron?

``` text
Cl + e⁻ → Cl⁻
```

It becomes chloride.

### Layer 3 → Cheminformatics Connection

Electron affinity contributes to understanding:

-   Anion formation
-   Charge distribution
-   Redox behavior
-   Electronic properties

These concepts become increasingly important when you move into
computational chemistry and molecular-property prediction.

------------------------------------------------------------------------

# 14. Electronegativity

## Layer 1 → Concept

**Electronegativity** is the tendency of an atom in a chemical bond to
attract shared electrons toward itself.

This is one of the most important concepts for organic chemistry.

The general trend is:

``` text
Electronegativity increases ↑
Electronegativity increases →
```

Fluorine is the most electronegative element.

A simplified ranking among common organic elements is:

``` text
F > O > N > C > H
```

### Example

Consider:

``` text
C — O
```

Oxygen is more electronegative than carbon.

Therefore the bonding electrons are pulled more toward oxygen:

``` text
Cδ+ — Oδ−
```

This creates a **polar bond**.

### Layer 2 → Problems

**Problem 1**

Which is more electronegative: O or C?

**Answer:** O.

**Problem 2**

Which is more electronegative: F or Cl?

**Answer:** F.

**Problem 3**

In C---O, which atom attracts the bonding electrons more strongly?

**Answer:** O.

### Layer 3 → Cheminformatics Connection

Electronegativity is directly connected to:

-   Bond polarity
-   Molecular polarity
-   Hydrogen bonding
-   Dipole moments
-   Solubility
-   Lipophilicity
-   Protein--ligand interactions

This is especially important in drug discovery because changing one atom
can substantially change molecular properties.

For example:

``` text
C-H
```

and

``` text
C-F
```

do not behave identically.

Replacing H with F can alter:

-   Electronic properties
-   Metabolic stability
-   Lipophilicity
-   Molecular interactions

------------------------------------------------------------------------

# 15. Metallic Character

## Layer 1 → Concept

**Metallic character** describes how strongly an element behaves like a
metal.

The general trend is:

``` text
Metallic character increases ↓
Metallic character increases ←
```

Therefore:

``` text
Bottom-left
     ↓
More metallic
```

and:

``` text
Top-right
     ↓
More nonmetallic
```

### Why?

Metals generally have a greater tendency to lose electrons.

Elements toward the lower-left generally have:

-   Larger atomic radius
-   Lower ionization energy
-   Lower electronegativity

These characteristics favor electron loss.

### Layer 2 → Problems

**Problem 1**

Which is more metallic: Na or Cl?

**Answer:** Na.

**Problem 2**

Which region of the periodic table has the strongest metallic character?

**Answer:** Lower-left region.

### Layer 3 → Cheminformatics Connection

Metallic character helps establish the fundamental differences between:

``` text
Organic covalent chemistry
        vs.
Metal / ionic chemistry
```

Most drug-like molecular datasets are dominated by organic compounds,
but metal-containing compounds require different chemical assumptions.

------------------------------------------------------------------------

# 16. Periodic Trend Summary

Memorize the overall directions:

``` text
                    ↑
        Atomic radius decreases
        Ionization energy increases
        Electronegativity increases
        Electron affinity generally
        becomes more favorable
                    |
                    |
←-------------------+-------------------→
                    |
                    |
        Atomic radius increases
        Metallic character increases
                    ↓
```

A simpler memory framework:

### Toward the upper-right

Generally:

``` text
Smaller atoms
Higher ionization energy
Higher electronegativity
More nonmetallic
```

### Toward the lower-left

Generally:

``` text
Larger atoms
Lower ionization energy
Lower electronegativity
More metallic
```

------------------------------------------------------------------------

# 17. Comparing the Major Trends

  -----------------------------------------------------------------------
  Property                Across a period →       Down a group ↓
  ----------------------- ----------------------- -----------------------
  Atomic radius           Generally decreases     Increases

  Ionic radius            Complex                 Generally increases

  Ionization energy       Generally increases     Decreases

  Electronegativity       Generally increases     Decreases

  Metallic character      Decreases               Increases

  Electron affinity       General trend toward    General trend becomes
                          more favorable          less favorable
  -----------------------------------------------------------------------

> **Important:** These are general trends, not absolute rules. Electron
> affinity and some ionization-energy patterns contain exceptions.

------------------------------------------------------------------------

# 18. Practice --- Basic

Try these before checking the answers.

### Question 1

How many groups are in the periodic table?

### Question 2

How many periods?

### Question 3

Are groups vertical or horizontal?

### Question 4

Are periods vertical or horizontal?

### Question 5

Which group contains the halogens?

### Question 6

Which group contains the noble gases?

### Question 7

Which is larger: Li or K?

### Question 8

Which is more electronegative: C or O?

### Question 9

Which has higher ionization energy: Na or Cl?

### Question 10

Which is larger: Na or Na⁺?

------------------------------------------------------------------------

# 19. Answers --- Basic

### 1

18 groups.

### 2

7 periods.

### 3

Vertical.

### 4

Horizontal.

### 5

Group 17.

### 6

Group 18.

### 7

K.  

Atomic radius increases down a group.

### 8

O.  

Electronegativity generally increases toward the upper-right.

### 9

Cl.

Ionization energy generally increases across a period.

### 10

Na.

A cation is generally smaller than its neutral atom.

------------------------------------------------------------------------

# 20. Practice --- Intermediate

### Question 1

Rank these atoms from smallest to largest atomic radius:

``` text
Li, Na, K
```

### Question 2

Rank these elements from lower to higher electronegativity:

``` text
C, N, O, F
```

### Question 3

Which has the greater ionization energy?

``` text
Mg or Ca
```

Explain why.

### Question 4

Which has the greater atomic radius?

``` text
Na or Cl
```

Explain why.

### Question 5

Explain why atomic radius generally decreases across a period.

### Question 6

Explain why atomic radius increases down a group.

### Question 7

Explain why Na⁺ is smaller than Na.

### Question 8

Explain why Cl⁻ is larger than Cl.

------------------------------------------------------------------------

# 21. Answers --- Intermediate

### 1

``` text
Li < Na < K
```

Atomic radius increases down the group.

### 2

``` text
C < N < O < F
```

Electronegativity generally increases from left to right across a
period.

### 3

**Mg has higher ionization energy than Ca.**

Both are in Group 2, but Ca is lower.

The outer electron in Ca is farther from the nucleus and easier to
remove.

### 4

**Na is larger than Cl.**

Both are in Period 3.

Moving across the period increases nuclear charge, pulling electrons
more strongly toward the nucleus.

### 5

Across a period, proton number increases while electrons are added to
the same general principal shell.

The stronger nuclear attraction pulls the electron cloud inward.

### 6

Moving down a group adds occupied electron shells.

More shells increase the distance between the nucleus and outer
electrons.

Therefore atomic radius increases.

### 7

Na⁺ forms when sodium loses its outer electron.

This reduces electron-electron repulsion and removes its outermost
occupied shell.

Therefore:

``` text
Na⁺ < Na
```

### 8

Cl⁻ has one additional electron compared with neutral chlorine.

The additional electron increases electron-electron repulsion.

Therefore:

``` text
Cl⁻ > Cl
```

------------------------------------------------------------------------

# 22. Cheminformatics Connection --- Why Periodic Trends Matter

The periodic table is not just a table to memorize.

It explains why changing an atom can change an entire molecule.

Consider a simple conceptual transformation:

``` text
Molecule A
    |
    | replace H with F
    ↓
Molecule B
```

The molecular skeleton may remain almost identical, but the changed atom
has different:

-   Atomic size
-   Electronegativity
-   Electron distribution
-   Bonding behavior

Therefore molecular properties can change.

This is one of the central ideas behind **structure--property
relationships**.

``` text
Atomic identity
      ↓
Electronic properties
      ↓
Bonding
      ↓
3D molecular structure
      ↓
Molecular properties
      ↓
Biological activity
```

This is exactly why atom-level chemistry matters in cheminformatics.

------------------------------------------------------------------------

# 23. Connection to Molecular Descriptors

Periodic properties ultimately influence molecular descriptors.

For example:

``` text
Atomic composition
      ↓
Molecular structure
      ↓
Chemical properties
      ↓
Descriptors
```

Common descriptors you will encounter later include:

-   Molecular weight
-   LogP
-   Topological polar surface area (TPSA)
-   Hydrogen-bond donors
-   Hydrogen-bond acceptors
-   Rotatable bonds
-   Formal charge
-   Fraction of sp³ atoms
-   Molecular fingerprints

Periodic trends help explain the chemistry behind many of these
properties.

------------------------------------------------------------------------

# 24. Connection to Drug Discovery

Suppose you modify a drug molecule:

``` text
R-H
```

to:

``` text
R-F
```

You have changed only one atom, but potentially changed:

``` text
Electronegativity
      ↓
Electron distribution
      ↓
Bond polarity
      ↓
Molecular interactions
      ↓
Metabolic behavior
      ↓
Pharmacological properties
```

This is why medicinal chemists frequently explore **small structural
modifications**.

Cheminformatics helps analyze these modifications computationally.

------------------------------------------------------------------------

# 25. What You Need to Master Before 1.4

Before moving to **1.4 Chemical Bonding**, make sure you can:

## Periodic Table Structure

-   [ ] Explain periodic law
-   [ ] Identify groups
-   [ ] Identify periods
-   [ ] Know there are 18 groups
-   [ ] Know there are 7 periods
-   [ ] Identify metals
-   [ ] Identify nonmetals
-   [ ] Identify metalloids
-   [ ] Understand main-group elements
-   [ ] Identify transition metals

## Periodic Trends

-   [ ] Explain atomic radius
-   [ ] Predict atomic-radius trends
-   [ ] Explain ionic radius
-   [ ] Compare cations and neutral atoms
-   [ ] Compare anions and neutral atoms
-   [ ] Explain ionization energy
-   [ ] Predict ionization-energy trends
-   [ ] Explain electron affinity at an introductory level
-   [ ] Explain electronegativity
-   [ ] Predict electronegativity trends
-   [ ] Explain metallic character

## Chemistry → Cheminformatics

You should understand:

``` text
Periodic position
      ↓
Electron configuration
      ↓
Atomic properties
      ↓
Bonding behavior
      ↓
Molecular structure
      ↓
Molecular properties
      ↓
Cheminformatics
```

------------------------------------------------------------------------

# 26. Final Mastery Test

Try these without notes.

### 1.

Why is the periodic table arranged by atomic number?

### 2.

What is the difference between a group and a period?

### 3.

Where are metals generally located?

### 4.

Where are nonmetals generally located?

### 5.

What is the general trend of atomic radius?

### 6.

What is the general trend of ionization energy?

### 7.

What is the general trend of electronegativity?

### 8.

What is the general trend of metallic character?

### 9.

Why is Na⁺ smaller than Na?

### 10.

Why is Cl⁻ larger than Cl?

### 11.

Which is more electronegative: N or O?

### 12.

Which is larger: Mg or Ba?

### 13.

Which has higher ionization energy: Li or Cs?

### 14.

Explain how periodic trends can influence a drug molecule's properties.

------------------------------------------------------------------------

# 27. Final Answers

### 1.

The modern periodic table is arranged by increasing atomic number.
Chemical properties show repeating patterns as atomic number increases.

### 2.

``` text
Group  → vertical column
Period → horizontal row
```

### 3.

Mostly the left and center.

### 4.

Mostly the upper-right, with hydrogen as an important exception.

### 5.

``` text
↑ toward upper-right → generally smaller
↓ toward lower-left → generally larger
```

More simply:

``` text
Atomic radius increases ↓ and ←
```

### 6

Ionization energy generally increases:

``` text
↑ and →
```

### 7

Electronegativity generally increases:

``` text
↑ and →
```

### 8

Metallic character generally increases:

``` text
↓ and ←
```

### 9

Na⁺ has lost an electron, reducing electron-electron repulsion and
potentially removing an entire outer shell.

### 10

Cl⁻ has gained an electron, increasing electron-electron repulsion.

### 11

O.  

### 12

Ba.

Atomic radius generally increases down a group.

### 13

Li.

Ionization energy generally decreases down a group.

### 14

Periodic properties determine how atoms interact with electrons and
other atoms. Changing an atom can alter bond polarity, charge
distribution, molecular interactions, and therefore properties such as
solubility, lipophilicity, stability, and biological activity.

------------------------------------------------------------------------

# 28. One-Page Memory Sheet

## Periodic Table

``` text
Groups  → vertical
Periods → horizontal

18 groups
7 periods
```

## Important Regions

``` text
Left / center → mostly metals
Upper-right   → mostly nonmetals
Staircase     → metalloids
Center        → transition metals
```

## Major Trends

``` text
                    Atomic radius
                         ↓
                         ←

Ionization energy      ↑ →
Electronegativity      ↑ →
Metallic character     ↓ ←
```

## Ion Size

``` text
Cation < neutral atom

Anion > neutral atom
```

## Key Groups

``` text
Group 1  → Alkali metals
Group 2  → Alkaline earth metals
Group 17 → Halogens
Group 18 → Noble gases
```

## Chemoinformatics Bridge

``` text
Periodic table
      ↓
Atomic properties
      ↓
Electron behavior
      ↓
Chemical bonding
      ↓
Molecular structure
      ↓
Molecular properties
      ↓
Descriptors / fingerprints
      ↓
QSAR / ML / Drug discovery
```

------------------------------------------------------------------------

# 29. Next Topic

## 1.4 Chemical Bonding

The next topic builds directly on everything here:

``` text
Valence electrons
      ↓
Why atoms bond
      ↓
Ionic bonding
      ↓
Covalent bonding
      ↓
Metallic bonding
      ↓
Lewis structures
      ↓
Octet rule
      ↓
Formal charge
      ↓
Resonance
      ↓
Bond polarity
      ↓
Bond strength
      ↓
Bond length
      ↓
Coordinate covalent bonds
```

This is a **very important topic for your cheminformatics preparation**,
because molecular structures that computers manipulate are fundamentally
determined by atoms and bonds.
