Of course, bhai! Ye lo, poora syllabus ekdam simple language mein, step-by-step, with formulas and numericals. Sab kuch aasan examples ke saath samjhane ki koshish ki hai.

---

# **Stress, Strain and Deformation of Solids: Complete Notes**

## **1. Rigid Bodies vs. Deformable Solids**

### **Rigid Body (कड़ा पिंड)**
*   **Kya Hai?** Yeh ek aisa perfect (आदर्श) body hai jiska **shape aur size kabhi nahi badalta**, chahe kitna bhi force lagao. Hume pata hai real life mein aisa kuch nahi hota, par calculations aasan karne ke liye hum maan lete hain.
*   **Example:** Jaise hi koi block force lagane par apna shape change na kare, woh rigid body hai.

### **Deformable Solid (विकृत होने वाला ठोस)**
*   **Kya Hai?** Yeh woh body hoti hai jiska **shape aur size force lagane par badal jata hai**. Real life ke saare solids, jaise steel, rubber, plastic, yeh sab deformable hote hain.
*   **Example:** Rubber band khinchne par lambi ho jati hai. Steel ka rod bhi thoda sa bend ho jata hai.

---

## **2. Tension, Compression & Shear Stresses (तनाव, संपीड़न और कतरनी प्रतिबल)**

**Stress (प्रतिबल)** = Force (बल) / Area (क्षेत्रफल)
Its SI unit is **Pascal (Pa)** or **N/m²**.

### **(a) Tensile Stress (तन्य प्रतिबल - खिचाव)**
*   **Kya Hai?** Jab kisi object ko kheechkar uski length badhaye.
*   **Formula:**
    `σ_t = P / A`
    *   `σ_t` = Tensile Stress
    *   `P` = Pulling (Tensile) Force
    *   `A` = Cross-sectional Area

### **(b) Compressive Stress (संपीडन प्रतिबल - दबाव)**
*   **Kya Hai?** Jab kisi object ko dabakar uski length ghataaye.
*   **Formula:**
    `σ_c = P / A`
    *   `σ_c` = Compressive Stress
    *   `P` = Pushing (Compressive) Force
    *   `A` = Cross-sectional Area

### **(c) Shear Stress (कर्तन प्रतिबल - कटाव)**
*   **Kya Hai?** Jab force aisa lagaye ki object ki ek layer dusri layer ke upar fisalne lage.
*   **Formula:**
    `τ = P / A`
    *   `τ` = Shear Stress
    *   `P` = Shear Force
    *   `A` = Area resisting shear

**📌 Example:** Scissors se paper kaatna, ya fir ek packet chips kholna.

---

## **3. Hooke’s Law & Elastic Constants (हुक का नियम और प्रत्यास्थता नियतांक)**

### **Hooke’s Law (हुक का नियम)**
*   **Kya Kehta Hai?** "Elastic limit tak, stress, strain ke **directly proportional (सीधे समानुपातिक)** hota hai."
*   **Formula:** `Stress ∝ Strain` OR `E = Stress / Strain`
    *   `E` is Young's Modulus.

### **Elastic Constants (प्रत्यास्थता नियतांक)**
Yeh 4 constants hote hain jo material ki stiffness (कड़ापन) batate hain.

1.  **Young’s Modulus (E):** `E = Tensile Stress / Tensile Strain`
    *   *Longitudinal (लंबवत) stiffness measure karta hai.*

2.  **Shear Modulus (G):** `G = Shear Stress / Shear Strain`
    *   *Shape change ki resistance measure karta hai.*

3.  **Bulk Modulus (K):** `K = Direct Stress / Volumetric Strain`
    *   *Volume change ki resistance measure karta hai. (Jaise water mein dabav)*

4.  **Poisson’s Ratio (μ or ν):** `ν = - (Lateral Strain / Longitudinal Strain)`
    *   *Jab aap kheechte ho to length badhti hai aur width ghatti hai, uska ratio.*

### **Relations Between Elastic Constants (सूत्र)**
In chaaro constants ka aapas mein relation hota hai. Ye formulas yaad rakhna:
*   `E = 2G(1 + ν)`
*   `E = 3K(1 - 2ν)`
*   `E = (9KG) / (3K + G)`

