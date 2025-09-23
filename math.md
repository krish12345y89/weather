### **Q1. State Sylvester’s Law of Inertia**

**Solution:**
Sylvester's Law of Inertia kehta hai ki:
> Ek real symmetric matrix \( A \) ko jab bhi hum congruent transformation se diagonalize karte hain (yani \( PAP^T \) form mein, jahan \( P \) invertible matrix hai), toh diagonal matrix mein:
> - **Positive** entries ki sankhya hamesha same rehti hai (ise **positive index** kehte hain).
> - **Negative** entries ki sankhya hamesha same rehti hai (ise **negative index** kehte hain).
> - **Zero** entries ki sankhya hamesha same rehti hai (yeh rank decide karti hai).

Ye teeno numbers (positive, negative, zero) matrix \( A \) ke **inertia** kehlate hain aur ye \( A \) ke liye invariant hain, chahe hum koi bhi congruent transformation kyun na use karein.

---

### **Q2. Dimensions of Vector Spaces**

**Solution:**
**(i) \( P_3(t) \)**
- Yeh polynomials ka space hai jinka degree ≤ 3 hai.
- Standard basis: \( \{1, t, t^2, t^3\} \)
- Basis mein 4 elements hain.
- **Dimension = 4**

**(ii) \( M_{n \times m}(\mathbb{R}) \)**
- Yeh sab \( n \times m \) real matrices ka space hai.
- Standard basis: Sab matrices jisme ek entry 1 hai aur baaki sab 0.
- Aise total \( n \times m \) matrices hain.
- **Dimension = \( n \times m \)**

**(iii) \( M_{n \times n}(\mathbb{R}) \)**
- Yeh square matrices ka space hai.
- **Dimension = \( n^2 \)**

**(iv) \( \mathbb{R}^n \)**
- Yeh n-tuples of real numbers ka space hai.
- Standard basis: \( \{e_1, e_2, \dots, e_n\} \) jahan \( e_i \) mein i-th entry 1 hai.
- **Dimension = \( n \)**

---

### **Q3. Eigenvalues, Eigenvectors aur Cayley-Hamilton Verification**

**Given:** \( A = \begin{pmatrix}2 & 1 & 1 \\ 0 & 1 & 0 \\ 1 & 1 & 2\end{pmatrix} \)

#### **Step 1: Characteristic Equation**
\[
\det(A - \lambda I) = \det\begin{pmatrix}2-\lambda & 1 & 1 \\ 0 & 1-\lambda & 0 \\ 1 & 1 & 2-\lambda\end{pmatrix}
\]
Expand karte hain (second row se easy hai):
\[
= (1-\lambda) \cdot \det\begin{pmatrix}2-\lambda & 1 \\ 1 & 2-\lambda\end{pmatrix}
\]
\[
= (1-\lambda) \left[ (2-\lambda)(2-\lambda) - 1 \cdot 1 \right]
\]
\[
= (1-\lambda) \left[ \lambda^2 - 4\lambda + 4 - 1 \right] = (1-\lambda)(\lambda^2 - 4\lambda + 3)
\]
\[
= (1-\lambda)(\lambda - 1)(\lambda - 3) = -(\lambda - 1)^2 (\lambda - 3)
\]
Toh characteristic equation: \( (\lambda - 1)^2 (\lambda - 3) = 0 \)

**Eigenvalues:** \( \lambda = 1 \) (multiplicity 2), \( \lambda = 3 \) (multiplicity 1)

#### **Step 2: Eigenvectors nikalna**

**For \( \lambda = 1 \):**
Solve \( (A - I)X = 0 \)
\[
A - I = \begin{pmatrix}1 & 1 & 1 \\ 0 & 0 & 0 \\ 1 & 1 & 1\end{pmatrix}
\]
Row reduce: Basically ek hi equation bachegi: \( x + y + z = 0 \)
Free variables: \( y = s, z = t \), toh \( x = -s - t \)
\[
X = s\begin{pmatrix}-1 \\ 1 \\ 0\end{pmatrix} + t\begin{pmatrix}-1 \\ 0 \\ 1\end{pmatrix}
\]
Eigenvectors: \( v_1 = (-1,1,0)^T \), \( v_2 = (-1,0,1)^T \)

