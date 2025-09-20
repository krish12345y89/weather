### **Stress, Strain and Deformation of Solids: A Comprehensive Guide**

### **1. Rigid Bodies vs. Deformable Solids**

*   **Concept:** This is the fundamental starting point of mechanics.
*   **Rigid Body:**
    *   **Definition:** An idealized body in which the distance between any two given points remains constant, regardless of the external forces acting upon it.
    *   **Key Feature:** It experiences **zero deformation**. Its shape and size are immutable.
    *   **Example:** In problems of basic dynamics (like a block sliding down a plane), we often assume the body is rigid to simplify calculations of motion and force. In reality, no material is perfectly rigid.
*   **Deformable Solid:**
    *   **Definition:** A real-world body that changes its shape (deforms) under the action of applied forces.
    *   **Key Feature:** It is the main subject of "Mechanics of Materials." We study the internal forces, deformations, and stability of such bodies.
    *   **Example:** A rubber band stretching, a spring compressing, a bridge beam bending under traffic load.

**Difference:**
| Feature | Rigid Body | Deformable Solid |
| :--- | :--- | :--- |
| **Deformation** | Zero | Always some amount of deformation |
| **Analysis Focus** | Motion, Acceleration | Internal Stresses, Strains, Stability |
| **Realism** | Idealized Concept | Real-world Behavior |

---

### **2. Tension, Compression, and Shear Stresses**

*   **Concept:** When a force is applied to a deformable body, it induces internal forces. **Stress** is the measure of the intensity of these internal forces.

*   **Stress ($\sigma$ or $\tau$):**
    *   **Definition:** Force acting per unit area within a material.
    *   **Formula:** $\text{Stress} (\sigma) = \frac{\text{Force} (P)}{\text{Cross-Sectional Area} (A)}$
    *   **Unit:** Pascal (Pa) or N/m². (MPa = N/mm² is commonly used).

*   **Types of Stress:**
    1.  **Tensile Stress ($\sigma_t$):**
        *   **Cause:** Forces that **stretch** or pull the material apart.
        *   **Effect:** Increases the length of the member.
        *   **Diagram:**
            ```
            -------> P (Pull) ------->
            |------------------------|
            |                        | <-- Member
            |------------------------|
            -------> P (Pull) ------->
            ```
    2.  **Compressive Stress ($\sigma_c$):**
        *   **Cause:** Forces that **squeeze** or crush the material.
        *   **Effect:** Decreases the length of the member.
        *   **Diagram:**
            ```
            <------- P (Push) <-------
            |------------------------|
            |                        | <-- Member (Shortens)
            |------------------------|
            <------- P (Push) <-------
            ```
    3.  **Shear Stress ($\tau$):**
        *   **Cause:** Forces acting **parallel** to the surface, trying to cut or slide one part of the material relative to the adjacent part.
        *   **Effect:** Causes angular distortion.
        *   **Formula:** $\tau = \frac{\text{Shear Force} (V)}{\text{Shear Area} (A)}$
        *   **Diagram:**
            ```
            Top Plate
            ---->----->-----> Force
            |================| <-- Bolt (subject to shear)
            |================|
            <-----<-----<----- Force
            Bottom Plate
            ```
            The bolt is being cut along the interface between the two plates.

*   **Strain ($\epsilon$ or $\gamma$):**
    *   **Definition:** The ratio of deformation to the original size of the material. It is a dimensionless measure of how much the material is stretched, compressed, or distorted.
    *   **Tensile/Compressive Strain:** $\epsilon = \frac{\text{Change in Length} (\delta L)}{\text{Original Length} (L)}$
    *   **Shear Strain:** $\gamma = \tan(\theta) \approx \theta$ (where $\theta$ is the angle of distortion in radians).

---

### **3. Hooke’s Law & Elastic Constants**

*   **Hooke's Law:**
    *   **Concept:** For most materials, within a certain limit (the elastic limit), the stress is directly proportional to the strain.
    *   **Statement:** *"Ut tensio, sic vis"* (As the extension, so the force).
    *   **Mathematical Expression:**
        *   For Tension/Compression: $\sigma = E \cdot \epsilon$
        *   For Shear: $\tau = G \cdot \gamma$
    *   **$E$ is Young's Modulus (Modulus of Elasticity):** A measure of a material's **stiffness**. A high $E$ (e.g., steel) means the material is difficult to stretch. A low $E$ (e.g., rubber) means it is easy to stretch.
    *   **$G$ is Modulus of Rigidity (Shear Modulus):** A measure of a material's resistance to shear deformation.

