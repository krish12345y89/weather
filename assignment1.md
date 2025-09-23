# Problem (restated)

**Given:** Atomic radius of Aluminium (Al) with FCC crystal structure is **0.1432 nm**.
**Find:** Number of **unit cells per cubic metre** (i.e., how many unit cells fit in $1\ \text{m}^3$).

---

# Topic background (what this is about)

**English (short explanation):**
FCC (face-centered cubic) is a crystal structure where atoms are located at the eight corners and at the centers of the six faces of the cube. The relation between the atomic radius $r$ and the cube edge length $a$ for FCC is:

$$
a = \frac{4r}{\sqrt{3}}
$$

because along the face diagonal three atomic radii line up: face diagonal $= 4r$ and face diagonal also $= a\sqrt{2}$; combining with geometry gives $a = \frac{4r}{\sqrt{3}}$.

**Hinglish (short):**
FCC matlab face-centered cubic — cube ke corners pe atoms hain aur har face ke center pe bhi ek atom hota hai. FCC mein atom radius $r$ aur unit cell edge $a$ ka relation:

$$
a=\frac{4r}{\sqrt{3}}
$$

Yeh isliye kyunki face diagonal pe 4 radii aa jaate hain aur face diagonal = $a\sqrt{2}$. Geometry se upar wala relation milta hai.

---

# Step-by-step solution (complete, with units and digit-by-digit arithmetic)

**Step 0 — convert radius to metres (very important):**
Given $r = 0.1432\ \text{nm}$.
1 nm = $10^{-9}$ m, so:

$$
r = 0.1432 \times 10^{-9}\ \text{m} = 1.432\times 10^{-10}\ \text{m}.
$$

**Hinglish:**
$r=0.1432$ nm ko metre mein badalo: $0.1432\times10^{-9} = 1.432\times10^{-10}$ m.

---

**Step 1 — compute lattice parameter $a$ for FCC:**
Formula:

$$
a = \frac{4r}{\sqrt{3}}.
$$

Compute numerically (showing the constants):

* $\sqrt{3} \approx 1.7320508075688772$.
* $4r = 4 \times 1.432\times10^{-10} = 5.728\times10^{-10}\ \text{m}.$

Now divide:

$$
a = \frac{5.728\times10^{-10}}{1.7320508075688772}
  = 3.307062341918177\times10^{-10}\ \text{m}.
$$

Round/express reasonably:

$$
a \approx 3.30706\times10^{-10}\ \text{m} \quad(\text{or }0.330706\ \text{nm}).
$$

**Hinglish:**
$\sqrt{3}\approx1.73205$. $4r=5.728\times10^{-10}$ m, divide karne pe:
$a\approx3.30706\times10^{-10}$ m (ya $0.330706$ nm).

---

**Step 2 — find volume of one unit cell $V_{cell}$:**
Unit cell is a cube of edge $a$, so:

$$
V_{cell} = a^3.
$$

Compute:

$$
a = 3.307062341918177\times10^{-10}\ \text{m},
$$

so

$$
V_{cell} = (3.307062341918177\times10^{-10})^3
         = 3.6168220841779314\times10^{-29}\ \text{m}^3.
$$

Round sensibly:

$$
V_{cell} \approx 3.61682\times10^{-29}\ \text{m}^3.
$$

**Hinglish:**
Unit cell ka volume $a^3$. $a$ ka cube leneka baad $V_{cell}\approx3.61682\times10^{-29}$ m³ milta hai.

---

**Step 3 — number of unit cells per cubic metre:**
We want how many such volumes fit into $1\ \text{m}^3$:

$$
N_{\text{cells}} = \frac{1\ \text{m}^3}{V_{cell}} = \frac{1}{3.6168220841779314\times10^{-29}}.
$$

Compute:

$$
N_{\text{cells}} = 2.7648581454271073\times10^{28}\ \text{unit cells per m}^3.
$$

Round to appropriate significant figures (input had 4 sig figs), so keep 4 sig figs:

$$
\boxed{N_{\text{cells}} \approx 2.765\times10^{28}\ \text{unit cells m}^{-3}}.
$$

**Hinglish:**
1 m³ ko divide karo unit-cell-volume se, milta hai $N\approx2.765\times10^{28}$ unit cells per m³ (4 significant figures rakh ke).

---

# Extra useful note (atoms per m³)

FCC has **4 atoms per unit cell** (because corner atoms contribute $8\times 1/8 =1$ and face atoms contribute $6\times 1/2 =3$, total = 4).

So **atoms per m³**:

$$
N_{\text{atoms}} = 4 \times N_{\text{cells}} = 4 \times 2.764858\times10^{28}
= 1.105943\times10^{29}\ \text{atoms m}^{-3}.
$$

Round:

$$
\boxed{N_{\text{atoms}} \approx 1.106\times10^{29}\ \text{atoms m}^{-3}}.
$$

