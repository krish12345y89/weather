# Explanation (English + Hinglish) — step by step

**Problem summary:**
Atomic radius of Al (FCC) = **0.143 nm**. Find number of unit cells in **1 m³**.

---

## 1) Convert units (why?)

We must work in metres because final answer asked per cubic **metre**.

0.143 nm = $0.143\times10^{-9}\ \text{m} = 1.43\times10^{-10}\ \text{m}$.
(Explanation: 1 nm = $10^{-9}$ m.)

**Hinglish:** unit nm ko metre mein convert karna zaroori hai kyunki hum final answer per cubic **metre** chahte hain.

---

## 2) Relation between atomic radius $r$ and lattice parameter $a$ for FCC (why this formula?)

In an FCC unit cell, atoms touch along the face diagonal. Along one face diagonal there are: corner atom radius + corner atom radius + face-centered atom diameter = $4r$. The face diagonal length geometrically is $a\sqrt{2}$.
So:

$$
a\sqrt{2} = 4r \quad\Rightarrow\quad a=\dfrac{4r}{\sqrt{2}}
$$

**Hinglish:** FCC mein atoms face diagonal pe touch karte hain, isliye face diagonal = $4r$, aur face diagonal = $a\sqrt2$. Is se $a=4r/\sqrt2$ milta hai.

Now plug $r=1.43\times10^{-10}\ \text{m}$:

$$
a=\frac{4\times1.43\times10^{-10}}{\sqrt{2}}
=4.04465\times10^{-10}\ \text{m}
$$

---

## 3) Volume of one cubic unit cell (why $a^3$?)

Unit cell is a cube of edge $a$, so its volume:

$$
V_{\text{cell}}=a^3
$$

Compute:

$$
V_{\text{cell}}=(4.04465\times10^{-10}\ \text{m})^3
\approx 6.6167\times10^{-29}\ \text{m}^3
$$

**Hinglish:** cube ka volume edge ka cube hota hai, isliye $a^3$.

---

## 4) Number of unit cells per cubic metre (why divide?)

One unit cell occupies $V_{\text{cell}}$ m³, so how many such cells fit in 1 m³ = $\dfrac{1\ \text{m}^3}{V_{\text{cell}}}$.

$$
N=\frac{1}{6.6167\times10^{-29}}\approx 1.511\times10^{28}
$$

So final answer:

$$
\boxed{1.51\times10^{28}\ \text{unit cells per m}^3}
$$

**Hinglish (summary):**

1. nm ko metre mein convert kiya.
2. FCC geometry se $a=4r/\sqrt2$ use kiya.
3. Unit cell ka volume $a^3$ nikala.
4. 1 m³ ko us volume se divide karke unit cells per cubic metre mil gaye: **$1.51\times10^{28}$**.

---

**Extra note (optional):** FCC unit cell contains 4 atoms (1 from corners net + 3 from faces net), so if you wanted atoms per m³ you would multiply this cell count by 4.

Bhai ab mai iske solution ko step-by-step **English + Hinglish** mein explain karta hoon, taki tujhe clearly samajh aaye ki kaunsa formula kyon use hua aur ideal $\dfrac{c}{a}$ ratio HCP structure mein kaise aata hai.

---

# **Question:**

For HCP crystal structure, show that ideal $\dfrac{c}{a}$ ratio = **1.633**

---

## 1) Background (Why this ratio matters?)

* In **HCP (Hexagonal Close Packed)**, the unit cell has:

  * **a** = side length of hexagon (base edge)
  * **c** = height of the hexagonal prism (distance between two bases).
* The ratio $\dfrac{c}{a}$ tells how "tall" or "flat" the HCP cell is.
* The **ideal ratio** comes from close-packing geometry when spheres (atoms) are touching.

**Hinglish:**
HCP structure ek hexagonal prism jaisa hota hai. Uski base ka side = $a$, aur prism ki height = $c$. Ideal $c/a$ ratio tab milega jab atoms bilkul close pack ho (jaise billiard balls ko tight pack karte hain).

---

## 2) Geometric model (Tetrahedron inside HCP)