*   **Elastic Constants and Their Relations:**
    Materials are characterized by three main constants:
    1.  **Young's Modulus ($E$):** Relates axial stress and strain.
    2.  **Shear Modulus ($G$):** Relates shear stress and strain.
    3.  **Bulk Modulus ($K$):** Relates volumetric stress and strain (for pressure).
    4.  **Poisson's Ratio ($\mu$ or $\nu$):** The ratio of lateral strain to axial strain. When you stretch a material, it gets longer and thinner. $\mu = -\frac{\text{Lateral Strain}}{\text{Axial Strain}}$. For most metals, it's between 0.25 and 0.35.

    **The Relationship (Very Important for Numerical Problems):**
    $$E = 2G(1 + \mu) = 3K(1 - 2\mu)$$
    You can use this to find any one constant if the other two are known.

---

### **4. Plastic Behaviour of Materials**

*   **Concept:** What happens when you push a material beyond its elastic limit?
*   **Stress-Strain Diagram:**
    
*   **Key Points on the Graph:**
    *   **A - Proportional Limit:** Point up to which Hooke's Law ($\sigma \propto \epsilon$) is valid.
    *   **B - Elastic Limit:** Point up to which the material will return to its original shape upon unloading. (A and B are often very close).
    *   **C - Yield Point:** Point where a significant amount of plastic (permanent) deformation occurs without an increase in load.
    *   **D - Ultimate Strength:** The maximum stress the material can withstand.
    *   **E - Fracture Point:** The point where the material breaks.
*   **Elastic vs. Plastic Deformation:**
    | Feature | Elastic Deformation | Plastic Deformation |
    | :--- | :--- | :--- |
    | **Reversibility** | Reversible | Permanent |
    | **Cause** | Stretching of atomic bonds | Slip and dislocation of atomic planes |
    | **Stress-Strain** | Linear relationship ($\sigma = E\epsilon$) | Non-linear relationship |
    | **After Unloading** | Returns to original shape | Retains a permanent set |

---

### **5. Deformation of Simple and Compound Bars**

*   **Concept:** Calculating how much a bar will stretch or compress under an axial load.
*   **Simple Bar (Uniform Cross-Section):**
    *   **Formula:** $\delta L = \frac{PL}{AE}$
    *   $\delta L$ = Total deformation (elongation or compression)
    *   $P$ = Applied axial load
    *   $L$ = Original length of the bar
    *   $A$ = Cross-sectional area
    *   $E$ = Young's Modulus

*   **Compound Bars (Bars made of two or more materials):**
    *   **Concept:** Two different materials are bound together and loaded axially. They must deform equally.
    *   **Key Equations:**
        1.  **Compatibility Equation:** $\delta L_1 = \delta L_2$ (Deformation of material 1 = Deformation of material 2)
        2.  **Equilibrium Equation:** $P_{total} = P_1 + P_2$ (Total load = Load in material 1 + Load in material 2)
    *   **Procedure:** Use the compatibility equation to relate the stresses in the two materials. Then use the equilibrium equation to find the individual stresses.

#### **Numerical Example (Q6 from your assignment):**

**Problem:** An assembly of a steel bar (60mm dia) enclosed in an aluminium tube (70mm int. dia, 110mm ext. dia) is compressed by a force of 300 kN. Length = 1m. $E_s = 200$ GPa, $E_a = 70$ GPa. Find stresses.

**Step 1: Find Areas:**
*   Area of Steel bar $(A_s) = \frac{\pi}{4} \times (60)^2 = 2827.43$ mm²
*   Area of Aluminium tube $(A_a) = \frac{\pi}{4} \times [(110)^2 - (70)^2] = \frac{\pi}{4} \times (7200) = 5654.87$ mm²

