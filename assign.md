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