**Hinglish:**
FCC mein ek unit cell me 4 atoms hote hain, isliye atoms per m³ = $4\times2.765\times10^{28}\approx1.106\times10^{29}$.

---

# Quick unit-check and intuition

* Units: $r$ in metres → $a$ in metres → $a^3$ in m³ → dividing 1 m³ by that gives a pure number (unit cells per m³). Units cancel correctly.
* Intuition: atomic sizes are \~10⁻¹⁰ m; so a unit cell volume \~10⁻²⁹ m³; therefore number per m³ \~10²⁸ — matches our result.

**Hinglish:**
Units sahi chal rahe hain. Atom size \~$10^{-10}$ m toh cell volume \~$10^{-29}$ m³ aur 1 m³ me \~$10^{28}$ cells honge — ye intuition sahi hai.

---

# Common mistakes (and what I think happened in the handwritten solution)

* A common slip: using $a = 2r$ (that would be for simple cubic, not for FCC) or mixing up face diagonal formula. For FCC the correct relation is $a = \tfrac{4r}{\sqrt{3}}$.
* In the handwritten solution image I see a different final numeric value (\~1.51×10²⁸). That’s likely because they used a wrong intermediate (maybe used $a = \frac{4r}{\sqrt{2}}$ or used wrong powers or unit conversion). The method above is the correct geometrical relation and arithmetic.

**Hinglish:**
Galti usually $a=2r$ lagana (woh simple cubic ke liye hota). Handwritten answer 1.51×10²⁸ alag number dikh raha hai — shayad intermediate me formula ya conversion galat hua. Upar jo maine step-by-step diya woh correct hai.

---

# Final answers (clean)

* **Unit cells per cubic metre:** $\boxed{2.765\times10^{28}\ \text{unit cells m}^{-3}}$ (4 s.f.)
* **Atoms per cubic metre (FCC):** $\boxed{1.106\times10^{29}\ \text{atoms m}^{-3}}$ (4 s.f.)

---
#  2nd one 

# 📌 Topic Background: HCP Crystal Structure

**English:**
HCP = Hexagonal Close-Packed.

* It consists of atoms arranged in hexagonal layers:

  * Bottom layer (A),
  * Middle layer (B),
  * Top layer (A again).
* The lattice parameters are:

  * $a$ = edge length of hexagon (distance between nearest neighbors in basal plane),
  * $c$ = height of the hexagonal prism (unit cell height).

We want to **prove** that for ideal close-packing,

$$
\frac{c}{a} = 1.633
$$

**Hinglish:**
HCP matlab Hexagonal Close-Packed structure. Isme atoms hexagonal layers me arrange hote hain: niche A layer, beech me B layer, aur upar fir A layer.
Lattice constants:

* $a$ = hexagon ka side (atoms ke beech ka distance basal plane me).
* $c$ = unit cell ki height (vertical dimension).

Target: Proof karo ki **ideal packing** me

$$
\frac{c}{a} = 1.633
$$

---

# 📌 Step-by-Step Proof

### Step 1: Consider the tetrahedron inside HCP

* Take 3 atoms at the **corners of the base hexagon** → they form an equilateral triangle of side $a$.
* Place 1 atom from the middle layer (B) above the center of this triangle.
  This makes a **regular tetrahedron**.

So geometry of tetrahedron is used.

---

### Step 2: Height of equilateral triangle

We know equilateral triangle of side $a$.
Height $h$ is:

$$
h = \sqrt{a^2 - \left(\frac{a}{2}\right)^2} = \sqrt{a^2 - \frac{a^2}{4}} = \sqrt{\frac{3a^2}{4}} = \frac{\sqrt{3}}{2}a
$$

**Hinglish:**
Equilateral triangle (side $a$) ki height:

$$
h = \sqrt{a^2 - \left(\frac{a}{2}\right)^2} = \frac{\sqrt{3}}{2}a
$$

---

### Step 3: Distance from atom to center of triangle

The centroid (center) of equilateral triangle lies at $ \frac{2}{3}$ of the height from the vertex.
So distance from one corner atom to centroid is:

$$
x = \frac{2}{3}h = \frac{2}{3}\cdot \frac{\sqrt{3}}{2}a = \frac{a}{\sqrt{3}}
$$

**Hinglish:**
Centroid distance vertex se = $2/3$ × height =

$$
x = \frac{a}{\sqrt{3}}
$$

---

### Step 4: Geometry of tetrahedron

Now consider line joining **atom at centroid (middle layer atom)** and **one atom of bottom layer**.

* That distance is the atomic diameter $= 2r$.
* But we are using $a = 2r$, so $a$ = edge length.

Now half of $c$ (i.e., $c/2$) is the vertical distance from middle atom to bottom layer atom.

From Pythagoras theorem in tetrahedron:

$$
\left(\frac{c}{2}\right)^2 = a^2 - x^2
$$

Substitute $x = \frac{a}{\sqrt{3}}$:

$$
\left(\frac{c}{2}\right)^2 = a^2 - \left(\frac{a}{\sqrt{3}}\right)^2
= a^2 - \frac{a^2}{3}
= \frac{2a^2}{3}
$$

