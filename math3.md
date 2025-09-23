Q1. State Sylvester’s Law of Inertia
Solution:
Sylvester's Law of Inertia kehta hai ki:

Ek real symmetric matrix 
A
A ko jab bhi hum congruent transformation se diagonalize karte hain (yani 
P
A
P
T
PAP 
T
  form mein, jahan 
P
P invertible matrix hai), toh diagonal matrix mein:

Positive entries ki sankhya hamesha same rehti hai (ise positive index kehte hain).

Negative entries ki sankhya hamesha same rehti hai (ise negative index kehte hain).

Zero entries ki sankhya hamesha same rehti hai (yeh rank decide karti hai).

Ye teeno numbers (positive, negative, zero) matrix 
A
A ke inertia kehlate hain aur ye 
A
A ke liye invariant hain, chahe hum koi bhi congruent transformation kyun na use karein.

# 2) Dimensions — jaldi aur yaad rakhne waale rules + examples

**(a)** $P_3(t)$ = polynomials of degree $\le 3$.

* Basis: $\{1, t, t^2, t^3\}$.
* **Dimension = 4.**
  **Hinglish:** degree ≤ 3 matlab coefficients ke liye 4 independent numbers — isliye dim = 4.

**(b)** $M_{n\times m}(\mathbb{R})$ = all real $n\times m$ matrices.

* Har matrix mein $n\cdot m$ entries hotey hain; each entry independent coordinate.
* **Dimension = $n m$.**

**(c)** $M_n(\mathbb{R})$ (square $n\times n$) → special case: **dimension = $n^2$.**

**(d)** $\mathbb{R}^n$ (standard n-tuples)

* Basis: standard basis $e_1,\dots,e_n$.
* **Dimension = $n$.**

**Why (very short proof idea):**
Dimension = number of basis vectors. For polynomials degree ≤ k, basis = $\{1,t,\dots,t^k\}$ → $k+1$. For matrices, basis can be matrices with a single 1 in one entry and 0 elsewhere — total $n\cdot m$.

**Quick memory cheat-sheet (one-liners):**

* Polynomial of deg ≤ d → dim = d+1.
* Matrix $n\times m$ → dim = number of entries = $nm$.
* $\mathbb{R}^n$ → dim = n.

---
Chalo bhai — ab **Question 3** ka full step-by-step solution **Hinglish** mein, saare calculations dikhake (taaki yaad ho jaye). Matrix jo tumne likhi thi maine waise hi liya:

$$
A=\begin{pmatrix}2 & a & 7\\[2pt] 0 & 1 & 0\\[2pt] 1 & 1 & 2\end{pmatrix}
$$

(yahaan middle top entry unclear thi — maine use $a$ se denote kiya. Agar woh koi number hai to usko $a$ mein rakh ke bhi sab chalega; agar $a\!=\!1$ ka special case lagega toh main mention kar dunga.)

---

# Step 1 — Characteristic polynomial (aur eigenvalues)

Characteristic polynomial $p(\lambda)=\det(A-\lambda I)$.

Second row me zeros hone ki wajah se expansion easy ho jaata hai:

$$
\det(A-\lambda I)=(1-\lambda)\det\begin{pmatrix}2-\lambda & 7\\[2pt] 1 & 2-\lambda\end{pmatrix}
=(1-\lambda)\big((2-\lambda)^2-7\big).
$$

Ab simplify karte hain:

$$
(2-\lambda)^2-7 = (\lambda^2 -4\lambda +4)-7 = \lambda^2 -4\lambda -3.
$$

Toh

$$
\det(A-\lambda I)=(1-\lambda)(\lambda^2 -4\lambda -3).
$$

Multiply karke polynomial ko standard form me laane par:

$$
p(\lambda)=\lambda^3-5\lambda^2+\lambda+3.
$$

Iske roots (solve karne par) milte hain:

$$
\boxed{\lambda_1 = 1,\qquad \lambda_{2,3} = 2\pm\sqrt{7}.}
$$

(Notice: eigenvalues **$a$** par depend nahi karte.)

---

# Step 2 — Eigenvectors

Hum har eigenvalue ke liye $(A-\lambda I)v=0$ solve karenge.

### (i) For $\lambda=1$

Compute $A-I$:

$$
A-I=\begin{pmatrix}1 & a & 7\\[2pt] 0 & 0 & 0\\[2pt] 1 & 1 & 1\end{pmatrix}.
$$

System $(A-I)v=0$ se milte hain equations (let $v=(v_1,v_2,v_3)^T$):