To derive, we consider a **tetrahedron** formed by:

* 3 atoms at the corners of one equilateral triangle (base)
* 1 atom sitting above at the next layer.

**Soch:** bottom layer mein 3 atoms ek equilateral triangle banate hain, aur next layer ka ek atom unke upar aata hai. Yeh 4 atoms ek **regular tetrahedron** banate hain.

---

## 3) Step 1 – Height of equilateral triangle

Equilateral triangle side = $a$.
Height of equilateral triangle:

$$
h = \sqrt{a^2 - \left(\tfrac{a}{2}\right)^2} = \frac{\sqrt{3}}{2}a
$$

**Hinglish:** triangle ki height nikalne ka normal formula hai $\sqrt{a^2 - (a/2)^2}$.

---

## 4) Step 2 – Distance from triangle center to atom above

From symmetry, the top atom sits **above the centroid** of triangle.

Distance from centroid to one vertex =

$$
\frac{2}{3}\times \text{height} = \frac{2}{3}\times \frac{\sqrt{3}}{2}a = \frac{a}{\sqrt{3}}
$$

**Hinglish:** centroid hamesha height ke $2/3$ distance pe hota hai, isliye vertex se centroid tak distance $a/\sqrt{3}$.

---

## 5) Step 3 – Tetrahedron height relation

Now form a right triangle:

* One side = distance from centroid to vertex = $a/\sqrt{3}$
* Other side = vertical height of tetrahedron = $c/2$ (half of full $c$, because atom lies halfway between top and bottom).
* Hypotenuse = atomic diameter = $a$.

So by Pythagoras:

$$
\left(\frac{c}{2}\right)^2 + \left(\frac{a}{\sqrt{3}}\right)^2 = a^2
$$

---

## 6) Step 4 – Solve for $c/a$

$$
\frac{c^2}{4} = a^2 - \frac{a^2}{3} = \frac{2a^2}{3}
$$

$$
c^2 = \frac{8}{3}a^2
$$

$$
\frac{c}{a} = \sqrt{\frac{8}{3}} = 1.633
$$

---

# **Final Answer:**

$$
\boxed{\dfrac{c}{a} = 1.633}
$$

---

## **Hinglish Summary:**

* HCP unit cell ko samajhne ke liye 4 atoms (3 niche + 1 upar) ko tetrahedron ke form mein liya.
* Equilateral triangle ka height $\sqrt{3}a/2$ nikala.
* Centroid se vertex ka distance $a/\sqrt{3}$.
* Pythagoras lagaya: $(c/2)^2 + (a/\sqrt{3})^2 = a^2$.
* Solve karne par ideal $\dfrac{c}{a} = 1.633$ milta hai.

---

Bhai, kya tu chahata hai mai is derivation ka **diagrammatic step-by-step explanation (with tetrahedron geometry)** bana kar bhi dikhau taaki aur crystal clear ho jaye?
Bhai isme tumhare notes mein **APF (Atomic Packing Factor)** ke derivations diye hain for BCC, FCC aur HCP. Main ab isko **English + Hinglish** mein step-by-step explain kar deta hoon ki kaunsa formula kyon use ho raha hai aur final result kaise aata hai.

---

# **Concept: What is APF?**

$$
\text{APF} = \frac{\text{Volume of atoms in unit cell}}{\text{Volume of unit cell}}
$$

**Hinglish:**
APF matlab packing efficiency — ek unit cell ke andar kitni jagah atoms ki solid spheres ne cover ki hai aur kitni khali bachi hai.

---

# **1) BCC (Body Centered Cubic)**

* **Atoms per unit cell:** 2 (1 from 8 corners × 1/8 + 1 from body center).

* **Relation between $a$ and $r$:**
  In BCC, atoms touch along the **body diagonal**.
  Body diagonal = $4r = \sqrt{3}a $
  So,

  $$
  a = \frac{4r}{\sqrt{3}}
  $$

* **Volume of atoms in cell:**
  $2 \times \frac{4}{3}\pi r^3 = \frac{8}{3}\pi r^3$