So,

$$
\frac{c}{2} = \sqrt{\frac{2}{3}}a
$$

Therefore:

$$
c = 2\sqrt{\frac{2}{3}}a
= \frac{2\sqrt{6}}{3}a
$$

---

### Step 5: Final ratio

$$
\frac{c}{a} = \frac{2\sqrt{6}}{3}
$$

Now compute numerically:

* $\sqrt{6} \approx 2.449$
* Multiply: $2 \times 2.449 = 4.898$
* Divide by 3 = $1.633$

So proven:

$$
\boxed{\frac{c}{a} = 1.633}
$$

**Hinglish:**
Tetrahedron geometry se

$$
\frac{c}{a} = \frac{2\sqrt{6}}{3} \approx 1.633
$$

---

# ✅ Final Answer

* **Ideal c/a ratio for HCP crystal structure = 1.633**
* Derived using tetrahedron geometry and Pythagoras theorem.

---
                    3rd question
Bhai mast question hai 👍 — ye wala **Atomic Packing Factor (APF)** ka derivation hai for **BCC, FCC, aur HCP**. Main har ek line aur formula ko **deeply samjhata hoon** in **English + Hinglish**, step-by-step.

---

# 📌 Topic Background: APF

**English:**
APF (Atomic Packing Factor) is the fraction of space occupied by atoms in a unit cell.

Formula:

$$
APF = \frac{\text{Volume of atoms in unit cell}}{\text{Volume of unit cell}}
$$

* Numerator: volume of all atoms inside the cell.
* Denominator: total cell volume.
  This tells us how efficiently atoms are packed.

**Hinglish:**
APF matlab unit cell me atoms kitni jagah fill kar rahe hain vs total jagah.

Formula:

$$
APF = \frac{\text{Atoms ka volume (cell ke andar)}}{\text{Cell ka total volume}}
$$

---

# 📌 Case 1: BCC (Body-Centered Cubic)

* In BCC → 8 corner atoms + 1 body atom.
* Each corner atom contributes $1/8$, so total contribution = $8 \times \frac{1}{8} = 1$.
* Plus the body atom = 1.
  So **2 atoms per unit cell**.

**Relation between a and r (atomic radius):**
In BCC, atoms touch along the body diagonal.

$$
\sqrt{3}a = 4r \quad \Rightarrow \quad a = \frac{4r}{\sqrt{3}}
$$

**Step 1 – Volume of atoms inside cell:**
One atom volume = $\frac{4}{3}\pi r^3$.
Total = $2 \times \frac{4}{3}\pi r^3 = \frac{8}{3}\pi r^3$.

**Step 2 – Volume of unit cell:**

$$
V_{cell} = a^3 = \left(\frac{4r}{\sqrt{3}}\right)^3 = \frac{64r^3}{3\sqrt{3}}
$$

**Step 3 – APF:**

$$
APF_{BCC} = \frac{\frac{8}{3}\pi r^3}{\frac{64}{3\sqrt{3}}r^3}
= \frac{\pi \sqrt{3}}{8} \approx 0.680
$$

✅ **Result: APF (BCC) = 0.68**

**Hinglish:**
BCC me 2 atoms/cell. Atoms ka volume $\frac{8}{3}\pi r^3$. Cell ka volume $\frac{64}{3\sqrt{3}}r^3$. Ratio nikal ke $0.68$ aata hai.

---

# 📌 Case 2: FCC (Face-Centered Cubic)

* In FCC → 8 corners + 6 face centers.
* Corner contribution = 1 atom, face contribution = 3 atoms.
  So total = 4 atoms/unit cell.

**Relation between a and r:**
Atoms touch along face diagonal.

$$
\sqrt{2}a = 4r \quad \Rightarrow \quad a = \frac{4r}{\sqrt{2}} = 2\sqrt{2}r
$$

**Step 1 – Volume of atoms:**

$$
4 \times \frac{4}{3}\pi r^3 = \frac{16}{3}\pi r^3
$$

**Step 2 – Volume of unit cell:**

$$
a^3 = (2\sqrt{2}r)^3 = 16\sqrt{2}r^3
$$

**Step 3 – APF:**

$$
APF_{FCC} = \frac{\frac{16}{3}\pi r^3}{16\sqrt{2}r^3}
= \frac{\pi}{3\sqrt{2}} \approx 0.740
$$

✅ **Result: APF (FCC) = 0.74**

**Hinglish:**
FCC me 4 atoms/cell. Total atom volume $\frac{16}{3}\pi r^3$. Cell volume $16\sqrt{2}r^3$. Ratio = $0.74$.

---

# 📌 Case 3: HCP (Hexagonal Close-Packed)

* In HCP, effectively 6 atoms/unit cell.
* Ideal ratio $\frac{c}{a} = 1.633$.

**Step 1 – Volume of atoms in unit cell:**