1. $v_1 + a v_2 + 7 v_3 = 0$
2. (second row) gives $0=0$ (no info)
3. $v_1 + v_2 + v_3 = 0$

Subtracting eqn3 from eqn1: $(a-1)v_2 + 6 v_3 = 0$.
Agar $a\neq 1$, choose free param $v_3=1$ then

$$
v_2 = -\frac{6}{a-1},\qquad v_1 = -v_2 - v_3 = \frac{7-a}{a-1}.
$$

Multiply by $(a-1)$ (scale) to clear denominators: ek convenient eigenvector

$$
\boxed{v^{(1)} = (7-a,\; -6,\; a-1)^T.}
$$

(agar $a=1$ ho to equation becomes $6v_3=0\Rightarrow v_3=0$ and then $v_1+v_2=0$ — that gives eigenvectors of form $(1,-1,0)^T$.)

### (ii) For $\lambda=2\pm\sqrt7$

Second row of $A-\lambda I$ is $(0,1-\lambda,0)$. Since $\lambda\neq1$ for these two roots, we get $v_2=0$.

Phir third-row (or first) se:

$$
v_1 + (1-\lambda)v_3 = 0 \quad\Rightarrow\quad v_1 = - (1-\lambda) v_3 = - (1-\lambda) v_3.
$$

But $1-\lambda = 1-(2\pm\sqrt7) = -1\mp\sqrt7$, and simplifying gives nicer choice if we set $v_3=1$:

For $\lambda = 2-\sqrt7$:

$$
v = (-\sqrt7,\,0,\,1)^T.
$$

For $\lambda = 2+\sqrt7$:

$$
v = (\sqrt7,\,0,\,1)^T.
$$

So eigenvectors:

$$
\boxed{v^{(2)} = (-\sqrt7,\,0,\,1)^T,\quad v^{(3)}=(\sqrt7,\,0,\,1)^T.}
$$

---

# Step 3 — (Optional) Normalize / check linear independence

Tin eigenvalues distinct hain → corresponding eigenvectors automatically linearly independent. Unko normalize karna ho to divide by their lengths — par exam me usually direction vectors hi chahiye.

---

# Step 4 — Verify Cayley–Hamilton theorem for this $A$

Characteristic polynomial tha $p(\lambda)=\lambda^3-5\lambda^2+\lambda+3$. Cayley–Hamilton kahta hai $p(A)=A^3-5A^2 + A + 3I = 0$ (zero matrix).

Ab main $A^2$ aur $A^3$ explicitly compute karke dikhaata hoon (ye symbolic in terms of $a$):

**Compute $A^2$:**

$$
A^2=\begin{pmatrix}
11 & 3a+7 & 28\\[2pt]
0 & 1 & 0\\[2pt]
4 & a+3 & 11
\end{pmatrix}.
$$

**Compute $A^3 = A\cdot A^2$:**

$$
A^3=\begin{pmatrix}
50 & 14a+35 & 133\\[2pt]
0 & 1 & 0\\[2pt]
19 & 5a+14 & 50
\end{pmatrix}.
$$

Ab $p(A)=A^3-5A^2+A+3I$. Compute entry-wise (main ones shown):

* $(1,1)$: $50 -5\cdot11 + 2 +3 = 50-55+5 =0.$

* $(1,2)$: $(14a+35) -5(3a+7) + a + 0 = 14a+35 -15a -35 + a =0.$

* $(1,3)$: $133 -5\cdot28 + 7 +0 =133 -140 +7 =0.$

* Middle row always gives $0$ (check: $0 -5\cdot0 + 0 + 3\cdot I_{22}$ etc → sums to zero as we compute; explicitly $(2,2):1-5\cdot1 +1 +3=0$).

* $(3,1)$: $19 -5\cdot4 +1 =19 -20 +1 =0.$

* $(3,2)$: $(5a+14) -5(a+3) +1 =5a+14 -5a -15 +1 =0.$

* $(3,3)$: $50 -5\cdot11 +2 +3 =50-55+5=0.$

Sab entries zero — matlab

$$
\boxed{A^3-5A^2 + A + 3I = 0,}
$$

jo Cayley–Hamilton ko confirm karta hai. Yeh calculation **general $a$** ke liye bhi true (humne symbolic $a$ ke saath calculate kiya).

---

# Short summary / memory tips (Hinglish)

* Characteristic polynomial se eigenvalues nikaalte ho; agar ek row/column me zeros ho to determinant expand karna easy ho jaata hai.
* Distinct eigenvalues → eigenvectors independent.
* Cayley–Hamilton: matrix apni characteristic polynomial satisfy karta hai; verify karne ke liye $A^2, A^3$ nikaal ke polynomial substitute karo and simplify — agar sab zeros aaye toh theorem satisfied.

