Nice — let’s go **very deep** and explain every line, every formula, and every unit — in **English** and then the same explanation in **Hinglish (mix of Hindi + English)** so you can study both ways. I’ll also show the arithmetic **digit-by-digit** so there’s no confusion.

---

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

Agar chaho toh main ye steps neatly typeset kar ke ek PDF ya image bana ke de dunga for submission — batao prefer karoge? (Otherwise, you can copy these steps into your answer sheet.)