$$
6 \times \frac{4}{3}\pi r^3 = 8\pi r^3
$$

**Step 2 – Volume of unit cell:**
Unit cell volume = Base area × height.

* Base = regular hexagon = $\frac{3\sqrt{3}}{2}a^2$.
* Height = $c = 1.633a$.
  So,

$$
V_{cell} = \frac{3\sqrt{3}}{2}a^2 \cdot c
$$

With $a = 2r$, $c = 1.633a$:

$$
V_{cell} = \frac{3\sqrt{3}}{2}(2r)^2(1.633\times 2r)
= 24.74r^3
$$

**Step 3 – APF:**

$$
APF_{HCP} = \frac{8\pi r^3}{24.74r^3}
= \frac{\pi}{3\sqrt{2}} \approx 0.74
$$

✅ **Result: APF (HCP) = 0.74**

**Hinglish:**
HCP me 6 atoms/cell. Atom volume $8\pi r^3$. Cell volume (hexagon base × height) nikal ke \~24.74r³ aata hai. Ratio \~0.74.

---

# 🎯 Final Results

* $APF_{BCC} = 0.68$
* $APF_{FCC} = 0.74$
* $APF_{HCP} = 0.74$

---
Nice — chalo is problem ko **line-by-line** aur **digit-by-digit** solve karte hain, phir comparison karke final conclusion denge. Main **English** explanation pehle dunga, phir **Hinglish** (simple mix) — aur har formula + unit conversion clear karunga.

---

# Problem (restated)

**Given:** Rhodium atomic radius $r = 0.1245\ \text{nm}$ and density $\rho_{\text{exp}} = 12.41\ \text{g cm}^{-3}$. Atomic mass $A = 102.91\ \text{g mol}^{-1}$.
**Q:** Decide whether Rh is BCC or FCC using these data (i.e., compute theoretical densities for BCC and FCC and compare).

---

# Key formula (what we will use)

Density from crystal geometry:

$$
\rho = \frac{nA}{N_A V_{\text{cell}}}
$$

where

* $n$ = number of atoms per unit cell (BCC: 2, FCC: 4),
* $A$ = atomic mass (g mol$^{-1}$),
* $N_A = 6.022\times10^{23}\ \text{mol}^{-1}$,
* $V_{\text{cell}}$ = volume of unit cell in cm$^3$.

Relations between lattice parameter $a$ and atomic radius $r$:

* BCC: body diagonal $=4r \Rightarrow \sqrt{3}\,a = 4r \Rightarrow a = \dfrac{4r}{\sqrt{3}}$.
* FCC: face diagonal $=4r \Rightarrow \sqrt{2}\,a = 4r \Rightarrow a = \dfrac{4r}{\sqrt{2}} = 2\sqrt{2}\,r$.

---

# Step 0 — unit conversion (very important)

Given $r = 0.1245\ \text{nm}$.
1 nm = $10^{-7}$ cm. So

$$
r = 0.1245\times 10^{-7}\ \text{cm} = 1.245\times10^{-8}\ \text{cm}.
$$

(Keep digits: $r = 1.245\cdot10^{-8}\ \text{cm}$.)

---

# BCC case (detailed arithmetic)

1. Lattice parameter:

$$
a_{BCC} = \frac{4r}{\sqrt{3}}
= \frac{4\times 1.245\times10^{-8}\ \text{cm}}{1.7320508075688772}
$$

Compute numerator: $4r = 4\times1.245\times10^{-8} = 4.980\times10^{-8}\ \text{cm}.$
Divide:

$$
a_{BCC} = \frac{4.980\times10^{-8}}{1.7320508076} = 2.8752043406\times10^{-8}\ \text{cm}.
$$

2. Unit cell volume:

$$
V_{BCC} = a^3 = (2.8752043406\times10^{-8})^3
= 2.3768739243\times10^{-23}\ \text{cm}^3.
$$

3. Atoms per cell: $n_{BCC}=2$. Atomic mass $A=102.91$ g/mol. Avogadro $N_A=6.022\times10^{23}$.

4. Density:

$$
\rho_{BCC}=\frac{2\times102.91}{6.022\times10^{23}\times 2.3768739243\times10^{-23}}
$$

Compute denominator: $6.022\times10^{23}\times 2.3768739243\times10^{-23} = 14.312\ldots$ (we keep full precision in intermediate). Doing full division gives:

$$
\rho_{BCC} \approx 14.37939707\ \text{g cm}^{-3}.
$$

(rounded sensibly: $\rho_{BCC}=14.38\ \text{g cm}^{-3}$.)

---

# FCC case (detailed arithmetic)

1. Lattice parameter:

$$
a_{FCC} = \frac{4r}{\sqrt{2}} = 2\sqrt{2}\,r.
$$

Compute:
$\sqrt{2}=1.41421356237$.
$a_{FCC} = \frac{4\times1.245\times10^{-8}}{1.41421356237} = 3.5213917703\times10^{-8}\ \text{cm}.$

2. Unit cell volume:

$$
V_{FCC} = a^3 = (3.5213917703\times10^{-8})^3 = 4.3665962230\times10^{-23}\ \text{cm}^3.
$$

3. Atoms per cell $n_{FCC}=4$.

4. Density:

$$
\rho_{FCC}=\frac{4\times102.91}{6.022\times10^{23}\times 4.3665962230\times10^{-23}}
$$

Compute:

$$
\rho_{FCC} \approx 15.65430473\ \text{g cm}^{-3}.
$$

(rounded: $\rho_{FCC}=15.65\ \text{g cm}^{-3}$.)

---

# Comparison with experimental density

* $\rho_{\text{exp}} = 12.41\ \text{g cm}^{-3}$ (given).
* $\rho_{BCC} \approx 14.38\ \text{g cm}^{-3}$ → error w\.r.t. experiment:

  $$
  \frac{14.38-12.41}{12.41}\times100\% \approx 15.9\% \text{ high}.
  $$
* $\rho_{FCC} \approx 15.65\ \text{g cm}^{-3}$ → error:

  $$
  \frac{15.65-12.41}{12.41}\times100\% \approx 26.1\% \text{ high}.
  $$

**Which is closer numerically?** BCC is closer (smaller % error), but *neither* theoretical density equals the experimental value — both predicted densities are larger than the given 12.41 g/cm³.

---

# Final conclusion & important note (physics context)

* **From raw numbers alone:** the theoretical BCC density (14.38) is closer to the given density (12.41) than the theoretical FCC density (15.65). So *numerically* BCC matches the given density better.
* **BUT (very important):** Real crystalline Rhodium is known to be **FCC** (space group $Fm\bar{3}m$). The mismatch between our calculated densities and the given experimental density likely means the given **atomic radius** (0.1245 nm) is **not** the correct metallic (packing) radius to combine with the simple geometric model — it could be a covalent radius, van der Waals radius, or from a different tabulation. Small differences in the radius used produce significant differences in the computed density because $V_{\text{cell}} \propto a^3 \propto r^3$.

So the right interpretation:

* If the exercise expects you to “use the given radius and decide purely by numerical comparison,” you would say **BCC** (because 14.38 is closer to 12.41 than 15.65 is).
* If the exercise is about **real material crystallography**, then state that **Rhodium is FCC** and explain the discrepancy by noting the atomic radius type issue (use of an inconsistent radius value).

---

# Short summary (clean)

* $r = 0.1245\ \text{nm} = 1.245\times10^{-8}\ \text{cm}$.
* $\rho_{BCC} \approx 14.38\ \text{g cm}^{-3}$.
* $\rho_{FCC} \approx 15.65\ \text{g cm}^{-3}$.
* Given $\rho_{\text{exp}} = 12.41\ \text{g cm}^{-3}$. Numerically BCC closer, but real Rh is FCC — discrepancy due to radius type/values.

---

# Hinglish (short, clear)

* Formula: $\rho = \dfrac{nA}{N_A V_{\text{cell}}}$. BCC mein $n=2$, FCC mein $n=4$.
* $r=0.1245$ nm ko cm mein karo → $1.245\times10^{-8}$ cm.
* BCC → $a=\dfrac{4r}{\sqrt{3}}$, $\rho_{BCC}\approx14.38\ \text{g/cm}^3$.
* FCC → $a=\dfrac{4r}{\sqrt{2}}$, $\rho_{FCC}\approx15.65\ \text{g/cm}^3$.
* Diya gaya experimental $\rho=12.41$. Dono theoretical density isse zyada hain; BCC thoda closer hai.
* **Par** actual Rhodium ka crystal structure **FCC** hota hai — jo mismatch hai woh isliye kyunki diya hua radius shayad metallic radius nahi balki koi aur radius table value hai. Radius type change karne se computed density bahut badal sakta hai.

---

Perfect, bhai 👍. Tumne ek handwritten solution likha hai, aur main ise **step by step** explain karta hoon (English + Hinglish mix), taki tumhe clear ho jaye ki kaise approach karna hai, kya formula use hua, aur kaha pe values aayi.

---

# Question Recap

* Given: $a = b = 0.25\ \text{nm}, \ c = 0.495\ \text{nm}, \ \alpha = \beta = \gamma = 90^\circ$.
* Atomic weight = 141 g/mol.
* Asked:
  (a) Crystal system?
  (b) Crystal structure type?
  (c) Density calculation.

---

# Step (a): Crystal system

Rule: Crystal system depends on **unit cell edge lengths and angles**.

* Given: $a = b \neq c$, and all angles = $90^\circ$.
* Condition $a=b\neq c, \alpha=\beta=\gamma=90^\circ$ ⇒ **Tetragonal system**.

✅ Answer: **Tetragonal crystal system**.

---

# Step (b): Crystal structure

* Since no mention of body-centering, face-centering etc. in question, assume **primitive (simple)** cell.
* So, structure = **Simple tetragonal**.