Agar chaahe to main ab is example ka numerical case $a=3$ leke eigenvectors ko simplify karke orthonormal bana ke dikhau (ya phir step-by-step manual compute of $A^2,A^3$ line-by-line). Batao kya chahiye — warna main agla question 4 pe chalu kar doon?
Thik hai bhai 👌 ab **Question 4** ko step by step solve aur explain karte hain **English + Hinglish** dono mein.

---

## Question 4

### 🔹 Given:

* Side of cube = **a**
* Body diagonal = $\sqrt{3}a$
* Relation between **radius (r)** and **body diagonal** of cube →
  $\text{Body diagonal} = 4r$

We need to **find packing efficiency**.

---

### 🔹 Step 1: Radius in terms of ‘a’

$$
\sqrt{3}a = 4r
$$

$$
r = \frac{\sqrt{3}}{4}a
$$

👉 Matlab cube ke andar jo sphere (atom) fit ho raha hai uska radius itna hoga.

---

### 🔹 Step 2: Volume of atoms in cube

Cube ke andar **4 atoms** hote hain (kyunki FCC ka case hai).

* Volume of 1 atom = $\frac{4}{3}\pi r^3$
* Total volume of atoms in cube =

$$
4 \times \frac{4}{3}\pi r^3 = \frac{16}{3}\pi r^3
$$

---

### 🔹 Step 3: Volume of cube

$$
V_{\text{cube}} = a^3
$$

---

### 🔹 Step 4: Packing efficiency

Formula:

$$
\text{Packing efficiency} = \frac{\text{Volume of atoms in cube}}{\text{Volume of cube}} \times 100
$$

Substitute values:

$$
= \frac{\frac{16}{3}\pi r^3}{a^3} \times 100
$$

Ab $r = \frac{\sqrt{3}}{4}a$ put karte hain:

$$
= \frac{16}{3}\pi \left(\frac{\sqrt{3}}{4}a\right)^3 \times \frac{100}{a^3}
$$

---

### 🔹 Step 5: Simplification

$$
= \frac{16}{3}\pi \times \frac{3\sqrt{3}}{64}a^3 \times \frac{100}{a^3}
$$

$$
= \frac{16}{3} \times \frac{3\sqrt{3}}{64} \pi \times 100
$$

$$
= \frac{16 \cdot 3\sqrt{3}}{192} \pi \times 100
$$

$$
= \frac{\sqrt{3}\pi}{4} \times 100
$$

---

### 🔹 Final Answer

$$
\text{Packing Efficiency} = \frac{\sqrt{3}\pi}{4} \times 100 \approx 68.02\%
$$

---

## ✅ Explanation in Hinglish

1. Cube ka diagonal = $\sqrt{3}a$. Isko 4r ke equal kiya kyunki sphere cube ke diagonal ke along touch karta hai.
2. Isse $r = \frac{\sqrt{3}}{4}a$ aaya.
3. Cube me FCC arrangement hota hai → 4 atoms present.
4. Atoms ka total volume = $\frac{16}{3}\pi r^3$.
5. Cube ka volume = $a^3$.
6. Efficiency ka formula lagaya: $\frac{\text{atom volume}}{\text{cube volume}} \times 100$.
7. Simplify karne ke baad \~ **68%** aaya.

👉 Matlab FCC packing efficiency **68% ke aas paas hoti hai**.

---
Thik hai bhai 👌 ab **Question 5** ko step by step solve karke **English + Hinglish** mein explain karte hain.

---

## Question 5

### 🔹 Given:

* Radius of atom = **r**
* Simple cubic lattice (SC)
* Relation between **edge length (a)** and **radius (r)**:

  $$
  a = 2r
  $$

We need: **Packing Efficiency of SC.**

---

### 🔹 Step 1: Number of atoms in SC unit cell

* SC mein sirf **corner atoms** hote hain.
* 1 cube mein **8 corners** hote hain.
* Har corner atom **1/8th** part contribute karta hai ek cube ko.

$$
N = 8 \times \frac{1}{8} = 1 \text{ atom per unit cell}
$$

---

### 🔹 Step 2: Volume of atoms in cube

* Volume of 1 atom =

$$
V_{\text{atom}} = \frac{4}{3}\pi r^3
$$

* Total volume of atoms in cube =

$$
= 1 \times \frac{4}{3}\pi r^3 = \frac{4}{3}\pi r^3
$$

---