---

## **4. Plastic Behaviour of Materials (प्लास्टिक व्यवहार)**

*   **Elastic Region (प्रत्यास्थ क्षेत्र):** Jab tak load elastic limit se kam hai, load hatate hi body apna original shape wapas le aati hai. (Jaise spring)
*   **Plastic Region (प्लास्टिक क्षेत्र):** Jab load elastic limit se zyada ho jata hai, to body **permanently deform** ho jati hai. Load hatane par bhi shape wapas nahi aati.
*   **Ductile vs Brittle:**
    *   **Ductile Material (आघातवर्धनीय):** Ye bahut deform hoke bhi nahi tootega (e.g., Copper, Gold, Steel).
    *   **Brittle Material (भंगुर):** Ye bina zyada deform hue directly toot jayega (e.g., Glass, Cast Iron).

---

## **5. Deformation of Simple and Compound Bars (विकृति)**

### **(a) Simple Bar (साधारण छड़)**
Simple bar ki deformation (length mein change) nikalne ka formula:
`ΔL = (P * L) / (A * E)`
*   `ΔL` = Change in Length
*   `P` = Axial Load (Tensile or Compressive)
*   `L` = Original Length
*   `A` = Cross-sectional Area
*   `E` = Young’s Modulus

### **(b) Compound Bars (मिश्रित छड़)**
*   **Series Connection (श्रृंखला में):** Load sab par same hota hai, total deformation alag-alag bars ki deformation ka sum hota hai.
    `Total ΔL = ΔL1 + ΔL2 + ... = (PL1)/(A1E1) + (PL2)/(A2E2) + ...`

*   **Parallel Connection (समानांतर में):** Deformation sab bars ki same hoti hai, load alag-alag bars mein bat jata hai.
    `P = P1 + P2` and `ΔL1 = ΔL2`
    Isme load distribution ke liye: `P1/(A1E1) = P2/(A2E2)`

---

## **6. Thermal Stresses (तापीय प्रतिबल)**

Jab kisi material ko garm kiya jata hai, toh woh failna (expand) chahta hai. Agar use failne nahi diya jata (jaise kisi rod ke dono ends fixed hon), toh uske andar stress paida hota hai. Use kehte hain **Thermal Stress**.

**Formula:**
`σ_thermal = E * α * ΔT`
*   `σ_thermal` = Thermal Stress
*   `E` = Young’s Modulus
*   `α` = Coefficient of thermal expansion (/°C)
*   `ΔT` = Temperature change (°C)

**📌 Numerical:**
**Q.** A steel rod (E = 200 GPa, α = 12 × 10⁻⁶ /°C) is held between two rigid walls. If its temperature is increased by 50°C, calculate the thermal stress developed.
**Sol.:**
`σ_thermal = E * α * ΔT`
`= (200 × 10⁹) × (12 × 10⁻⁶) × (50)`
`= 120,000,000 Pa` or **120 MPa** (Compressive)

---

## **7. Volumetric Strains (आयतनिक विकृति)**

Volumetric Strain (ε_v) woh hoti hai jab poore object ka volume change hota hai.
`ε_v = Change in Volume / Original Volume = ΔV / V`

**Formula for a cube with 3 stresses:**
`ε_v = (σx + σy + σz)/E * (1 - 2ν)`

**Agar sab taraf same pressure 'p' lag raha ho (Hydrostatic Pressure):**
`ε_v = (3p / E) * (1 - 2ν)`

---

## **8. Stresses on Inclined Planes (झुके हुए तल पर प्रतिबल)**

Kisi bhi inclined plane (tircha/tedha plane) par do prakar ke stresses hote hain:
1.  **Normal Stress (σ_θ):** Jo plane ke perpendicular (लंबवत) lagta hai.
2.  **Shear Stress (τ_θ):** Jo plane ke parallel (समानांतर) lagta hai.

**Formulas (if only σx is applied):**
*   Normal Stress, `σ_θ = σx * cos²θ`
*   Shear Stress, `τ_θ = (σx / 2) * sin2θ`

**Yaha **θ** vertical axis se inclined plane ka angle hai.**