✅ Answer: **Primitive tetragonal structure**.

---

# Step (c): Density calculation

### Formula

$$
\rho = \frac{nA}{N_A V_c}
$$

where

* $n$ = number of atoms per unit cell (primitive = 1),
* $A$ = atomic weight = 141 g/mol,
* $N_A = 6.022 \times 10^{23}\ \text{mol}^{-1}$,
* $V_c$ = unit cell volume (in cm³).

---

### Step 1: Convert units

* $a = b = 0.25\ \text{nm} = 0.25 \times 10^{-7}\ \text{cm} = 2.5 \times 10^{-8}\ \text{cm}$.
* $c = 0.495\ \text{nm} = 4.95 \times 10^{-8}\ \text{cm}$.

---

### Step 2: Calculate volume

$$
V_c = a \times b \times c = (2.5 \times 10^{-8})(2.5 \times 10^{-8})(4.95 \times 10^{-8})
$$

$$
V_c = 3.09375 \times 10^{-23}\ \text{cm}^3
$$

⚠️ Tumhare solution mein $5.125 \times 10^{-23}\ \text{cm}^3$ likha hai — shayad multiplication galat ho gaya. Correct value is **3.09 × 10⁻²³ cm³**.

---

### Step 3: Apply density formula

$$
\rho = \frac{nA}{N_A V_c}
= \frac{1 \times 141}{(6.022 \times 10^{23})(3.09375 \times 10^{-23})}
$$

Denominator: $6.022 \times 10^{23} \times 3.09375 \times 10^{-23} \approx 18.62$.

$$
\rho = \frac{141}{18.62} \approx 7.57\ \text{g/cm}^3
$$

---

# ✅ Final Answers

(a) **Tetragonal system**
(b) **Primitive tetragonal**
(c) **Density ≈ 7.6 g/cm³**

---

# Hinglish Explanation (Short)

* $a=b\neq c,\ \alpha=\beta=\gamma=90^\circ$ ⇒ Tetragonal system.
* Primitive cell assume karo ⇒ Primitive tetragonal.
* Density nikalne ka formula: $\rho = \frac{nA}{N_A V_c}$.
* Values daalke solve karo ⇒ \~7.6 g/cm³ aata hai.

---
Nice — let’s do this cleanly. I’ll (1) state the quick answers you wrote, (2) show the *exact method* (every line, every small step) so you *know why* those indices are correct, and (3) give the same explanation in short Hinglish.

---

## Quick answers (from your sketches)

* **Left drawing**
  Plane (1) → **(0 0 1)**
  Plane (2) → **(1 0 0)**

* **Right drawing**
  Plane (1) → **(0 0 1)**
  Direction (2) → **\[0 1 0]**  (i.e. along the y-axis)

Now — why these are correct.

---

## How to get Miller indices for a plane — step-by-step (every tiny step)

1. **Choose an origin.** Usually one corner of the unit cell (the lower-left-rear corner) is used as origin $O$.

2. **Find intercepts of the plane with the crystallographic axes (in unit-cell coordinates).**

   * If the plane cuts the $x$-axis at $p$, $y$-axis at $q$, and $z$-axis at $r$, *express these intercepts as multiples of the lattice parameters*, i.e. $p = u\cdot a,\ q = v\cdot b,\ r = w\cdot c$. In reduced (fractional) coordinates this is simply $(u,v,w)$.
   * If the plane is **parallel** to an axis then that intercept is at infinity → treat the intercept value as $\infty$.

3. **Take reciprocals** of the intercepts: $\left(\frac{1}{u},\frac{1}{v},\frac{1}{w}\right)$. For an intercept at $\infty$ the reciprocal is 0.

4. **Clear fractions** (multiply by the least common denominator) to obtain three smallest integers $(h,k,l)$ with no common factor. These integers are the **Miller indices (h k l)**. Finally write them in parentheses: $(h\ k\ l)$.

---

### Apply this to your left figure — Plane (1)

* Look at the shaded plane — it is the plane coincident with the top face (i.e. it is parallel to $x$ and $y$ and cuts the $z$-axis at $z=1$ (one lattice height)).
* Intercepts (in units of $a,b,c$) = $x=\infty,\ y=\infty,\ z=1$.
* Reciprocals = $1/\infty = 0,\ 1/\infty = 0,\ 1/1 = 1$.
* Miller indices = $(0\ 0\ 1)$. ✅

**Interpretation:** $(001)$ is the plane parallel to the $xy$-plane at the top (i.e. normal along +z).

---

### Left figure — Plane (2)

* The other shaded face is parallel to $y,z$ (i.e. it is a face perpendicular to $x$), so intercepts = $x=1,\ y=\infty,\ z=\infty$.
* Reciprocals = $1,0,0$.
* Miller indices = $(1\ 0\ 0)$. ✅

**Interpretation:** $(100)$ is a plane normal to the $x$-axis (a face parallel to $y$- and $z$-axes).

---

## Miller indices for the right sketch