**For \( \lambda = 3 \):**
Solve \( (A - 3I)X = 0 \)
\[
A - 3I = \begin{pmatrix}-1 & 1 & 1 \\ 0 & -2 & 0 \\ 1 & 1 & -1\end{pmatrix}
\]
Row reduce:
- Second row: \( -2y = 0 \Rightarrow y = 0 \)
- First row: \( -x + z = 0 \Rightarrow z = x \)
- Third row: \( x + 0 - x = 0 \) (automatically satisfied)

Let \( x = t \), toh \( z = t \)
\[
X = t\begin{pmatrix}1 \\ 0 \\ 1\end{pmatrix}
\]
Eigenvector: \( v_3 = (1,0,1)^T \)

#### **Step 3: Cayley-Hamilton Theorem Verify karna**
Theorem kehta hai: Matrix apni characteristic equation ko satisfy karegi.
Characteristic equation: \( (\lambda - 1)^2 (\lambda - 3) = 0 \Rightarrow \lambda^3 - 5\lambda^2 + 7\lambda - 3 = 0 \)

Iska matlab: \( A^3 - 5A^2 + 7A - 3I = 0 \) (zero matrix)

**Compute \( A^2 \):**
\[
A^2 = \begin{pmatrix}2&1&1\\0&1&0\\1&1&2\end{pmatrix} \begin{pmatrix}2&1&1\\0&1&0\\1&1&2\end{pmatrix} = \begin{pmatrix}5&4&4\\0&1&0\\4&4&5\end{pmatrix}
\]

**Compute \( A^3 = A \cdot A^2 \):**
\[
A^3 = \begin{pmatrix}2&1&1\\0&1&0\\1&1&2\end{pmatrix} \begin{pmatrix}5&4&4\\0&1&0\\4&4&5\end{pmatrix} = \begin{pmatrix}14&13&13\\0&1&0\\13&13&14\end{pmatrix}
\]

**Ab check karo:**
\[
A^3 - 5A^2 + 7A - 3I
\]
\[
= \begin{pmatrix}14&13&13\\0&1&0\\13&13&14\end{pmatrix} - 5\begin{pmatrix}5&4&4\\0&1&0\\4&4&5\end{pmatrix} + 7\begin{pmatrix}2&1&1\\0&1&0\\1&1&2\end{pmatrix} - 3\begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}
\]
Term-wise calculate karo:

- First entry: \( 14 - 25 + 14 - 3 = 0 \)
- Second entry: \( 13 - 20 + 7 - 0 = 0 \)
- Third entry: \( 13 - 20 + 7 - 0 = 0 \)
- Second row: \( 0 - 0 + 0 - 0 = 0 \) etc.

Sab entries zero aayengi. Toh **verified**.

---

### **Q4. Cayley-Hamilton Theorem Statement**

**Solution:**
Cayley-Hamilton Theorem kehta hai ki:
> Har square matrix apni hi characteristic equation ko satisfy karti hai.
> Yani, agar characteristic equation hai:
> \[ \det(A - \lambda I) = \lambda^n + c_{n-1}\lambda^{n-1} + \dots + c_1\lambda + c_0 = 0 \]
> Toh matrix ke liye:
> \[ A^n + c_{n-1}A^{n-1} + \dots + c_1 A + c_0 I = 0 \]
> (Yahan \( \lambda \) ki jagah \( A \) use karo, aur constant term ko \( c_0 I \) form mein.)

---

### **Q5. Definitions**

**(i) Similar Matrices:**
Do matrices \( A \) aur \( B \) similar kehlati hain agar ek invertible matrix \( P \) exist karti hai such that:
\[
B = P^{-1} A P
\]
Similar matrices ka characteristic polynomial same hota hai, eigenvalues same hoti hain, but eigenvectors alag hote hain.

**(ii) Orthogonal Matrix:**
Ek square matrix \( Q \) orthogonal hoti hai agar:
\[
Q^T Q = Q Q^T = I
\]
Yani, \( Q^{-1} = Q^T \). Orthogonal matrix ke columns (aur rows) orthonormal hote hain (unit length aur mutually perpendicular).

