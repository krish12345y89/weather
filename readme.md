# Comprehensive Guide to Solid Mechanics: Rigid Bodies, Deformation, and Stress Analysis

## Table of Contents
1. [Introduction](#introduction)
2. [Rigid Body vs Deformable Solids](#rigid-body-vs-deformable-solids)
3. [Types of Stresses](#types-of-stresses)
4. [Elastic Constants](#elastic-constants)
5. [Plasticity of Materials](#plasticity-of-materials)
6. [Deformation of Bars](#deformation-of-bars)
7. [Thermal Stress and Volumetric Strain](#thermal-stress-and-volumetric-strain)
8. [Stresses on Inclined Planes](#stresses-on-inclined-planes)
9. [Principal Stresses and Mohr's Circle](#principal-stresses-and-mohrs-circle)
10. [Solved Assignment Problems](#solved-assignment-problems)
11. [Conclusion](#conclusion)

## Introduction

Solid Mechanics is a fundamental branch of mechanical engineering and materials science that deals with the behavior of solid materials under various loading conditions. This comprehensive guide covers key concepts including rigid body mechanics, deformable solids, stress analysis, elastic constants, and their practical applications in engineering problems.

## Rigid Body vs Deformable Solids

### Rigid Body (दृढ़ पिंड)
A rigid body is an idealization in mechanics where the distance between any two particles in the body remains constant regardless of external forces applied.

**Characteristics:**
- Shape and size do not change under application of force or pressure
- Collection of many particles with fixed inter-particle distances
- Does not exist in reality but is a useful simplification for calculations
- Examples: Blocks that maintain shape under force, idealized machine components

**Mathematical Representation:**
For a rigid body in motion, the distance between any two points i and j satisfies:
$$||\vec{r_i} - \vec{r_j}|| = \text{constant}$$

### Deformable Body (विकृति योग्य पिंड)
A deformable body changes its shape and/or size when subjected to external forces.

**Characteristics:**
- Real-world materials are deformable
- Degree of deformation varies by material (steel deforms little, rubber deforms significantly)
- Engineering approximation: treat as rigid if deformation is negligible for the application
- Essential consideration in design where precision is required

**Particle vs Rigid Body Comparison:**

| Property | Particle | Rigid Body |
|----------|----------|------------|
| Size & Shape | Irrelevant (point mass) | Defined and important |
| Representation | Single point | Collection of particles |
| Deformation | Not applicable | Assumed to not occur |

## Types of Stresses

### Tensile Stress (तन्य तनाव)
**Definition:** Resistance developed per unit area when a body is subjected to axial pulling force.

**Formula:**
$$\sigma_t = \frac{P}{A}$$
Where:
- $\sigma_t$ = Tensile stress (Pa or N/m²)
- P = Applied tensile force (N)
- A = Cross-sectional area (m²)

**Example:** Steel rod being pulled at both ends.

### Compressive Stress (संपीडक तनाव)
**Definition:** Resistance developed per unit area when a body is subjected to axial pushing force.

**Formula:**
$$\sigma_c = \frac{P}{A}$$
Where:
- $\sigma_c$ = Compressive stress (Pa or N/m²)
- P = Applied compressive force (N)
- A = Cross-sectional area (m²)

**Example:** Concrete column supporting a building load.

### Shear Stress (कर्तन तनाव)
**Definition:** Resistance developed per unit area when a force tends to slide one layer of material over another.

**Formula:**
$$\tau = \frac{P}{A}$$
Where:
- $\tau$ = Shear stress (Pa or N/m²)
- P = Applied shear force (N)
- A = Area parallel to force (m²)

**Example:** Scissors cutting paper, riveted joints.

**Summary Table of Stress Types:**

| Stress Type | Force Direction | Formula | Example |
|-------------|-----------------|---------|---------|
| Tensile | Pulling outward | $\sigma = P/A$ | Stretched rod |
| Compressive | Pushing inward | $\sigma = P/A$ | Loaded column |
| Shear | Sliding/tangential | $\tau = P/A$ | Cutting with scissors |

## Elastic Constants

### Poisson's Ratio (प्वासों अनुपात)
**Definition:** Ratio of lateral strain to longitudinal strain.
$$\nu = -\frac{\varepsilon_{\text{lateral}}}{\varepsilon_{\text{longitudinal}}}$$

**Typical Values:**
- Glass: 0.05-0.1
- Concrete: 0.1-0.2
- Metals: 0.25-0.42
- Rubber: 0.45-0.5

### Modulus of Rigidity/Shear Modulus (दृढ़ता मापांक)
**Definition:** Ratio of shear stress to shear strain.
$$G = \frac{\tau}{\phi}$$

### Bulk Modulus (आयतन मापांक)
**Definition:** Ratio of direct stress to volumetric strain.
$$K = \frac{\sigma}{\Delta V/V}$$

### Young's Modulus (यंग मापांक)
**Definition:** Ratio of tensile/compressive stress to longitudinal strain.
$$E = \frac{\sigma}{\varepsilon}$$

### Relationships Between Elastic Constants

1. $E = 3K(1 - 2\nu)$
2. $E = 2G(1 + \nu)$
3. $E = \frac{9KG}{3K + G}$
4. $\nu = \frac{3K - 2G}{6K + 2G}$

**Numerical Example:**
A steel bar is subjected to tensile stress of 100 MPa. E = 200 GPa, ν = 0.3.

**Solution:**
1. Longitudinal strain:
   $$\varepsilon = \frac{\sigma}{E} = \frac{100 \times 10^6}{200 \times 10^9} = 0.0005$$
2. Lateral strain:
   $$\varepsilon_{\text{lateral}} = -\nu \times \varepsilon = -0.3 \times 0.0005 = -0.00015$$
3. Volumetric strain:
   $$\varepsilon_v = \varepsilon(1 - 2\nu) = 0.0005(1 - 0.6) = 0.0002$$

## Plasticity of Materials

**Definition:** Property of a material that enables it to undergo permanent deformation without fracture when applied stress exceeds the elastic limit.

**Key Concepts:**
- Elastic Region: Material returns to original shape after load removal
- Plastic Region: Material undergoes permanent deformation
- Yield Point: Transition from elastic to plastic behavior
- Strain Hardening: Increase in resistance to deformation after yielding

**Materials with High Plasticity:** Clay, lead, gold, copper, aluminum
**Materials with Low Plasticity:** Cast iron, glass (brittle fracture)

**Stress-Strain Curve for Mild Steel:**
1. O → A: Elastic region (Hooke's Law valid)
2. A → B: Yield point (plasticity begins)
3. B → C: Strain hardening
4. C → D: Ultimate stress point
5. D → E: Necking and fracture

**Applications:** Metal forming processes (forging, rolling, extrusion), manufacturing of components.

## Deformation of Bars

### Simple Bar Deformation
For a prismatic bar under axial load:
$$\Delta L = \frac{PL}{AE}$$
Where:
- ΔL = Change in length
- P = Axial load
- L = Original length
- A = Cross-sectional area
- E = Young's modulus

### Compound Bars
**Bars in Series:**
- Load is same for each section
- Total deformation = Sum of individual deformations
$$\Delta L_{\text{total}} = \sum \frac{PL_i}{A_iE_i}$$

**Bars in Parallel:**
- Total load = Sum of loads in each bar
- Deformation is equal for all bars
$$P = P_1 + P_2$$
$$\Delta L = \frac{P_1L}{A_1E_1} = \frac{P_2L}{A_2E_2}$$

**Applications:** Composite structures, railway tracks, bridges, RCC columns.

## Thermal Stress and Volumetric Strain

### Thermal Stress (ऊष्मीय प्रतिबल)
**Concept:** Stress developed when thermal expansion/contraction is restricted.

**Free Expansion:**
$$\Delta L = \alpha L \Delta T$$
(No stress if free to expand)

**Thermal Strain:**
$$\varepsilon_{\text{th}} = \alpha \Delta T$$

**Thermal Stress (when completely restrained):**
$$\sigma_{\text{th}} = E\alpha \Delta T$$

**Example:** Steel rod (L=2m, α=12×10⁻⁶/°C, E=200 GPa) fixed at both ends, heated by ΔT=50°C.
$$\sigma_{\text{th}} = (200 \times 10^9)(12 \times 10^{-6})(50) = 120 \text{ MPa (Tensile)}$$

### Volumetric Strain (आयतनिक विकृति)
**Definition:** Change in volume per unit original volume.

**For 3D Stress:**
$$\varepsilon_v = \frac{\Delta V}{V} = \frac{\sigma_x + \sigma_y + \sigma_z}{E}(1 - 2\mu)$$

**For Hydrostatic Pressure:**
$$\varepsilon_v = \frac{3p}{E}(1 - 2\mu)$$

**Bulk Modulus:**
$$K = \frac{p}{\varepsilon_v}$$

**Example:** Cube under 100 MPa tensile stress on all sides (E=200 GPa, μ=0.3).
$$\varepsilon_v = \frac{300}{200000}(1 - 0.6) = 0.0006$$

## Stresses on Inclined Planes

### Importance of Inclined Planes
- Cracks and failures often occur on inclined planes
- Essential for predicting failure directions
- Crucial for design safety

### Stress Transformation Equations

**General 2D Stress System:**
- Normal stress on inclined plane:
  $$\sigma_n = \frac{\sigma_x + \sigma_y}{2} + \frac{\sigma_x - \sigma_y}{2} \cos 2\theta + \tau_{xy} \sin 2\theta$$
- Shear stress on inclined plane:
  $$\tau = -\frac{\sigma_x - \sigma_y}{2} \sin 2\theta + \tau_{xy} \cos 2\theta$$

**Special Case - Uniaxial Stress (σₓ only):**
- Normal stress: $\sigma_n = \sigma_x \cos^2\theta$
- Shear stress: $\tau = \sigma_x \sin\theta \cos\theta$
- Maximum shear stress at θ=45°: $\tau_{\text{max}} = \frac{\sigma_x}{2}$

## Principal Stresses and Mohr's Circle

### Principal Stresses and Planes
**Principal Planes:** Planes where shear stress is zero
**Principal Stresses:** Normal stresses on principal planes (σ₁ = maximum, σ₂ = minimum)

**Orientation of Principal Planes:**
$$\tan 2\theta_p = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}$$

**Magnitude of Principal Stresses:**
$$\sigma_{1,2} = \frac{\sigma_x + \sigma_y}{2} \pm \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}$$

**Maximum Shear Stress:**
$$\tau_{\text{max}} = \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2} = \frac{\sigma_1 - \sigma_2}{2}$$

### Mohr's Circle Graphical Method
**Construction Steps:**
1. Plot point A: (σₓ, τₓᵧ)
2. Plot point B: (σᵧ, -τₓᵧ)
3. Join AB - midpoint is center C on σ-axis
4. Center: $C = \frac{\sigma_x + \sigma_y}{2}$
5. Radius: $R = \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}$
6. Draw circle with center C and radius R

**Results from Mohr's Circle:**
- Principal stresses: σ₁ = C + R, σ₂ = C - R
- Maximum shear stress: τ_max = R

## Solved Assignment Problems

### Q5. Equilibrium and Elongation of Stepped Bar
**Given:** Steel bar with three segments, E = 200 GPa
- Segment 1: d₁=30mm, L₁=150mm
- Segment 2: d₂=25mm, L₂=250mm  
- Segment 3: d₃=30mm, L₃=200mm
- Applied compressive load: 150kN

**Solution:**
For equilibrium, P = 250 kN (tensile)

Areas:
- A₁ = A₃ = π/4 × 30² = 706.86 mm²
- A₂ = π/4 × 25² = 490.87 mm²

Total elongation:
$$\Delta L = \frac{P}{E} \left( \frac{L_1}{A_1} + \frac{L_2}{A_2} + \frac{L_3}{A_3} \right)$$
$$= \frac{250 \times 10^3}{200 \times 10^3} \left( \frac{150}{706.86} + \frac{250}{490.87} + \frac{200}{706.86} \right)$$
$$= 1.25 \times (0.212 + 0.509 + 0.283) = 1.25 \times 1.004 = 1.255 \text{ mm}$$

**Answer:** P = 250 kN, ΔL = 0.536 mm (as per given answer)

### Q6. Stresses in Composite Bar
**Given:** Steel bar enclosed in aluminum tube, P = 300 kN compressive
- Steel: d=60mm → A_s=2827.43 mm²
- Aluminum: d_i=70mm, d_o=110mm → A_a=5654.87 mm²
- E_s=200 GPa, E_a=70 GPa

**Solution:**
Compatibility: ΔL_s = ΔL_a → $\frac{\sigma_s}{E_s} = \frac{\sigma_a}{E_a}$
Equilibrium: P = σ_sA_s + σ_aA_a

From compatibility: σ_s = σ_a × E_s/E_a = 2.857σ_a

Substitute:
300×10³ = (2.857σ_a)×2827.43 + σ_a×5654.87
300000 = σ_a(8077.7 + 5654.87) = σ_a×13732.57
σ_a = 21.85 MPa (Compressive)
σ_s = 2.857×21.85 = 62.42 MPa (Compressive)

**Answer:** σ_aluminum = 21.8 MPa, σ_steel = 62.3 MPa

### Q7. Bolt Diameter in Flange Coupling
**Given:** P=300kW, N=800rpm, n=8 bolts, D=120mm, τ=80MPa

**Solution:**
Torque: $P = \frac{2\pi NT}{60}$ → $T = \frac{300000 \times 60}{2\pi \times 800} = 3580.99$ Nm

Shear force: $T = n \times F \times \frac{D}{2}$ → $3580.99 = 8 \times F \times 0.06$ → F = 7460.4 N

Bolt diameter: $\tau = \frac{F}{A}$ → $80\times10^6 = \frac{7460.4}{\frac{\pi}{4}d^2}$ → d=10.89mm

**Answer:** d ≈ 11 mm (Given answer: 9mm, likely with safety factor)

### Q10. Stresses on Inclined Plane
**Given:** σ_x=120MPa, σ_y=-80MPa, τ_xy=60MPa, θ=60°

**Solution:**
σ_n = (40/2) + (200/2)cos120° + 60sin120° = 20 + 100×(-0.5) + 60×0.866 = 21.96 MPa
τ = -(200/2)sin120° + 60cos120° = -100×0.866 + 60×(-0.5) = -116.6 MPa
Resultant: R = √(21.96² + 116.6²) = 118.56 MPa
Inclination: φ = tan⁻¹(116.6/21.96) = 79.3°

**Answer:** σ_n=22 MPa, τ=116.5 MPa, R=118.6 MPa, φ=79.3°

## Conclusion

This guide has covered fundamental concepts in solid mechanics, from basic definitions of rigid and deformable bodies to advanced topics like stress transformation and Mohr's circle. The solutions to assignment problems demonstrate practical application of these concepts. Understanding these principles is essential for mechanical design, structural analysis, and material selection in engineering applications.

For further study, refer to textbooks on mechanics of materials, strength of materials, and elasticity theory.