**Important Point:** **θ = 45°** par **Shear Stress maximum** hota hai. `τ_max = σx / 2`
Isliye ductile materials (jaise steel) 45° ke angle par shear fail hote hain.

---

## **9. Principal Stresses & Principal Planes (मुख्य प्रतिबल और मुख्य तल)**

*   **Principal Planes (मुख्य तल):** Yeh woh special inclined planes hote hain jinka orientation (कोण) aisa hota hai ki **un par shear stress bilkul zero (शून्य)** hota hai.
*   **Principal Stresses (मुख्य प्रतिबल):** Principal planes par jo normal stress lagta hai use kehte hain Principal Stress. Yeh **maximum aur minimum possible normal stresses** hote hain pure body par.

**Formulas (for general 2D stress σx, σy, τxy):**
*   **Orientation of Principal Planes:**
    `tan(2θ_p) = (2 * τxy) / (σx - σy)`
    Is equation se `θ_p` nikaloge.

*   **Magnitude of Principal Stresses (σ1 & σ2):**
    `σ1, σ2 = ( (σx + σy) / 2 ) ± √( [ (σx - σy) / 2 ]² + τxy² )`
    *   `σ1` is always **Maximum** Principal Stress.
    *   `σ2` is always **Minimum** Principal Stress.

---

## **10. Mohr’s Circle of Stress (मोहर का वृत्त)**

Mohr's Circle ek graphical method hai jisse aap kisi bhi angle θ par stress, principal stresses, max shear stress, etc. aaram se find kar sakte ho.

**Steps to Draw Mohr's Circle:**
1.  **Coordinates Banayo:** X-axis = Normal Stress (σ), Y-axis = Shear Stress (τ).
2.  **Plot Points:** Point C1 (`σx`, `τxy`) and Point C2 (`σy`, `-τxy`).
3.  **Center (C):** Dono points ko milaye, center X-axis par hoga.
    `C = ( (σx + σy)/2 , 0 )`
4.  **Radius (R):** `R = √( [ (σx - σy)/2 ]² + τxy² )`
5.  **Circle Banayo:** Center `C` aur radius `R` leke circle draw karo.

**Results from the Circle:**
*   **Principal Stresses:** Circle jaha X-axis ko katata hai wahi σ1 aur σ2 hote hain.
    `σ1 = C + R`, `σ2 = C - R`
*   **Maximum Shear Stress:** Circle ka topmost point, `τ_max = R`

**📌 Example:**
**Q.** For a point, σx = 80 MPa, σy = 20 MPa, τxy = 30 MPa. Find σ1, σ2, τ_max using Mohr's Circle.
**Sol.:**
1.  Center, `C = (80 + 20)/2 = 50 MPa`
2.  Radius, `R = √( [(80-20)/2]² + (30)² ) = √( (30)² + (30)² ) = √1800 ≈ 42.43 MPa`
3.  **σ1 = C + R = 50 + 42.43 = 92.43 MPa**
4.  **σ2 = C - R = 50 - 42.43 = 7.57 MPa**
5.  **τ_max = R = 42.43 MPa**

---

## **📝 Practice Numerical Problems**

1.  A mild steel bar of 20 mm diameter and 300 mm long is subjected to a tensile load of 50 kN. Find the stress, strain, and elongation. Take E = 200 GPa.
2.  A composite bar is made of a central steel plate (60mm wide, 10mm thick) sandwiched between two copper plates (60mm wide, 5mm thick each). If the bar is subjected to a tensile load of 50 kN, find the stresses in each material and the total elongation. Take E_steel = 200 GPa, E_copper = 100 GPa, Length = 200mm.
3.  A steel rod of 20 mm diameter is heated from 20°C to 120°C. If the ends are rigidly fixed, calculate the thermal stress developed. (α = 12 × 10⁻⁶ /°C, E = 200 GPa).
4.  At a point in a material, the stresses are σx = 60 MPa (Tensile), σy = 40 MPa (Compressive), and τxy = 30 MPa. Find the principal stresses and their directions using the formulas. Also, find the maximum shear stress.

Bhai, poora syllabus cover ho gaya hai. Har cheez ko basics se samjhane ki koshish ki hai. Agar koi specific numerical solve karni ho ya koi concept aur clear karne ka ho, to bata dena.
