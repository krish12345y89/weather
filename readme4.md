Of course, bhai! Ye rahe 20 numerical problems on Mohr's Circle of Stress. Har ek ko step-by-step, easy English aur Hindi dono mein samjhaya hai. Main formulas aur concepts bhi explain karunga.

---

### **Mohr's Circle Basics Recap (Quick Review)**

*   **What it is:** A graphical method to find stresses on any inclined plane.
*   **Key Formulas:**
    *   **Center of Circle (C)** on the σ-axis: `C = (σₓ + σᵧ) / 2`
    *   **Radius of Circle (R):** `R = √[ ((σₓ - σᵧ)/2)² + τₓᵧ² ]`
    *   **Principal Stresses (σ₁, σ₂):** `σ₁ = C + R`, `σ₂ = C - R`
    *   **Maximum Shear Stress (τ_max):** `τ_max = R`
    *   **Angle to Principal Planes (θ_p):** `tan(2θ_p) = (2τₓᵧ) / (σₓ - σᵧ)`

---

### **Numerical Problems on Mohr's Circle**

**Problem 1: Uniaxial Tension (Basic)**
**Given:** At a point, σₓ = 100 MPa (T), σᵧ = 0, τₓᵧ = 0.
**Find:** σ₁, σ₂, τ_max using Mohr's Circle.

**Solution:**
**Step 1:** Find Center (C).
`C = (σₓ + σᵧ)/2 = (100 + 0)/2 = 50 MPa`

**Step 2:** Find Radius (R).
`R = √[ ((100 - 0)/2)² + (0)² ] = √(50²) = 50 MPa`

**Step 3:** Find Principal Stresses.
`σ₁ = C + R = 50 + 50 = 100 MPa`
`σ₂ = C - R = 50 - 50 = 0 MPa`

**Step 4:** Find Max Shear Stress.
`τ_max = R = 50 MPa`

**Conclusion:** For simple tension, σ₁ is the applied stress, and max shear is half of it.

---

**Problem 2: Uniaxial Compression**
**Given:** σₓ = -80 MPa (C), σᵧ = 0, τₓᵧ = 0.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (-80 + 0)/2 = -40 MPa`
`R = √[ ((-80 - 0)/2)² + 0² ] = √(40²) = 40 MPa`
`σ₁ = -40 + 40 = 0 MPa`
`σ₂ = -40 - 40 = -80 MPa`
`τ_max = 40 MPa`

**Conclusion:** In compression, the minor principal stress (σ₂) is the applied stress.

---

**Problem 3: Pure Shear**
**Given:** σₓ = 0, σᵧ = 0, τₓᵧ = 40 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (0 + 0)/2 = 0 MPa`
`R = √[ ((0 - 0)/2)² + (40)² ] = √(0 + 1600) = 40 MPa`
`σ₁ = 0 + 40 = 40 MPa` (Tension)
`σ₂ = 0 - 40 = -40 MPa` (Compression)
`τ_max = 40 MPa`

**Conclusion:** Pure shear produces equal and opposite principal stresses.

---

**Problem 4: Biaxial Stress (No Shear)**
**Given:** σₓ = 120 MPa (T), σᵧ = 40 MPa (T), τₓᵧ = 0.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (120 + 40)/2 = 80 MPa`
`R = √[ ((120 - 40)/2)² + 0² ] = √(40²) = 40 MPa`
`σ₁ = 80 + 40 = 120 MPa`
`σ₂ = 80 - 40 = 40 MPa`
`τ_max = 40 MPa`

---

**Problem 5: Biaxial Stress (One Tension, One Compression)**
**Given:** σₓ = 60 MPa (T), σᵧ = -20 MPa (C), τₓᵧ = 0.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (60 + (-20))/2 = 20 MPa`
`R = √[ ((60 - (-20))/2)² + 0² ] = √(40²) = 40 MPa`
`σ₁ = 20 + 40 = 60 MPa`
`σ₂ = 20 - 40 = -20 MPa`
`τ_max = 40 MPa`

---

**Problem 6: General Case (With Shear) - 1**
**Given:** σₓ = 80 MPa, σᵧ = 20 MPa, τₓᵧ = 30 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (80 + 20)/2 = 50 MPa`
`R = √[ ((80 - 20)/2)² + (30)² ] = √(30² + 30²) = √1800 = 42.43 MPa`
`σ₁ = 50 + 42.43 = 92.43 MPa`
`σ₂ = 50 - 42.43 = 7.57 MPa`
`τ_max = 42.43 MPa`

---

**Problem 7: General Case (With Shear) - 2**
**Given:** σₓ = 50 MPa, σᵧ = -10 MPa, τₓᵧ = 40 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (50 + (-10))/2 = 20 MPa`
`R = √[ ((50 - (-10))/2)² + (40)² ] = √(30² + 40²) = √2500 = 50 MPa`
`σ₁ = 20 + 50 = 70 MPa`
`σ₂ = 20 - 50 = -30 MPa`
`τ_max = 50 MPa`