### 🔹 Step 3: Volume of cube

$$
a = 2r \quad \Rightarrow \quad V_{\text{cube}} = a^3 = (2r)^3 = 8r^3
$$

---

### 🔹 Step 4: Packing efficiency

Formula:

$$
\text{Packing efficiency} = \frac{\text{Volume of atoms in unit cell}}{\text{Volume of unit cell}} \times 100
$$

$$
= \frac{\frac{4}{3}\pi r^3}{8r^3} \times 100
$$

---

### 🔹 Step 5: Simplify

$$
= \frac{\pi}{6} \times 100
$$

$$
\approx 52.36\%
$$

---

## ✅ Final Answer:

$$
\text{Packing Efficiency of Simple Cubic (SC)} = 52.36\%
$$

---

## ✅ Hinglish Explanation

1. SC (simple cubic) mein sirf corner atoms hote hain.

   * 8 corners × (1/8 contribution) = 1 atom/unit cell.
2. Total atom ka volume = $\frac{4}{3}\pi r^3$.
3. Cube ka side $a = 2r$.

   * Cube volume = $(2r)^3 = 8r^3$.
4. Packing efficiency = $\frac{\text{atoms ka volume}}{\text{cube ka volume}} \times 100$.
5. Solve karke $\pi/6 \times 100 \approx 52.36\%$.

👉 Matlab SC packing efficiency sabse kam hoti hai (only \~52%).

---

Bhai ab **6th question** karaun kya?
Bhai ab **Question 7** ko step by step karte hain 👌 aur dono language me (English + Hinglish) explain karte hain.  

---

## Question 7  

### 🔹 Given:  
- Structure = **Face Centered Cubic (FCC)**  
- Atomic radius = \( r \)  
- Need to find:  
  1. Relation between \( r \) and \( a \) (edge length)  
  2. Packing efficiency  

---

### 🔹 Step 1: Number of atoms in FCC unit cell  
- 8 corners → \( 8 \times \frac{1}{8} = 1 \) atom  
- 6 face centers → \( 6 \times \frac{1}{2} = 3 \) atoms  
\[
N = 1 + 3 = 4 \text{ atoms per unit cell}
\]

---

### 🔹 Step 2: Relation between \( r \) and \( a \)  
- In FCC, atoms touch along **face diagonal**.  
- Face diagonal length = \( \sqrt{2}a \)  
- Along face diagonal: 4 radii = \( 4r \)  
\[
\sqrt{2}a = 4r
\]  

\[
a = \frac{4r}{\sqrt{2}} = 2\sqrt{2}r
\]

---

### 🔹 Step 3: Volume of atoms in unit cell  
\[
V_{\text{atoms}} = N \times \frac{4}{3}\pi r^3
= 4 \times \frac{4}{3}\pi r^3
= \frac{16}{3}\pi r^3
\]

---

### 🔹 Step 4: Volume of cube  
\[
V_{\text{cube}} = a^3 = (2\sqrt{2}r)^3
= 16\sqrt{2}r^3
\]

---

### 🔹 Step 5: Packing Efficiency  
\[
\text{Packing efficiency} = \frac{V_{\text{atoms}}}{V_{\text{cube}}} \times 100
\]

\[
= \frac{\frac{16}{3}\pi r^3}{16\sqrt{2}r^3} \times 100
\]

---

### 🔹 Step 6: Simplify  
Cancel \( 16r^3 \):  

\[
= \frac{\pi}{3\sqrt{2}} \times 100
\]

\[
\approx 74.05\%
\]

---

## ✅ Final Answer:  
- Relation:  
  \[
  a = 2\sqrt{2}r
  \]  
- Packing Efficiency:  
  \[
  74.05\%
  \]  

---

## ✅ Hinglish Explanation  
1. FCC mein total **4 atoms/unit cell** hote hain (1 from corners + 3 from face centers).  
2. Atoms **face diagonal** ke along touch karte hain → relation \( \sqrt{2}a = 4r \) → \( a = 2\sqrt{2}r \).  
3. Atom volume = \( \frac{16}{3}\pi r^3 \).  
4. Cube volume = \( 16\sqrt{2}r^3 \).  
5. Packing efficiency = \( \frac{\pi}{3\sqrt{2}} \times 100 \approx 74.05\% \).  

👉 Matlab FCC (aur HCP bhi) sabse efficient packing hota hai ≈ **74%**.  

---

Bhai ab mai chahu toh **1 se 7 ka ek combined summary chart** bana dun jisme SC, BCC, FCC sabka relation + packing efficiency ek jagah ho?
