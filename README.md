# Static Structural Analysis of 1D Stepped Beam 🏗️



## 📌 Project Overview
This project performs a Finite Element Analysis (FEA) on a **1D stepped beam** using **Ansys Mechanical 2025 R2**. The simulation models a structural component with varying circular cross-sections under a high axial tensile load to evaluate structural integrity, deformation, and axial stress distribution.

## ⚙️ Simulation Specifications

### 1. Geometry & Mesh
* **Element Type:** 1D Line Body (Beam Elements).
* [cite_start]**Cross Sections:** Three varying circular sections (Stepped Geometry)[cite: 63].
    * [cite_start]*Radii:* 20mm, 15mm, and 10mm[cite: 93].
* [cite_start]**Mesh Statistics:** 22 Elements, 45 Nodes[cite: 57].

### 2. Material Properties: Structural Steel
The beam is modeled using standard Structural Steel with the following properties:
| Property | Value | Unit |
| :--- | :--- | :--- |
| **Young's Modulus** | 200 | [cite_start]GPa [cite: 287] |
| **Poisson's Ratio** | 0.3 | [cite_start]- [cite: 287] |
| **Yield Strength** | 250 | [cite_start]MPa [cite: 285] |
| **Ultimate Strength** | 460 | [cite_start]MPa [cite: 285] |

### 3. Boundary Conditions & Loads
* [cite_start]**Support:** Fixed Support applied at the vertex (constrained in all DOFs)[cite: 139].
* [cite_start]**Loading:** Axial Force of **100,000 N (100 kN)** applied in the X-direction.

## 📊 Results & Analysis

### 🔍 Key Findings
The simulation successfully converged with the following results:

1.  **Total Deformation:**
    * [cite_start]**Maximum Deflection:** 0.0363 mm (3.6298e-5 m) occurring at the free end[cite: 194].
    * The deformation gradient is linear relative to the stiffness of the stepped sections.
2.  **Direct Stress:**
    * [cite_start]**Average Stress:** 79.6 MPa (7.9639e7 Pa)[cite: 264].
    * **Safety Factor:** The maximum stress (79.6 MPa) is significantly lower than the Yield Strength (250 MPa), indicating the design is safe under the applied load.

### 📸 Visualizations
**Total Deformation Contour:**
*(Figure 1: Axial deformation showing maximum displacement at the loaded end)*

## 📂 File Structure
* `Model.wbpj`: The Ansys Workbench project file.
* `Report.pdf`: Detailed simulation report.
* `StaticFigure41.png`: Result visualization.

## 🚀 How to Run
1.  Open **Ansys Workbench 2025 R2** (or compatible version).
2.  Go to `File > Open` and select the `.wbpj` file from this repository.
3.  Right-click on **Model** and select **Update** to refresh the mesh.
4.  Right-click on **Solution** and select **Solve**.

---
## 👨‍💻 Author
**Yazan Alzyuod**
* **Mechanical Engineer** specializing in Robotics, UGV Design, and FEA.
* 📧 [yqlasem@gmail.com](mailto:yqlasem@gmail.com)
* 🔗 [LinkedIn Profile](https://www.linkedin.com/in/yazan-alzyuod)
* 💻 [GitHub Profile](https://github.com/Yazan-Alzyuod)