---

**Problem 8: Finding Stresses on an Inclined Plane**
**Given:** σₓ = 100 MPa, σᵧ = 40 MPa, τₓᵧ = 20 MPa.
**Find:** Stresses on a plane inclined at 30° to the vertical.

**Solution (Using Mohr's Circle Concepts):**
**Step 1:** Find C and R.
`C = (100 + 40)/2 = 70 MPa`
`R = √[ ((100-40)/2)² + (20)² ] = √(30² + 20²) = √1300 = 36.06 MPa`

**Step 2:** Find the angle from the principal plane to the given plane. First, find the angle to the principal plane (`2θ_p`).
`tan(2θ_p) = (2*20) / (100-40) = 40/60 = 0.6667`
`2θ_p = arctan(0.6667) ≈ 33.69°`

The angle we need for the inclined plane is `2θ = 2 * 30° = 60°`.
The total angle from the principal plane reference is `60° + 33.69° = 93.69°`.

**Step 3:** Calculate stresses on the inclined plane.
`σ_n = C + R*cos(93.69°) = 70 + 36.06*cos(93.69°) = 70 + (-2.0) ≈ 68.0 MPa`
`τ_n = R*sin(93.69°) = 36.06 * sin(93.69°) = 36.06 * 0.998 ≈ 36.0 MPa`

**Conclusion:** On the 30° plane, normal stress is ~68 MPa, and shear stress is ~36 MPa.

---

**Problem 9: Finding Principal Directions**
**Given:** σₓ = 90 MPa, σᵧ = 30 MPa, τₓᵧ = 40 MPa.
**Find:** Orientation of principal planes (θ_p).

**Solution:**
`tan(2θ_p) = (2 * τₓᵧ) / (σₓ - σᵧ) = (2*40) / (90-30) = 80/60 = 1.333`
`2θ_p = arctan(1.333) ≈ 53.13°`
`θ_p ≈ 26.57°` (from the vertical plane)

---

**Problem 10: Given Stresses, Find Unknowns**
**Given:** On a plane, σ_n = 60 MPa, τ_n = 20 MPa. On another plane perpendicular to the first, σ_n = 20 MPa, τ_n = -20 MPa. (These are σₓ, σᵧ, τₓᵧ).
**Find:** σₓ, σᵧ, τₓᵧ.

**Solution:**
From the data:
`σₓ = 60 MPa`, `τₓᵧ = 20 MPa`
`σᵧ = 20 MPa`, `τₓᵧ = -20 MPa` (Shear on opposite faces are equal and opposite).

So, the state of stress is: `σₓ = 60 MPa, σᵧ = 20 MPa, τₓᵧ = 20 MPa`.

---

**Problem 11: Higher Shear Stress**
**Given:** σₓ = 70 MPa, σᵧ = 10 MPa, τₓᵧ = 50 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (70+10)/2 = 40 MPa`
`R = √[ ((70-10)/2)² + (50)² ] = √(30² + 50²) = √3400 = 58.31 MPa`
`σ₁ = 40 + 58.31 = 98.31 MPa`
`σ₂ = 40 - 58.31 = -18.31 MPa`
`τ_max = 58.31 MPa`

---

**Problem 12: Hydrostatic Stress Component**
**Given:** σₓ = 150 MPa, σᵧ = 150 MPa, τₓᵧ = 40 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (150+150)/2 = 150 MPa`
`R = √[ ((150-150)/2)² + (40)² ] = √(0 + 1600) = 40 MPa`
`σ₁ = 150 + 40 = 190 MPa`
`σ₂ = 150 - 40 = 110 MPa`
`τ_max = 40 MPa`

**Conclusion:** Even with high equal normal stress, max shear is only due to the shear component.

---

**Problem 13: Mostly Compressive**
**Given:** σₓ = -60 MPa, σᵧ = -20 MPa, τₓᵧ = 30 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (-60 + (-20))/2 = -40 MPa`
`R = √[ ((-60 - (-20))/2)² + (30)² ] = √((-20)² + 30²) = √1300 = 36.06 MPa`
`σ₁ = -40 + 36.06 = -3.94 MPa`
`σ₂ = -40 - 36.06 = -76.06 MPa`
`τ_max = 36.06 MPa`

---

**Problem 14: Finding Original State from Principal Stresses**
**Given:** Principal Stresses: σ₁ = 110 MPa, σ₂ = 30 MPa. The principal planes are at 15° and 105°.
**Find:** σₓ, σᵧ, τₓᵧ on the original vertical/horizontal planes.

**Solution:**
**Step 1:** Find C and R.
`C = (σ₁ + σ₂)/2 = (110 + 30)/2 = 70 MPa`
`R = (σ₁ - σ₂)/2 = (110 - 30)/2 = 40 MPa`

**Step 2:** The original planes are at an angle `θ = -15°` from the principal planes. We need to find stresses at `2θ = -30°`.
`σₓ = C + R*cos(2θ) = 70 + 40*cos(-30°) = 70 + 40*(√3/2) = 70 + 34.64 = 104.64 MPa`
`σᵧ = C - R*cos(2θ) = 70 - 40*cos(-30°) = 70 - 34.64 = 35.36 MPa`
`τₓᵧ = R*sin(2θ) = 40*sin(-30°) = 40*(-0.5) = -20 MPa`

---

**Problem 15: Complex State**
**Given:** σₓ = 95 MPa, σᵧ = 35 MPa, τₓᵧ = -50 MPa. (Negative Shear)
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (95+35)/2 = 65 MPa`
`R = √[ ((95-35)/2)² + (-50)² ] = √(30² + 50²) = √3400 = 58.31 MPa`
`σ₁ = 65 + 58.31 = 123.31 MPa`
`σ₂ = 65 - 58.31 = 6.69 MPa`
`τ_max = 58.31 MPa`

---

**Problem 16: Equal Tension and Compression**
**Given:** σₓ = 75 MPa (T), σᵧ = -75 MPa (C), τₓᵧ = 0.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (75 + (-75))/2 = 0 MPa`
`R = √[ ((75 - (-75))/2)² + 0² ] = √(75²) = 75 MPa`
`σ₁ = 0 + 75 = 75 MPa`
`σ₂ = 0 - 75 = -75 MPa`
`τ_max = 75 MPa`

**Conclusion:** This is a case of pure shear, equivalent to Problem 3.

---

**Problem 17: High Difference in Normal Stresses**
**Given:** σₓ = 200 MPa, σᵧ = 50 MPa, τₓᵧ = 30 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (200+50)/2 = 125 MPa`
`R = √[ ((200-50)/2)² + (30)² ] = √(75² + 30²) = √(5625 + 900) = √6525 = 80.78 MPa`
`σ₁ = 125 + 80.78 = 205.78 MPa`
`σ₂ = 125 - 80.78 = 44.22 MPa`
`τ_max = 80.78 MPa`

---

**Problem 18: Low Normal, High Shear**
**Given:** σₓ = 10 MPa, σᵧ = -20 MPa, τₓᵧ = 60 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (10 + (-20))/2 = -5 MPa`
`R = √[ ((10 - (-20))/2)² + (60)² ] = √(15² + 60²) = √(225 + 3600) = √3825 = 61.85 MPa`
`σ₁ = -5 + 61.85 = 56.85 MPa`
`σ₂ = -5 - 61.85 = -66.85 MPa`
`τ_max = 61.85 MPa`

---

**Problem 19: Nearly Zero Minor Principal Stress**
**Given:** σₓ = 80 MPa, σᵧ = 0, τₓᵧ = 40 MPa.
**Find:** σ₁, σ₂, τ_max.

**Solution:**
`C = (80+0)/2 = 40 MPa`
`R = √[ ((80-0)/2)² + (40)² ] = √(40² + 40²) = √3200 = 56.57 MPa`
`σ₁ = 40 + 56.57 = 96.57 MPa`
`σ₂ = 40 - 56.57 = -16.57 MPa`
`τ_max = 56.57 MPa`

---

**Problem 20: Verification Problem**
**Given:** σₓ = 120 MPa, σᵧ = 80 MPa, τₓᵧ = -40 MPa.
**Find:** σ₁, σ₂, τ_max and the angle of the principal plane.

**Solution:**
`C = (120+80)/2 = 100 MPa`
`R = √[ ((120-80)/2)² + (-40)² ] = √(20² + 40²) = √2000 = 44.72 MPa`
`σ₁ = 100 + 44.72 = 144.72 MPa`
`σ₂ = 100 - 44.72 = 55.28 MPa`
`τ_max = 44.72 MPa`

**Find Angle:**
`tan(2θ_p) = (2 * -40) / (120-80) = -80 / 40 = -2`
`2θ_p = arctan(-2) ≈ -63.43°`
`θ_p ≈ -31.72°` (from the vertical plane)

---

### **Final Tips (Bhai Ke Tips):**
1.  **Sign Convention is King:** Always remember:
    *   **Tensile Stress (+ve)**
    *   **Compressive Stress (-ve)**
    *   **Shear Stress causing clockwise rotation (+ve)** (This is the most common convention for Mohr's Circle).
2.  **Center (C)** is always on the σ-axis. It's the average of the two normal stresses.
3.  **Radius (R)** is always positive. It's the hypotenuse of a right-angled triangle.
4.  **τ_max** is always equal to the **Radius (R)**.
5.  **Practice Drawing:** Even if you calculate, try to sketch the circle. It makes understanding the angles much easier.

Bhai, maine poori koshish ki hai in problems ko detailed aur simple banane ki. Agar kisi step mein confusion ho toh pooch lena.