**(iii) Unitary Matrix:**
Ek square matrix \( U \) unitary hoti hai agar (complex numbers ke liye):
\[
U^* U = U U^* = I
\]
Yani, \( U^{-1} = U^* \) (where \( U^* \) denotes conjugate transpose). Agar matrix real hai, toh unitary matrix orthogonal matrix hi hoti hai.

---

### **Q6. Vector Space aur Subspace Definition**

**Vector Space:**
Ek set \( V \) (elements ko vectors kehte hain) jisme do operations define hain:
1. **Vector addition:** \( u + v \in V \)
2. **Scalar multiplication:** \( \alpha u \in V \) (scalar field se, typically real numbers)

Ye operations 10 axioms ko satisfy karte hain (jaise commutativity, associativity, zero vector, additive inverse, etc.).

**Subspace:**
Ek vector space \( V \) ka subset \( W \) subspace kehlata hai agar:
1. \( W \) non-empty hai (usually zero vector \( \mathbf{0} \in W \))
2. \( W \) addition aur scalar multiplication ke under closed hai:
   - \( u, v \in W \Rightarrow u + v \in W \)
   - \( u \in W, \alpha \in \mathbb{R} \Rightarrow \alpha u \in W \)

Subspace khud ek vector space hota hai.

---

### **Q7. Matrix of Linear Transformation**

**Given:**
- \( T: \mathbb{R}^2 \to \mathbb{R}^3 \) defined by \( T(x,y) = (x-y, x, x+2y) \)
- Basis of \( \mathbb{R}^2 \): \( B_2 = \{(1,2), (2,3)\} \)
- Basis of \( \mathbb{R}^3 \): \( B_3 = \{(1,1,0), (0,1,1), (1,2,3)\} \)

**Step 1: Basis vectors par transformation apply karo**

- \( T(1,2) = (1-2, 1, 1+4) = (-1, 1, 5) \)
- \( T(2,3) = (2-3, 2, 2+6) = (-1, 2, 8) \)

**Step 2: In images ko target basis \( B_3 \) ke terms mein express karo**

Yani, solve karo:
\[
(-1, 1, 5) = a(1,1,0) + b(0,1,1) + c(1,2,3)
\]
\[
(-1, 2, 8) = p(1,1,0) + q(0,1,1) + r(1,2,3)
\]

**Pehla system:**
- From coordinates: 
  \( a + 0b + c = -1 \)
  \( a + b + 2c = 1 \)
  \( 0a + b + 3c = 5 \)

Solve: Third eq: \( b + 3c = 5 \Rightarrow b = 5 - 3c \)
First eq: \( a + c = -1 \Rightarrow a = -1 - c \)
Second eq: \( (-1 - c) + (5 - 3c) + 2c = 1 \)
\( 4 - 2c = 1 \Rightarrow -2c = -3 \Rightarrow c = 1.5 \)
Toh \( a = -1 - 1.5 = -2.5 \), \( b = 5 - 4.5 = 0.5 \)

So \( T(1,2) = -2.5(1,1,0) + 0.5(0,1,1) + 1.5(1,2,3) \)

**Dusra system:**
- Equations:
  \( p + r = -1 \)
  \( p + q + 2r = 2 \)
  \( q + 3r = 8 \)

Third eq: \( q = 8 - 3r \)
First: \( p = -1 - r \)
Second: \( (-1 - r) + (8 - 3r) + 2r = 2 \)
\( 7 - 2r = 2 \Rightarrow -2r = -5 \Rightarrow r = 2.5 \)
Toh \( p = -1 - 2.5 = -3.5 \), \( q = 8 - 7.5 = 0.5 \)

So \( T(2,3) = -3.5(1,1,0) + 0.5(0,1,1) + 2.5(1,2,3) \)

**Step 3: Matrix banayo**
Matrix \( [T]_{B_2}^{B_3} \) ke columns yeh coefficients honge:

Pehla column: \( \begin{pmatrix}-2.5 \\ 0.5 \\ 1.5\end{pmatrix} \)
Dusra column: \( \begin{pmatrix}-3.5 \\ 0.5 \\ 2.5\end{pmatrix} \)

Toh final matrix:
\[
[T]_{B_2}^{B_3} = \begin{pmatrix} -2.5 & -3.5 \\ 0.5 & 0.5 \\ 1.5 & 2.5 \end{pmatrix}
\]

---