* **Volume of cell:**
  $a^3 = \left(\frac{4r}{\sqrt{3}}\right)^3 = \frac{64r^3}{3\sqrt{3}}$

* **APF calculation:**

  $$
  APF_{BCC} = \frac{\frac{8}{3}\pi r^3}{\frac{64}{3\sqrt{3}}r^3}
  = \frac{\pi \sqrt{3}}{8} \approx 0.680
  $$

✅ **BCC APF = 0.68 (68% packing).**

**Hinglish:** BCC mein packing loose hoti hai, isliye 68% hi space atoms bharte hain.

---

# **2) FCC (Face Centered Cubic)**

* **Atoms per unit cell:** 4 (1 from corners + 3 from faces).

* **Relation between $a$ and $r$:**
  Atoms touch along **face diagonal**.
  Face diagonal = $4r = \sqrt{2}a$
  So,

  $$
  a = \frac{4r}{\sqrt{2}} = 2\sqrt{2}r
  $$

* **Volume of atoms in cell:**
  $4 \times \frac{4}{3}\pi r^3 = \frac{16}{3}\pi r^3$

* **Volume of cell:**
  $a^3 = (2\sqrt{2}r)^3 = 16\sqrt{2}r^3$

* **APF calculation:**

  $$
  APF_{FCC} = \frac{\frac{16}{3}\pi r^3}{16\sqrt{2}r^3}
  = \frac{\pi}{3\sqrt{2}} \approx 0.740
  $$

✅ **FCC APF = 0.74 (74% packing).**

**Hinglish:** FCC sabse dense cubic packing hai, isliye maximum efficiency 74%.

---

# **3) HCP (Hexagonal Close Packed)**

* **Atoms per unit cell:** 6 (kaise? → 12 corners × 1/6 + 2 faces × ½ + 3 inside = 6).

* **Base area of hexagon:**
  A hexagon with side $a$ can be divided into 6 equilateral triangles.

  $$
  A_{hexagon} = 6 \times \frac{\sqrt{3}}{4}a^2 = \frac{3\sqrt{3}}{2}a^2
  $$

* **Volume of HCP cell:**

  $$
  V_{cell} = A_{base} \times c = \frac{3\sqrt{3}}{2}a^2c
  $$

  (and for ideal HCP, $c/a = 1.633$).

* **Volume of atoms in cell:**
  $6 \times \frac{4}{3}\pi r^3 = 8\pi r^3$

* **Relation between $a$ and $r$:**
  In HCP, atoms touch in the base plane:

  $$
  a = 2r
  $$

* **Final APF:**
  After simplification (using $c/a=1.633$),

  $$
  APF_{HCP} \approx 0.740
  $$

✅ **HCP APF = 0.74 (same as FCC).**

**Hinglish:** FCC aur HCP dono close packing structure hain, dono ka APF equal = 74%.

---

# **Final Results:**

* $APF_{BCC} = 0.68$
* $APF_{FCC} = 0.74$
* $APF_{HCP} = 0.74$

---

👉 Bhai, kya tu chahta hai mai inko ek **comparison chart + simple diagrams** bana kar bhi dikhau (taaki ek glance mein samajh aa jaye difference BCC, FCC aur HCP packing ka)?
Bhai chalo ab is wale question ko detail mein step-by-step samajhte hain (English + Hinglish), taki clear ho jaye har formula kyon use hua aur final result kaise aya.

---

# **Question:**

Calculate the radius of Sodium atom, given:

* Crystal structure = FCC
* Density = $2.24 \, \text{g/cm}^3$
* Atomic weight = $ 192.2 \, \text{g/mol}$

---

# **Step 1 – Concept**

We use density formula for a crystal:

$$
\rho = \frac{n \cdot M}{N_A \cdot a^3}
$$

Where:

* $\rho$ = density
* $n$ = number of atoms per unit cell (FCC → $n=4$)
* $M$ = molar mass (g/mol)
* $N_A$ = Avogadro’s number = $6.022 \times 10^{23}$ atoms/mol
* $a$ = lattice parameter (edge length of unit cell)

