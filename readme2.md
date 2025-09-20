# 📘 Mechanics of Solids: Rigid Body, Deformable Solids, Stress, Strain & Mohr's Circle

## 📚 Table of Contents
1. [Rigid Body & Deformable Solids](#-rigid-body--deformable-solids)
2. [Types of Stress in Solids](#-stress-types-in-solids)
3. [Elastic Constants](#-elastic-constants)
4. [Plasticity of Materials](#-plasticity-of-materials)
5. [Deformation of Bars](#-deformation-of-simple-and-compound-bars)
6. [Thermal Stress & Volumetric Strain](#-thermal-stress--volumetric-strain)
7. [Stresses on Inclined Planes](#-stresses-on-inclined-planes)
8. [Principal Stresses & Principal Planes](#-principal-stresses-and-principal-planes)
9. [Mohr's Circle of Stress](#-mohrs-circle-of-stress)

---

## 🔹 Rigid Body & Deformable Solids
[📺 Video Link](https://youtu.be/kQHtgtq-6gw?si=IyuFnTSvGFG7KToU)

### 🔹 What is a Rigid Body?
- **Definition**: A rigid body is an idealization where the body's shape or size never deforms under pressure, force, or motion.
- **Scientific View**: A rigid body is a collection of many small particles where the distance between them remains constant, whether at rest or in motion.
- **Reality Check**: Perfect rigid bodies don't exist in real life. Under extreme force or near light speed, deformation occurs. However, the concept simplifies physics and engineering calculations.

### 🔹 Examples of Rigid Body Behavior
1. **Block 1**: Broke when pressed → Not rigid.
2. **Block 2**: Shape changed (rectangular to arc) → Not rigid.
3. **Block 3**: Shape remained unchanged under force → Rigid body example.

### 🔹 Deformable Body
- A deformable body changes shape or size when external force, load, or pressure is applied.
- Most real-world solids are deformable (e.g., steel deforms slightly, rubber deforms significantly).
- In engineering, small deformations are often ignored, and the body is treated as rigid.

### 🔹 Particle vs Rigid Body
| Property         | Particle                          | Rigid Body                          |
|------------------|-----------------------------------|-------------------------------------|
| Size & Shape     | Doesn’t matter, treated as point mass | Has definite shape & size         |
| Representation   | A small point                     | Collection of many particles       |
| Deformation      | Not applicable                    | Assumed not to deform              |

### 🔹 Rigid Body Mechanics
- **Statics**: Rigid body at rest or in equilibrium (e.g., girl sitting on a chair, forces balanced).
- **Dynamics**: Rigid body in motion (e.g., moving car, shape unchanged).

### 🔹 Summary
- **Rigid Body**: Shape and size don’t change; deformation ignored.
- **Deformable Body**: Shape and size change under load.
- **Engineering Use**: Rigid body simplification makes calculations easier.

---

## 📦 Stress Types in Solids
[📺 Video Link](https://youtu.be/MtNfwMweFt0?si=6Z0-rcNQuMgTCCaI)

### 1. Tensile Stress (तनाव / खिंचाव तनाव)
- **Definition**: Stress developed per unit area when a body is pulled axially.
- **Formula**:  
  \(\sigma_t = \frac{P}{A}\)  
  Where:  
  \(\sigma_t\) = Tensile Stress,  
  \(P\) = Pulling Force (N),  
  \(A\) = Cross-sectional Area (mm²).  
- **Example**: Steel rod pulled at both ends.

### 2. Compressive Stress (दाब / संपीड़न तनाव)
- **Definition**: Stress developed per unit area when a body is pushed axially.
- **Formula**:  
  \(\sigma_c = \frac{P}{A}\)  
  Where:  
  \(\sigma_c\) = Compressive Stress,  
  \(P\) = Compressive Force (N),  
  \(A\) = Cross-sectional Area (mm²).  
- **Example**: Concrete column under building load.

### 3. Shear Stress (कतरनी तनाव)
- **Definition**: Stress developed per unit area when layers of material slide over each other.
- **Formula**:  
  \(\tau = \frac{P}{A}\)  
  Where:  
  \(\tau\) = Shear Stress,  
  \(P\) = Shear Force (N),  
  \(A\) = Area resisting shear (mm²).  
- **Example**: Scissors cutting paper, rivet joint.

### 📊 Summary Table
| Stress Type          | Force Direction (English) | बल की दिशा (Hindi) | Formula     | Example               |
|----------------------|---------------------------|-------------------|-------------|-----------------------|
| Tensile Stress       | Pulling (Outward)         | खींचना / तनना    | \(\sigma = \frac{P}{A}\) | Rod under pulling load |
| Compressive Stress   | Pushing (Inward)          | दबाना / संपीड़न  | \(\sigma = \frac{P}{A}\) | Concrete column       |
| Shear Stress         | Sliding / Tangential      | कतरनी / फिसलाना  | \(\tau = \frac{P}{A}\)  | Scissors cutting paper |

---

## 📘 Elastic Constants
[📺 Video Link](https://youtu.be/sZi0W3pr8Jg?si=E0SqGW7bI3k6rGLa)

### 1. Poisson’s Ratio (ν / μ)
- **Definition**: Ratio of lateral strain to longitudinal strain.  
  \(\nu = \frac{\text{Lateral Strain}}{\text{Longitudinal Strain}}\)
- **Value Range**:  
  Glass: 0.05–0.1, Concrete: 0.1–0.2, Metals: 0.25–0.42, Rubber: 0.45–0.5.

### 2. Shear Modulus (G or C or N)
- **Definition**: Ratio of shear stress to shear strain.  
  \(G = \frac{\tau}{\phi}\)  
  Where:  
  \(\tau\) = Shear Stress,  
  \(\phi\) = Shear Strain.

### 3. Bulk Modulus (K)
- **Definition**: Ratio of direct stress to volumetric strain.  
  \(K = \frac{\sigma}{\Delta V / V}\)  
  Where:  
  \(\sigma\) = Direct Stress,  
  \(\Delta V/V\) = Volumetric Strain.

### 4. Young’s Modulus (E)
- **Definition**: Ratio of tensile/compressive stress to longitudinal strain.  
  \(E = \frac{\sigma}{\varepsilon}\)  
  Where:  
  \(\sigma\) = Normal Stress,  
  \(\varepsilon\) = Longitudinal Strain.

### 📐 Relationships Between Elastic Constants
1. \(E = 3K(1 - 2\nu)\)
2. \(E = 2G(1 + \nu)\)
3. \(E = \frac{9KG}{3K + G}\)
4. \(\nu = \frac{3K - 2G}{6K + 2G}\)

### 🔢 Numerical Example
**Q:** A steel bar subjected to tensile stress of 100 MPa. Young’s modulus = 200 GPa, Poisson’s ratio = 0.3. Find longitudinal strain, lateral strain, and volumetric strain.  
**Solution:**  
- Longitudinal strain:  
  \(\varepsilon = \frac{\sigma}{E} = \frac{100 \times 10^6}{200 \times 10^9} = 0.0005\)  
- Lateral strain:  
  \(\varepsilon_{\text{lat}} = -\nu \times \varepsilon = -0.3 \times 0.0005 = -0.00015\)  
- Volumetric strain:  
  \(\varepsilon_v = \varepsilon(1 - 2\nu) = 0.0005(1 - 0.6) = 0.0002\)

---

## 📘 Plasticity of Materials
[📺 Video Link](https://youtu.be/fbLnyQjIq3Q?si=v6Dms2eTbdfh9Lx-)

### 1. Definition
- **English**: Property enabling permanent deformation without fracture when stress exceeds elastic limit.
- **Hindi**: Material की वह property जो स्थायी deformation ermöglicht जब stress elastic limit से अधिक हो।

### 2. Elastic vs Plastic
- **Elastic Region**: Load हटाने पर material original shape में वापस आता है।
- **Plastic Region**: Load हटाने पर भी material permanently deformed रहता है।

### 3. Examples
- **Highly Plastic**: Clay, Lead, Gold, Copper, Aluminium.
- **Low Plastic**: Cast Iron, Glass (brittle).
- **Special Case**: Rubber (elastic, not plastic).

### 4. Stress-Strain Curve (Mild Steel)
- O → A: Elastic region (Hooke’s law valid).
- A → B: Yield point (plasticity starts).
- B → C: Strain hardening.
- C → D: Ultimate stress.
- D → E: Fracture.

### 5. Applications
- Metal forming (forging, rolling, extrusion).
- Manufacturing utensils, automobile parts.
- Soil mechanics (clay shows plastic behavior).

### ✨ Summary
- Plasticity: Permanent deformation ability beyond elastic limit.
- High plasticity = ductile metals; Low plasticity = brittle materials.

---

## 📘 Deformation of Simple and Compound Bars
[📺 Video Link](https://youtu.be/FwOsoeOvZzo?si=u9qjXBLpUEK1CvrI)

### 1. Deformation Basics
- Change in length due to axial load (tensile/compressive).

### 2. Deformation of Simple Bar
- Formula:  
  \(\Delta L = \frac{P \cdot L}{A \cdot E}\)  
  Where:  
  \(\Delta L\) = Change in length,  
  \(P\) = Axial load,  
  \(L\) = Original length,  
  \(A\) = Cross-sectional area,  
  \(E\) = Young’s modulus.

### 3. Deformation of Compound Bars
- **Bars in Series**: Total deformation = sum of deformations.  
  \(\Delta L = \sum \frac{P \cdot L_i}{A_i \cdot E_i}\)
- **Bars in Parallel**: Load divides, deformation equal.  
  \(\frac{P_1}{A_1 E_1} = \frac{P_2}{A_2 E_2}\),  
  \(\Delta L = \frac{P_1 L}{A_1 E_1}\)

### 4. Applications
- Railway tracks (steel + concrete).
- Bridges, pressure vessels, RCC columns.

---

## 🌡️ Thermal Stress & Volumetric Strain
[📺 Video Link](https://youtu.be/FwOsoeOvZzo?si=u9qjXBLpUEK1CvrI)

### 1. Thermal Stress
- Develops when expansion/contraction is restricted.  
  \(\sigma_{\text{th}} = E \cdot \alpha \cdot \Delta T\)  
  Where:  
  \(E\) = Young’s modulus,  
  \(\alpha\) = Coefficient of linear expansion,  
  \(\Delta T\) = Temperature change.

### 2. Volumetric Strain
- Change in volume per unit volume.  
  \(\varepsilon_v = \frac{\Delta V}{V} = \frac{\sigma_x + \sigma_y + \sigma_z}{E}(1 - 2\mu)\)  
  For hydrostatic stress:  
  \(\varepsilon_v = \frac{3p}{E}(1 - 2\mu)\)

### 🔢 Example
**Thermal Stress**: Steel rod fixed at both ends, \(L = 2m\), \(\alpha = 12 \times 10^{-6}/°C\), \(E = 200\) GPa, \(\Delta T = 50°C\).  
\(\sigma_{\text{th}} = 200 \times 10^9 \times 12 \times 10^{-6} \times 50 = 120\) MPa (tensile).

---

## 📘 Stresses on Inclined Planes
[📺 Video Link](https://youtu.be/RnW4S-Iob3E?si=z4tSUB-N2yWqVS6Q)

### 1. Introduction
- Stresses act on inclined planes: normal stress (\(\sigma_n\)) and shear stress (\(\tau\)).

### 2. Uniaxial Stress (\(\sigma_x\) only)
- Normal stress:  
  \(\sigma_n = \sigma_x \cos^2 \theta\)
- Shear stress:  
  \(\tau = \sigma_x \sin \theta \cos \theta\)
- Max shear at \(\theta = 45°\):  
  \(\tau_{\text{max}} = \frac{\sigma_x}{2}\)

### 3. Biaxial Stress (\(\sigma_x, \sigma_y\))
- Normal stress:  
  \(\sigma_n = \frac{\sigma_x + \sigma_y}{2} + \frac{\sigma_x - \sigma_y}{2} \cos 2\theta\)
- Shear stress:  
  \(\tau = -\frac{\sigma_x - \sigma_y}{2} \sin 2\theta\)

### 4. General 2D Stress (\(\sigma_x, \sigma_y, \tau_{xy}\))
- Normal stress:  
  \(\sigma_n = \frac{\sigma_x + \sigma_y}{2} + \frac{\sigma_x - \sigma_y}{2} \cos 2\theta + \tau_{xy} \sin 2\theta\)
- Shear stress:  
  \(\tau = -\frac{\sigma_x - \sigma_y}{2} \sin 2\theta + \tau_{xy} \cos 2\theta\)

### 5. Principal Stresses & Planes
- Principal planes: shear stress = 0.  
  \(\tan 2\theta_p = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}\)
- Principal stresses:  
  \(\sigma_{1,2} = \frac{\sigma_x + \sigma_y}{2} \pm \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\)

### 6. Max Shear Stress
- \(\tau_{\text{max}} = \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\)

---

## 📘 Principal Stresses and Principal Planes
[📺 Video Link](https://youtube.com/playlist?list=PL4fDZvq5vt6gWFyofRduga32tICcRoBBO&si=6KQ9f2EOvzJFS9U2)

### 1. Concept
- Principal planes: shear stress = 0.
- Principal stresses: normal stresses on these planes.

### 2. Mathematical Derivation
- Orientation:  
  \(\tan 2\theta_p = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}\)
- Principal stresses:  
  \(\sigma_{1,2} = \frac{\sigma_x + \sigma_y}{2} \pm \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\)

### 3. Special Cases
- Pure uniaxial stress: \(\sigma_1 = \sigma_x\), \(\sigma_2 = 0\).
- Pure shear: \(\sigma_1 = +\tau_{xy}\), \(\sigma_2 = -\tau_{xy}\).
- Equal biaxial stress: \(\sigma_1 = \sigma_2 = \sigma_x\).

### 4. Max Shear Stress
- \(\tau_{\text{max}} = \frac{\sigma_1 - \sigma_2}{2}\)

### 🔢 Numerical Example
**Q:** \(\sigma_x = 80\) MPa, \(\sigma_y = 20\) MPa, \(\tau_{xy} = 30\) MPa.  
- \(\tan 2\theta_p = \frac{2 \times 30}{80 - 20} = 1 \Rightarrow \theta_p = 22.5°\)  
- \(\sigma_{1,2} = 50 \pm \sqrt{30^2 + 30^2} = 50 \pm 42.43\)  
- \(\sigma_1 = 92.43\) MPa, \(\sigma_2 = 7.57\) MPa

---

## 📘 Mohr’s Circle of Stress
[📺 Video Link](https://youtu.be/RZbLtfvnWgI?si=Li4XQU-mJJGRWkTG)

### 1. Introduction
- Graphical method to find stresses on inclined planes.

### 2. Construction Steps
1. Plot points: \(A(\sigma_x, \tau_{xy})\), \(B(\sigma_y, -\tau_{xy})\).
2. Join AB; midpoint is center \(C = \frac{\sigma_x + \sigma_y}{2}\).
3. Radius \(R = \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\).
4. Draw circle with center C and radius R.

### 3. Results from Mohr’s Circle
- Principal stresses: \(\sigma_{1,2} = C \pm R\).
- Max shear stress: \(\tau_{\text{max}} = R\).
- Principal plane angle: \(\tan 2\theta_p = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}\).

### 🔢 Example
**Given:** \(\sigma_x = 60\) MPa, \(\sigma_y = 20\) MPa, \(\tau_{xy} = 40\) MPa.  
- Center \(C = \frac{60 + 20}{2} = 40\) MPa  
- Radius \(R = \sqrt{(20)^2 + 40^2} = 44.72\) MPa  
- Principal stresses: \(\sigma_1 = 84.72\) MPa, \(\sigma_2 = -4.72\) MPa  
- Max shear stress: \(\tau_{\text{max}} = 44.72\) MPa

---

## 🎯 Summary
- **Rigid Body**: Idealization for simplified calculations.
- **Stress Types**: Tensile, compressive, shear.
- **Elastic Constants**: Define material behavior under load.
- **Plasticity**: Permanent deformation beyond elastic limit.
- **Deformation**: Depends on load, geometry, and material properties.
- **Thermal Stress**: Develops when expansion/contraction is restricted.
- **Inclined Planes**: Stresses vary with angle.
- **Principal Stresses**: Max/min normal stresses on shear-free planes.
- **Mohr’s Circle**: Graphical tool for stress analysis.

---

For visual explanations, watch the linked YouTube videos!  
**📚 Happy Learning!**