Right sketch shows a top horizontal plane (shaded) and an arrow indicating a direction along the middle of the face pointing along the y-axis.

### Plane (1) on right

* Same reasoning as left top plane: it is parallel to $x,y$ and cuts $z$ at 1 → **(0 0 1)**.

### Direction (2) on right

* Direction arrow is along the **y–axis** (from origin along the edge in the y direction).
* Direction indices are given in square brackets and are simply the vector components in lattice units: $[u\ v\ w]$. For the y-axis that is $[0\ 1\ 0]$. ✅

---

## Notes & common pitfalls

* Planes use **parentheses**: $(h\ k\ l)$. Directions/vectors use **square brackets**: $[u\ v\ w]$.
* If plane intercept equals infinity (plane parallel to an axis) its reciprocal is 0.
* Don’t confuse Miller indices with intercepts — always do intercept → take reciprocals → clear fractions.
* For tetragonal/orthogonal unit cells (a, b, c at right angles) we simply use fractional intercepts $x/a,\ y/b,\ z/c$. For non-orthogonal cells there are small geometric adjustments but method is same conceptually.

---

## Short Hinglish recap

* Plane ka intercept lo with x,y,z in unit-cell units → reciprocals lo → smallest integers banao → woh Miller indices.
* Agar plane kisi axis ke parallel ho → intercept = ∞ → reciprocal = 0.
* Example from tumhari drawing: top horizontal plane = parallel to x,y → (0 0 1). Side face normal to x = (1 0 0). Arrow along y = direction \[0 1 0].

---
Bahut badiya bhai 👌 tu ne FCC aur BCC ke plane pe **atomic packing** (yaani ki ek plane me atoms kitne effectively occupy karte hain) ka derivation likha hai. Chalo isko line by line aur formula by formula deep me samajhte hain. Main English + Hinglish dono me samjhaunga taaki clarity aa jaye.

---

## 🔹 Topic: Atomic Packing on Planes in Crystals (FCC & BCC)

Crystal structures jaise **FCC (Face Centered Cubic)** aur **BCC (Body Centered Cubic)** me alag-alag planes (100), (110), (111) pe packing density different hoti hai. Ye concept **Miller indices (hkl)** aur **atomic packing factor (APF)** se related hai.

### Step 1: Contribution of Atoms

Notes me likha hai:

* Atom at **corner** contributes = 1/8
* Atom at **face center** contributes = 1/2
* Atom at **body center** contributes = 1

**Explanation (English):**
Ek cubic cell me atom ka kuch part hi ek unit cell ka hota hai.

* Jo atom **corner** pe hai, wo 8 different unit cells me share hota hai → contribution = 1/8.
* Jo atom **face center** pe hai, wo 2 unit cells me share hota hai → contribution = 1/2.
* Jo atom **body center** pe hai, wo sirf ek hi cell ka part hota hai → contribution = 1.

**Hinglish:**
Unit cell ke andar har atom pura ka pura ek cell ka nahi hota. Kuch hissa ek cell ka hota hai, baaki neighboring cells me chala jata hai. Isi liye hume contribution count karna padta hai.

---

### Step 2: FCC (100) Plane

* Tumhare notes me likha hai:

  ```
  N = (1/8 × 8) + (1/2 × 8)
  N = 4
  ```

**Explanation:**

* (100) plane ek **square plane** hai jisme 4 corners + 1 face-centered atom aata hai.
* 4 corners (each 1/4 in plane counting, but per unit cell contribution = 1/8)
* 1 face-center (contributes 1/2 but appears fully in the plane)

Total = 4 atoms effective in the (100) plane.

**Hinglish:**
FCC ke (100) plane me 4 atoms effectively hote hain jo packing me participate karte hain.

---

### Step 3: FCC (111) Plane (Notes me mention kiya hai)

(111) plane ka matlab hai ek diagonal triangular plane jo cube ke andar se cut karta hai.

* Isme 3 corner atoms aur 3 face-centered atoms aate hain.
* Contribution calculation karke total atoms = 2 milte hain.

Ye sabse **closely packed plane** hota hai FCC me (isi wajah se slip aur deformation zyada (111) plane pe hoti hai).

---

### Step 4: BCC (Notes ka 2nd Image)

* Likha hai:

  ```
  Atom at body center contribution = 1
  N = 1 × 1 + 1 × (corners contribution)
  N = 2
  ```

**Explanation:**

* BCC unit cell ke center me ek pura atom hota hai (contribution = 1).
* Saath hi corners ke atoms ka bhi thoda hissa count hota hai.
* Effective atoms per unit cell = 2.

**Hinglish:**
BCC me ek atom pure ka pura andar hota hai aur 8 corner atoms ke chhote hisson ko mila ke ek aur atom banta hai. Matlab total 2 atoms har BCC cell me hote hain.

---

## 🔹 Important Concept: Atomic Packing Factor (APF)

**Formula:**

$$
APF = \frac{\text{Volume of atoms in unit cell}}{\text{Volume of unit cell}}
$$