**Hinglish:** Density ka relation unit cell se yeh hai ki ek cube ka volume ($a^3$) aur uske andar kitne atoms hain uske hisaab se average density nikalti hai.

---

# **Step 2 – Rearrange for $a^3$:**

$$
a^3 = \frac{n \cdot M}{\rho \cdot N_A}
$$

Put values:

$$
a^3 = \frac{4 \times 192.2}{2.24 \times 6.022 \times 10^{23}}
$$

$$
a^3 \approx 5.70 \times 10^{-23} \, \text{cm}^3
$$

Take cube root:

$$
a \approx 3.84 \times 10^{-8} \, \text{cm}
= 3.84 \, \text{Å}
$$

---

# **Step 3 – Relation between $a$ and $r$ (FCC)**

For FCC:
Atoms touch along face diagonal →

$$
\sqrt{2}a = 4r \quad \Rightarrow \quad r = \frac{a}{2\sqrt{2}}
$$

**Hinglish:** FCC mein 4 atoms ek face diagonal par lagte hain, isliye relation aata hai $4r = \sqrt{2}a$.

---

# **Step 4 – Calculate atomic radius**

$$
r = \frac{3.84}{2\sqrt{2}} \, \text{Å}
= \frac{3.84}{2 \times 1.414} 
= \frac{3.84}{2.828}
$$

$$
r \approx 1.36 \, \text{Å} = 0.136 \, \text{nm}
$$

---

# ✅ **Final Answer:**

$$
\boxed{r \approx 0.136 \, \text{nm}}
$$

---

### **Quick Hinglish Recap:**

1. Density formula use kiya: $\rho = \frac{nM}{N_A a^3}$.
2. Isse $a^3$ nikala → $a = 3.84 \, \text{Å}$.
3. FCC relation use kiya: $4r = \sqrt{2}a$.
4. Radius aaya: **0.136 nm**.

---
Chalo — step-by-step karte hain (English + Hinglish) — taaki clearly pata chale kya compute hua, kyu mismatch aa sakta hai, aur final conclusion kya hogi.

**Given**

* Atomic radius of Rhodium $r = 0.1245\ \text{nm} = 0.1245\times10^{-9}\ \text{m}$
* Density (experimental) $\rho_{\text{given}} = 12.41\ \text{g cm}^{-3} = 12410\ \text{kg m}^{-3}$
* Atomic (molar) mass $M \approx 102.91\ \text{g mol}^{-1} = 102.91\times10^{-3}\ \text{kg mol}^{-1}$
* $N_A = 6.022\times10^{23}\ \text{mol}^{-1}$

---

## Formula we use

$$
\rho = \frac{nM}{N_A a^3}
$$

where $n$ = atoms/unit cell (BCC → 2, FCC → 4), and $a$ (lattice parameter) relates to $r$ differently for BCC and FCC:

* **BCC:** body diagonal = $4r = \sqrt{3}\,a \Rightarrow a=\dfrac{4r}{\sqrt{3}}$.
* **FCC:** face diagonal = $4r = \sqrt{2}\,a \Rightarrow a=\dfrac{4r}{\sqrt{2}}$.

We compute theoretical $\rho$ for both structures using the given $r$.

---

## Calculation (numbers)

Convert inputs to SI and plug in:

1. For **BCC**:

* $a_{\text{BCC}} = \dfrac{4r}{\sqrt{3}} = \dfrac{4\times0.1245\times10^{-9}}{\sqrt3}= $ (use directly in volume).
* Volume $V_{\text{cell,BCC}} = a^3$.
* $n=2$.
* $\rho_{\text{BCC}} = \dfrac{2M}{N_A a^3}$.

Numerical result:

$$
\rho_{\text{BCC}}\approx 14.38\ \text{g cm}^{-3}.
$$

2. For **FCC**:

* $a_{\text{FCC}} = \dfrac{4r}{\sqrt{2}}$.
* $V_{\text{cell,FCC}} = a^3$.
* $n=4$.
* $\rho_{\text{FCC}} = \dfrac{4M}{N_A a^3}$.

Numerical result:

$$
\rho_{\text{FCC}}\approx 15.65\ \text{g cm}^{-3}.
$$