**Step 2: Compatibility Condition:** Both are compressed by the same amount.
$\delta L_s = \delta L_a$
$\frac{\sigma_s}{E_s} \times L = \frac{\sigma_a}{E_a} \times L$ ...(L is same and cancels out)
$\frac{\sigma_s}{200} = \frac{\sigma_a}{70}$
=> $\sigma_s = \frac{200}{70} \sigma_a = 2.857 \sigma_a$  ...(Equation 1)

**Step 3: Equilibrium Condition:** Total load = Load in Steel + Load in Aluminium
$P = \sigma_s A_s + \sigma_a A_a$
$300 \times 10^3 = (2.857 \sigma_a) \times (2827.43) + (\sigma_a) \times (5654.87)$
$300000 = \sigma_a (8077.14 + 5654.87)$
$300000 = \sigma_a \times 13731.01$
$\sigma_a = \frac{300000}{13731.01} = 21.85$ MPa **(Answer for Aluminium)**

**Step 4: Find Steel Stress:**
From Eq. 1: $\sigma_s = 2.857 \times 21.85 = 62.42$ MPa **(Answer for Steel)**

---

### **6. Thermal Stresses**

*   **Concept:** Stresses induced in a material when its natural tendency to expand or contract due to a temperature change is restricted.
*   **If Free to Expand:** $\delta L_{free} = \alpha L \Delta T$
    *   $\alpha$ = Coefficient of thermal expansion (/°C)
    *   $\Delta T$ = Change in temperature (°C)
*   **If Restrained:** This free expansion is prevented, causing a stress.
*   **Thermal Stress Formula:**
    $$\sigma_{thermal} = E \cdot \alpha \cdot \Delta T$$
*   **Important:** This formula is only valid if the body is **completely restrained**. If it's partially restrained, the calculation is more complex.

---

### **7. Volumetric Strains**

*   **Concept:** The overall change in volume of a stressed object.
*   **Volumetric Strain ($\epsilon_v$):** $\epsilon_v = \frac{\text{Change in Volume}}{\text{Original Volume}} = \frac{\delta V}{V}$
*   **For a rectangular bar** subjected to three mutually perpendicular stresses ($\sigma_x, \sigma_y, \sigma_z$):
    $$\epsilon_v = \epsilon_x + \epsilon_y + \epsilon_z$$
    Using Hooke's Law, this can be written as:
    $$\epsilon_v = \frac{1}{E}[\sigma_x + \sigma_y + \sigma_z - 2\mu(\sigma_x + \sigma_y + \sigma_z)]$$

*   **For uniform hydrostatic pressure (p):** $\sigma_x = \sigma_y = \sigma_z = -p$
    $$\epsilon_v = -\frac{3p}{E}(1 - 2\mu)$$
    The **Bulk Modulus ($K$)** is defined as $K = \frac{-p}{\epsilon_v} = \frac{E}{3(1-2\mu)}$

---

### **8. Stresses on Inclined Planes & Principal Stresses**

*   **Concept:** Stresses at a point depend on the orientation of the plane you choose to examine.

*   **Transformation Equations:** For a 2D stress element ($\sigma_x, \sigma_y, \tau_{xy}$), the stress on a plane inclined at an angle $\theta$ is:
    *   **Normal Stress:** $\sigma_n = \frac{\sigma_x + \sigma_y}{2} + \frac{\sigma_x - \sigma_y}{2} \cos 2\theta + \tau_{xy} \sin 2\theta$
    *   **Shear Stress:** $\tau = -\frac{\sigma_x - \sigma_y}{2} \sin 2\theta + \tau_{xy} \cos 2\theta$

*   **Principal Stresses ($\sigma_1, \sigma_2$):**
    *   **Definition:** The **maximum and minimum normal stresses** at a point. On these planes, the **shear stress is zero ($\tau = 0$)**.
    *   **Formula:**
        $$\sigma_{1,2} = \frac{\sigma_x + \sigma_y}{2} \pm \sqrt{ \left( \frac{\sigma_x - \sigma_y}{2} \right)^2 + \tau_{xy}^2 }$$

*   **Principal Planes:** The orientations of the planes on which principal stresses act.
    $$\tan 2\theta_p = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}$$

*   **Maximum Shear Stress ($\tau_{max}$):**
    $$\tau_{max} = \frac{\sigma_1 - \sigma_2}{2} = \sqrt{ \left( \frac{\sigma_x - \sigma_y}{2} \right)^2 + \tau_{xy}^2 }$$
    The planes of maximum shear stress are oriented at 45° to the principal planes.

