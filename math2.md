**1) State Sylvester’s law (of inertia)**
Simple statement (Hinglish):

* Agar $A$ ek real symmetric matrix hai, to koi bhi invertible matrix $P$ ke liye $P^T A P$ ko diagonal form mein convert kar sakte hain jisme diagonal entries sirf $+1, -1, 0$ type ke “signs” honge.
* Sylvester’s law kehta hai ki **positive count**, **negative count**, aur **zero count** (inna ko collectively *inertia* bolte hain) invariant hote hain under congruence $P^T A P$. Matlab kisi bhi congruent transformation se signs ki exact number nahi badalti.
  Why useful (hinglish): yeh batata hai ki real symmetric matrix ka “signature” (kitne +, kitne -) fixed hota hai — basis change se nahi badalta.

---

**2) Dimensions of common vector spaces**
(Explain why briefly)

* $P_3(t)$ = polynomials of degree $\le 3$.
  Basis: $\{1, t, t^2, t^3\}$ → **dimension = 4**.
  (Hinglish: degree ≤3 hone se coefficients 4 hote hain — isliye dim 4.)

* $M_{n\times m}(\mathbb{R})$ = all real $n\times m$ matrices.
  You can choose each of the $n\cdot m$ entries freely → **dimension = $n m$**.

* $M_{n}(\mathbb{R})$ (square) is just special case $m=n$ → **dimension = $n^2$**.

* $\mathbb{R}^n$ (or $F^n$) → standard basis $e_1,\dots,e_n$ → **dimension = $n$**.

* General rule (hinglish): dimension = number of independent coordinates / basis elements.

---

**3) Find eigenvalues & eigenvectors of the matrix**
Matrix shown in paper (I denote middle-top entry by $a$ because handwriting was unclear):

$$
A=\begin{pmatrix}2 & a & 7\\[2pt] 0 & 1 & 0\\[2pt] 1 & 1 & 2\end{pmatrix}
$$

**Step 1 — Characteristic polynomial** (expand using 2nd row since it has zeros):

$$
\det(A-\lambda I)=(1-\lambda)\det\begin{pmatrix}2-\lambda & 7\\[2pt]1 & 2-\lambda\end{pmatrix}
=(1-\lambda)\big((2-\lambda)^2-7\big).
$$

Simplify: $(1-\lambda)\big(\lambda^2-4\lambda-3\big)$.
Roots (set =0) give eigenvalues:

$$
\boxed{\lambda_1=1,\qquad \lambda_{2,3}=2\pm\sqrt{7}.}
$$

(Notice: eigenvalues **do not depend** on $a$.)

**Step 2 — Eigenvectors**

* For $\lambda=1$: solve $(A-I)v=0$. Equations reduce to

  $$
  v_1+ a v_2 + 7 v_3 =0,\qquad v_1+v_2+v_3=0.
  $$

  From these (eliminate $v_1$) you get

  $$
  (a-1)v_2 + 6 v_3 = 0 \;\Rightarrow\; v_2 = -\frac{6}{a-1}v_3.
  $$

  Choose $v_3=1$ (free parameter), then

  $$
  v_1=\frac{7-a}{\,a-1\,},\; v_2=-\frac{6}{a-1},\; v_3=1.
  $$

  You can scale by $(a-1)$ to remove denominators: an equivalent eigenvector is

  $$
  \boxed{v^{(1)}=(7-a,\;-6,\;a-1)^T}\quad(\text{or any nonzero scalar multiple}).
  $$

  (If the handwritten middle entry is e.g. $a=3$, then $v^{(1)}=(4,-6,2)$ which scales to $(2,-3,1)$.)

* For $\lambda=2\pm\sqrt7$: from second row $(1-\lambda)v_2=0$ we get $v_2=0$. Then third-row gives
  $v_1+(2-\lambda)v_3=0\Rightarrow v_1=-(2-\lambda)v_3$.
  Set $v_3=1$ → $v_1=-(2-\lambda)$. So

  $$
  \boxed{ \text{for }\lambda=2-\sqrt7:\; v=\big(-\sqrt7,\,0,\,1\big)^T,\qquad
                \text{for }\lambda=2+\sqrt7:\; v=\big(\sqrt7,\,0,\,1\big)^T.}
  $$

**Cayley–Hamilton verification (example with a concrete $a$)**
Take $a=3$ (clean numbers). Then

$$
A=\begin{pmatrix}2&3&7\\0&1&0\\1&1&2\end{pmatrix}.
$$

Characteristic polynomial expanded gives $p(\lambda)=\lambda^3-5\lambda^2+\lambda+3$. Cayley–Hamilton says $p(A)=A^3-5A^2+A+3I=0$. If you compute $A^2,A^3$ and substitute (I checked numerically), you get the zero matrix — so CH theorem holds. (General algebraic proof: CH theorem is true for every square matrix; here you can verify by direct substitution.)

---

**4) State Cayley–Hamilton theorem**
(Hinglish concise)