(You can check: I used $M=102.91\times10^{-3}\ \text{kg mol}^{-1},\ N_A=6.022\times10^{23}$, $r=0.1245\times10^{-9}\ \text{m}$.)

---

## Compare with given density

* Given (experimental) $\rho_{\text{exp}} = 12.41\ \text{g cm}^{-3}$.
* $|\rho_{\text{exp}}-\rho_{\text{BCC}}| \approx 1.97\ \text{g cm}^{-3}$.
* $|\rho_{\text{exp}}-\rho_{\text{FCC}}| \approx 3.24\ \text{g cm}^{-3}$.

So with the **given** atomic radius $0.1245\ \text{nm}$, the **BCC** theoretical density is numerically **closer** to the given density than FCC — but neither matches well.

---

## Important physical note (why mismatch can happen)

* **“Atomic radius”** can mean different things (covalent radius, metallic radius, van der Waals radius, ionic radius). The relation $a$–$r$ we used assumes **metallic (contact) radius** where atoms touch along diagonals. If the provided $r$ is *not* the metallic radius, the density computed from it will be wrong.
* Experimental lattice parameter (and thus density calculated from the true metallic radius) is the correct way to decide structure.
* Also experimental density may include thermal expansion / measurement differences.

If we instead ask: *what radius would make FCC match the experimental density?* — solving the density formula for $r$ (FCC) with $\rho=12.41\ \text{g/cm}^3$ gives

$$
r_{\text{required,FCC}}\approx 0.1345\ \text{nm}.
$$

So a metallic radius ≈ **0.1345 nm** would make the FCC formula reproduce the experimental density.

---

## Final conclusion (straight answer)

* Using the **given** radius $0.1245\ \text{nm}$, the **computed** densities are:

  * BCC ≈ **14.38 g/cm³**
  * FCC ≈ **15.65 g/cm³**
    → **BCC** result is numerically closer to the given 12.41 g/cm³, but still not a good match.
* **Physically**, Rhodium is a **face-centred cubic (FCC)** metal. The mismatch here most likely comes from the type/value of the atomic radius you used — use the metallic radius (or measured lattice parameter) to get consistent results. If you plug $r\approx0.1345$ nm into the FCC formulas you recover the experimental density 12.41 g/cm³.

---

## Short Hinglish summary

* Tumne jo $r=0.1245$ nm diya, us se BCC walā calculation experimentally diye gaye 12.41 g/cm³ se zyaada **closer** aaya, lekin dono (BCC/FCC) match achhe se nahi kar rahe.
* Yeh mismatch isliye hai kyunki **“atomic radius”** ka matlab alag-alag tarah se liya ja sakta hai — metallic radius chahiye tha.
* Real Rhodium **FCC** hota; agar tum FCC ke liye metallic radius $≈0.1345$ nm use karoge to experimental density mil jayegi.

Agar chaho to main:

1. Yahan saare intermediate numeric steps likh kar deta hoon (with each numeric substitution),
2. Ya ek chhota diagram bana ke $a$–$r$ relations dikhau,
3. Aur/ya tumhara diya hua radius kis type ka ho sakta hai (covalent vs metallic) uska short table bata doon — bol do jo chahte ho.
Nice — chalo step-by-step solve karte hain (English **+** Hinglish), saare formulas aur unit conversions clear likh ke.

---

# Given

* $a=b=0.25\ \text{nm}$ and $c=0.45\ \text{nm}$
* $\alpha=\beta=\gamma=90^\circ$
* Atomic weight $M = 51\ \text{g mol}^{-1}$

---

## (a) Which crystal system?

**English:** All angles 90° and $a=b$ but $c\neq a$ → this is a **tetragonal** system.
**Hinglish:** Sab angles 90° hain, base edges equal hain lekin height different — isliye **tetragonal**.

---

## (b) What crystal structure (Bravais type)?

**English:** No centering is mentioned, so it’s a **primitive (simple) tetragonal** unit cell — one lattice point (atom) per cell.
**Hinglish:** Centering ka zikr nahi hai, isliye simple/prmitive tetragonal maana jayega — ek atom per unit cell (net).