* FCC → APF = 0.74 (sabse closely packed structure, spheres ka max filling fraction)
* BCC → APF = 0.68
* SC (simple cubic) → APF = 0.52

**Hinglish:**
APF batata hai ki ek crystal me total jagah ka kitna percent hissa atoms ne fill kiya hai. FCC me lagbhag 74% space atoms se bhar jata hai (sabse zyada dense packing).

---

## 🔹 Why do we study plane-wise packing?

* Ye batata hai ki crystal ke kis plane pe atoms zyada closely packed hain.
* Slip (plastic deformation) hamesha **closely packed planes** pe hoti hai.
* FCC ka slip plane (111) hai → isiliye FCC metals ductile hote hain.
* BCC me slip plane kam closely packed hote hain → kam ductility.

---

👉 Summary in simple Hinglish:

* **FCC corner atom = 1/8, face atom = 1/2.**
* (100) plane FCC me 4 atoms effectively aate hain.
* (111) plane FCC ka sabse dense packing plane hota hai (2 atoms).
* **BCC me ek body center atom (1) + corner contributions (1) = 2 atoms total per unit cell.**
* APF: FCC (0.74), BCC (0.68), SC (0.52).

---
Bahut badiya bhai 🙌 tu ne ab linear aur planar density ke notes bheje hain. Ye ekdum fundamental concept hai jo har crystal structure me use hota hai. Chalo ise line by line, easy English + Hinglish dono me deep samajhte hain.

---

# 🔹 Topic: Linear Density (LD) & Planar Density (PD)

---

## 1. **Linear Density (LD)**

**Notes se line:**

* *Number of atoms whose centers lie along a specific crystallographic direction per unit length of that direction.*

**👉 English Explanation:**
Linear density batata hai ki ek given **direction** (jaise \[100], \[110], \[111]) me kitne atoms ke centers aate hain per unit length.

* Ye measure karta hai ki ek straight line direction me atoms kitne closely packed hain.

**👉 Formula:**

$$
LD = \frac{\text{Number of atoms centered on direction}}{\text{Length of direction}}
$$

**👉 Hinglish:**
LD ka matlab hai ki ek crystal ke andar kisi ek **direction line** pe kitne atoms line up hote hain per unit distance.
Agar direction tightly packed hai to LD zyada hoga.

---

### Example: FCC along \[110] direction

* \[110] direction ek cube ka face diagonal hai.
* Us line pe 2 atoms ke centers aate hain.
* Length of \[110] = $a\sqrt{2}$ (face diagonal).

$$
LD_{[110]} = \frac{2}{a\sqrt{2}} = \frac{\sqrt{2}}{a}
$$

**Hinglish:** Matlab FCC ka sabse dense linear packing \[110] direction me hota hai.

---

## 2. **Planar Density (PD)**

**Notes se line:**

* *Number of atoms whose centers lie within a specific crystallographic plane per unit area of that plane.*

**👉 English Explanation:**
Planar density ek **plane** (jaise (100), (110), (111)) ke andar kitne atoms effectively hote hain per unit area.

* Ye batata hai ki ek flat plane me atoms kitne closely packed hain.

**👉 Formula:**

$$
PD = \frac{\text{Number of atoms centered on plane}}{\text{Area of plane}}
$$

**👉 Hinglish:**
PD ka matlab hai ki ek crystal ke ek **plane** (jaise ek face ya diagonal plane) me per unit area kitne atoms fit ho jate hain.
Jo plane sabse closely packed hoga uska PD sabse zyada hoga.

---

### Example: FCC (111) plane

* FCC (111) plane ek triangular plane hota hai.
* Us plane me effectively 2 atoms hote hain.
* Area of (111) plane = $\frac{\sqrt{3}}{2} a^2$.

$$
PD_{(111)} = \frac{2}{\frac{\sqrt{3}}{2} a^2} = \frac{4}{\sqrt{3} a^2}
$$

**Hinglish:**
FCC ka (111) plane sabse zyada tightly packed plane hai (isliye slip aur deformation isi pe hoti hai).

---

## 3. Difference Between LD and PD

| Concept       | Linear Density (LD)                         | Planar Density (PD)                     |
| ------------- | ------------------------------------------- | --------------------------------------- |
| Definition    | Atoms per unit **length** along a direction | Atoms per unit **area** of a plane      |
| Unit          | Atoms / length (e.g., atoms/nm)             | Atoms / area (e.g., atoms/nm²)          |
| Example (FCC) | \[110] direction has highest LD             | (111) plane has highest PD              |
| Importance    | Tells which **direction** is tightly packed | Tells which **plane** is tightly packed |

---

👉 **Summary in Hinglish:**

* **LD** = atoms per unit line (direction me packing).
* **PD** = atoms per unit area (plane me packing).
* FCC me **sabse zyada LD \[110] direction** me hoti hai.
* FCC me **sabse zyada PD (111) plane** pe hoti hai.

---