* *Cayley–Hamilton theorem* kehta hai: **Har square matrix apni characteristic polynomial ko satisfy karta hai**.
* Formally: agar $p(\lambda)=\det(\lambda I - A)$ to $p(A)=0$ (zero matrix).
* Usefulness: matrix polynomials ko reduce karne mein, powers of A ko lower-degree polynomials se replace karne mein bahut helpful.

---

**5) Define: similar matrix, orthogonal matrix, unitary matrix**
(Hinglish + short properties)

* **Similar matrices**: $B$ is similar to $A$ if $\exists$ invertible $P$ such that $B=P^{-1}AP$. Similar matrices represent the same linear map in different bases → they have same characteristic polynomial, same eigenvalues (multiplicities), same trace, determinant.

* **Orthogonal matrix** (real): $Q$ orthogonal if $Q^T Q = I$ (equivalently $Q^{-1}=Q^T$). Columns form an orthonormal basis (real). Preserves inner product and lengths.

* **Unitary matrix** (complex analogue): $U$ unitary if $U^* U = I$ where $U^*$ is conjugate transpose. Preserves complex inner product and lengths.

---

**6) Define Vector space & Subspace**
(Hinglish)

* **Vector space** over a field $F$: set $V$ with two operations (vector addition and scalar multiplication) that satisfy 8 axioms (associativity, commutativity of addition, identity $0$, additive inverses, distributivity of scalars over vector addition and over field addition, compatibility of scalar multiplication, and identity scalar $1\cdot v = v$). Example: $\mathbb{R}^n$, polynomial spaces $P_n$, matrix spaces $M_{n\times m}$.

* **Subspace**: subset $W\subset V$ which itself is a vector space under same operations. Test: $W$ non-empty, closed under addition and closed under scalar multiplication.

---

**7) Linear map $T:\mathbb{R}^2\to\mathbb{R}^3$ — find matrix w\.r.t. given bases**
Given:

$$
T(x,y)=(x-y,\; x,\; x+2y).
$$

Domain ordered basis $B=\{e_1,e_2\}$ with $e_1=(1,2),\; e_2=(2,3)$.
Codomain ordered basis $B'=\{u_1,u_2,u_3\}$ with $u_1=(1,1,0),\; u_2=(0,1,1),\; u_3=(1,2,3)$.

**Step A — Compute images of domain basis**

* $T(e_1)=T(1,2)=(1-2,\;1,\;1+4)=(-1,\,1,\,5).$
* $T(e_2)=T(2,3)=(2-3,\;2,\;2+6)=(-1,\,2,\,8).$

**Step B — Express each $T(e_i)$ in the codomain basis $B'$**
We want scalars $c_1,c_2,c_3$ such that

$$
c_1(1,1,0)+c_2(0,1,1)+c_3(1,2,3) = \text{(target)}.
$$

Solve for $T(e_1)=(-1,1,5)$:

Equations (coordinate-wise):

$$
\begin{cases}
c_1 + c_3 = -1 \\
c_1 + c_2 + 2c_3 = 1 \\
c_2 + 3 c_3 = 5
\end{cases}
$$

Solve: from first $c_1=-1-c_3$. Substitute in second→ $ -1-c_3 + c_2 + 2c_3 =1 \Rightarrow c_2 + c_3 =2$. Third→ $c_2 + 3c_3 =5$. Subtract these two: $2c_3=3\Rightarrow c_3=\tfrac32$. Then $c_2=\tfrac12$, $c_1=-\tfrac52$. So coordinates of $T(e_1)$ in $B'$ are $\big(-\tfrac52,\;\tfrac12,\;\tfrac32\big)^T$.

Similarly for $T(e_2)=(-1,2,8)$:

$$
\begin{cases}
c_1 + c_3 = -1\\
c_1 + c_2 + 2c_3 = 2\\
c_2 + 3c_3 = 8
\end{cases}
$$

Solve: from first $c_1=-1-c_3$. Substitute → $ -1-c_3 + c_2 +2c_3 =2 \Rightarrow c_2 + c_3 =3$. Third → $c_2 + 3c_3 =8$. Subtract → $2c_3=5\Rightarrow c_3=\tfrac52$. Then $c_2=\tfrac12$, $c_1=-\tfrac72$. So coordinates: $\big(-\tfrac72,\;\tfrac12,\;\tfrac52\big)^T$.

**Step C — Final matrix of $T$ w\.r.t. $B$ (domain) and $B'$ (codomain)**
Matrix is $3\times2$ whose columns are the coordinate vectors found above:

$$
\boxed{[T]_{B'\leftarrow B}=
\begin{pmatrix}
-\tfrac52 & -\tfrac72\\[4pt]
\tfrac12 & \tfrac12\\[4pt]
\tfrac32 & \tfrac52
\end{pmatrix}.}
$$

(You can keep fractions or multiply whole matrix by 2 if you prefer integers — but standard is above.)

---

Agar chahiye to main inmein se kisi bhi part ka aur detailed numeric walkthrough (jaise Cayley–Hamilton ka full A^2, A^3 compute kar ke) step-by-step likh doon. Batao konsa part aur deepen karna hai — warna ye answers exam ke liye ready aur neat hain. 👍