---

## (c) Density calculation (step-by-step)

**Formula:**

$$
\rho=\frac{n\;M}{N_A\;V_{\text{cell}}}
$$

where $n$ = atoms per cell (primitive → 1), $N_A=6.022\times10^{23}\ \text{mol}^{-1}$.

**Unit conversion:** convert nm → cm because density in g/cm³ common:

$$
1\ \text{nm}=10^{-7}\ \text{cm}
$$

So

$$
a=0.25\ \text{nm}=0.25\times10^{-7}\ \text{cm}=2.5\times10^{-8}\ \text{cm}
$$

$$
c=0.45\ \text{nm}=4.5\times10^{-8}\ \text{cm}
$$

**Unit cell volume (tetragonal):** $V=a^2c$

$$
V=(2.5\times10^{-8}\,\text{cm})^2\times(4.5\times10^{-8}\,\text{cm})
=2.8125\times10^{-23}\ \text{cm}^3
$$

**Plug into density formula:** $n=1$

$$
\rho=\frac{1\times 51\ \text{g/mol}}{6.022\times10^{23}\ \text{mol}^{-1}\times 2.8125\times10^{-23}\ \text{cm}^3}
$$

Do the arithmetic:

$$
\rho \approx 3.01\ \text{g/cm}^3
$$

**Hinglish summary of calculation:**

* $V=a^2c = 2.8125\times10^{-23}\ \text{cm}^3$.
* Ek cell mein 1 atom hai, isliye $\rho = \dfrac{51}{6.022\times10^{23}\times V}$.
* Final $\rho \approx 3.01\ \text{g/cm}^3$.

---

## Final answers

(a) **Tetragonal**.
(b) **Primitive (simple) tetragonal** structure (1 atom per cell).
(c) **Density ≈ 3.01 g·cm⁻³**.

---
Bhai, tumhare notes bilkul sahi direction mein hain 👍
Main tumhe aur **deep samjhata hoon (English + Hinglish dono)** with clarity, formulas, aur logical meaning.

---

# **Linear Density (LD)**

### **Definition (English):**

Linear density is the **number of atoms whose centers lie on a specific crystallographic direction per unit length of that direction.**

$$
LD = \frac{\text{No. of atoms centered on direction}}{\text{Length of direction}}
$$

### **Meaning (Hinglish):**

Linear density matlab ek **line (crystal direction)** ke along atoms kitne closely packed hain.
Jitna zyada LD hoga → utna zyada tightly packed line hogi → stronger slip direction (dislocations easily move there).

---

### **Example:**

In FCC, the **\[110] direction** has highest LD because atoms are closely packed along the face diagonal.

---

# **Planar Density (PD)**

### **Definition (English):**

Planar density is the **number of atoms whose centers lie on a specific crystallographic plane per unit area of that plane.**

$$
PD = \frac{\text{No. of atoms centered on plane}}{\text{Area of plane}}
$$

### **Meaning (Hinglish):**

Planar density batata hai ki **ek plane (jaise (111), (100), (110)) par atoms kitne tight arranged hain**.
Higher PD = plane zyada dense hai = preferred slip plane (dislocation movement yahin hoti hai).

---

### **Example:**

In FCC, the **(111) plane** is most densely packed plane (highest PD).

---

# **Key Difference (Summary Table)**

| Property         | Linear Density (LD)                    | Planar Density (PD)                  |
| ---------------- | -------------------------------------- | ------------------------------------ |
| What it measures | Atoms per unit **length**              | Atoms per unit **area**              |
| Formula          | $LD = \dfrac{\# atoms}{\text{length}}$ | $PD = \dfrac{\# atoms}{\text{area}}$ |
| Direction/Plane  | Along crystallographic **direction**   | On crystallographic **plane**        |
| Example (FCC)    | Highest along **\[110]**               | Highest on **(111)** plane           |

---

👉 Simple samajh lo:

* LD = **line pe atoms kitne close-close hain**.
* PD = **plane pe atoms kitne close-close hain**.

---