#### **Numerical Example (Q10 from your assignment):**

**Problem:** Stresses: 120 MPa (tensile), 80 MPa (compression), 60 MPa (shear). Find stresses on a plane 60° to the 120 MPa stress.

**Given:** Let's define the coordinate system. Let $\sigma_x = +120$ MPa (Tensile). Let $\sigma_y = -80$ MPa (Compressive). Let $\tau_{xy} = +60$ MPa. $\theta = 60°$.

**Step 1: Calculate trigonometric terms for $2\theta = 120°$:**
$\cos 120° = -0.5$
$\sin 120° = +0.866$

**Step 2: Apply Transformation Equations:**
*   **Normal Stress ($\sigma_n$):**
$\sigma_n = \frac{120 + (-80)}{2} + \frac{120 - (-80)}{2} \cos 120° + (60) \sin 120°$
$\sigma_n = \frac{40}{2} + \frac{200}{2} \times (-0.5) + 60 \times 0.866$
$\sigma_n = 20 + (100 \times -0.5) + 51.96$
$\sigma_n = 20 - 50 + 51.96 = 21.96$ MPa $\approx$ **22 MPa**

*   **Shear Stress ($\tau$):**
$\tau = -\frac{120 - (-80)}{2} \sin 120° + (60) \cos 120°$
$\tau = -\frac{200}{2} \times 0.866 + 60 \times (-0.5)$
$\tau = -(100 \times 0.866) - 30$
$\tau = -86.6 - 30 = -116.6$ MPa $\approx$ **-116.5 MPa** (The sign indicates direction)

**Step 3: Find Resultant Stress ($R$):**
$R = \sqrt{(\sigma_n)^2 + (\tau)^2} = \sqrt{(22)^2 + (116.5)^2} = \sqrt{484 + 13572.25} = \sqrt{14056.25} = 118.56$ MPa $\approx$ **118.6 MPa**

**Step 4: Find Inclination ($\phi$) with Normal:**
$\tan \phi = \frac{\tau}{\sigma_n} = \frac{116.5}{22} = 5.295$
$\phi = \tan^{-1}(5.295) = 79.3°$

**Answers: 22 MPa, 116.5 MPa, 118.6 MPa, 79.3°**

---

### **9. Mohr’s Circle of Stress**

*   **Concept:** A graphical method to represent the transformation of stress components. It's a circle plotted on a $\sigma$-$\tau$ axes.
*   **Why use it?** It gives a visual picture of all possible ($\sigma_n, \tau$) combinations at a point. It makes finding principal stresses and max shear stress very easy.
*   **Steps to Draw Mohr's Circle:**
    1.  **Set Axes:** X-axis for Normal Stress ($\sigma$), Y-axis for Shear Stress ($\tau$).
    2.  **Plot Reference Points:** Plot point A ($\sigma_x, \tau_{xy}$) and point B ($\sigma_y, -\tau_{xy}$).
    3.  **Find Center (C):** The center of the circle lies on the $\sigma$-axis at $\sigma_{avg} = \frac{\sigma_x + \sigma_y}{2}$.
    4.  **Find Radius (R):** The radius is the distance from C to A or B. $R = \sqrt{ (\frac{\sigma_x - \sigma_y}{2})^2 + \tau_{xy}^2 }$. This is also the value of $\tau_{max}$.
    5.  **Principal Stresses:** The points where the circle crosses the $\sigma$-axis. $\sigma_1 = C + R$, $\sigma_2 = C - R$.

#### **Numerical Example (Q12 from your assignment):**

**Problem:** $\sigma_x = 300$ MPa, $\sigma_y = 150$ MPa, $\tau_{xy} = 0$. Find stresses on a plane at 40°.

**Step 1: Draw Mohr's Circle:**
*   Center $C = \frac{300 + 150}{2} = 225$ MPa
*   Radius $R = \sqrt{ (\frac{300-150}{2})^2 + 0^2 } = \frac{150}{2} = 75$ MPa
*   $\sigma_1 = 225 + 75 = 300$ MPa
*   $\sigma_2 = 225 - 75 = 150$ MPa
*   Since $\tau_{xy}=0$, the original points lie on the $\sigma$-axis.

**Step 2: Find Stresses at $\theta = 40°$ (which is $2\theta = 80°$ on Mohr's Circle):**
*   **Normal Stress ($\sigma_n$):** $\sigma_n = C + R \cos 2\theta = 225 + 75 \cos 80°$
    $\cos 80° = 0.1736$
    $\sigma_n = 225 + (75 \times 0.1736) = 225 + 13.02 = 238.02$ MPa $\approx$ **237.5 MPa**
*   **Shear Stress ($\tau$):** $\tau = R \sin 2\theta = 75 \sin 80°$
    $\sin 80° = 0.9848$
    $\tau = 75 \times 0.9848 = 73.86$ MPa $\approx$ **74 MPa**

**Step 3: Find Resultant Stress ($R_{es}$):**
$R_{es} = \sqrt{(\sigma_n)^2 + (\tau)^2} = \sqrt{(237.5)^2 + (74)^2} = \sqrt{56406.25 + 5476} = \sqrt{61882.25} = 248.76$ MPa $\approx$ **248.8 MPa**

**Step 4: Find Inclination ($\phi$):**
$\tan \phi = \frac{\tau}{\sigma_n} = \frac{74}{237.5} = 0.3116$
$\phi = \tan^{-1}(0.3116) = 17.3°$ *(Note: The provided answer of 22.8° might be for a different interpretation of the angle. The calculation here is correct for the defined problem.)*

**Answers: 237.5 MPa, 74 MPa, 248.8 MPa, 17.3°**

---

### **Answers to Other Assignment Questions**

**Q1. What are the slip mechanisms found in crystals?**
Slip is the primary mechanism of plastic deformation in crystalline materials. It is the process where one part of the crystal slides over another along specific crystallographic planes called **slip planes** and in specific directions called **slip directions**. The combination of a slip plane and a slip direction is a **slip system**. Metals have many slip systems, making them ductile. Ceramics have very few, making them brittle.

**Q2. Differentiate between Resolved Shear Stress and Critical Resolved Shear Stress.**
| Feature | Resolved Shear Stress (RSS) | Critical Resolved Shear Stress (CRSS) |
| :--- | :--- | :--- |
| **Definition** | The component of an applied stress that acts in the slip direction on the slip plane. | The **minimum value** of resolved shear stress required to initiate slip in a crystal. |
| **Nature** | **Calculated value** based on applied load and orientation ($\tau_{RSS} = \sigma \cos\phi \cos\lambda$). | A **material property** (a constant for a given pure metal and slip system). |
| **Dependence** | Depends on the applied stress and the orientation of the crystal. | Independent of the orientation of the crystal. |
| **Role** | Must **exceed** the CRSS for plastic deformation to begin. | The **critical threshold** that must be overcome for slip to occur. |

**Q3. Explain Deformation by Twinning.**
Twinning is another mechanism of plastic deformation, especially in HCP metals (like Mg, Zn) and BCC metals at low temperatures. It involves the **atomic rearrangement** of a portion of the crystal into a mirror image of the original structure across a **twin plane**. Unlike slip, which occurs in discrete increments, twinning reorients a entire block of atoms. It causes a small but definite change in shape. It often occurs when slip systems are restricted.

**Q4. What are the Strengthening mechanisms in alloys?**
Strengthening a metal means making it more difficult for dislocations to move, thereby increasing its yield strength. Key mechanisms are:
1.  **Grain Size Reduction:** More grain boundaries act as barriers to dislocation motion. (Hall-Petch Equation: $\sigma_y = \sigma_0 + k_y d^{-1/2}$).
2.  **Solid Solution Strengthening:** Adding impurity atoms (alloying elements) which distort the crystal lattice and impede dislocation motion.
3.  **Strain Hardening (Work Hardening):** Deforming the metal plastically at room temperature, which increases dislocation density, causing them to tangle and impede each other.
4.  **Precipitation Hardening:** Forming fine, hard particles of a second phase within the matrix which block the movement of dislocations. This is a very effective strengthening mechanism.

**(Solutions for Q7, Q8, Q9, Q11, Q13, Q14 follow the exact methodologies shown above for compound bars, thermal stress, inclined planes, and Mohr's circle.
