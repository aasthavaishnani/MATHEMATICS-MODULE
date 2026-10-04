# Calculative Foundation: Linear Algebra in Student Performance Analytics

## 🎯 Project Overview
This repository contains a comprehensive practical and theoretical implementation of **Linear Algebra concepts** applied to student performance analytics. The project demonstrates the execution of vector operations, matrix transformations, geometric interpretations, and spectral decomposition (Eigenvalues & Eigenvectors) using Python.

---

## 📑 Problem Statement
A research institute dataset containing student performance scores across multiple subjects was analyzed to:
1. Represent and manipulate data points as multidimensional vectors.
2. Perform core matrix operations (multiplication, transpose, determinant, and inverse).
3. Geometric conceptualization of data dimensions (Lines, Planes, and Hyperplanes).
4. Extract principal components via Covariance Matrix decomposition (Eigenvalues & Eigenvectors).

---

## 🛠️ Project Structure & Tasks

### Part A: Vector Fundamentals
- **Vector Representation**: Individual student scores mapped as 1D feature vectors.
- **Norms**: Computed Norm-1 ($L_1$) and Norm-2 ($L_2$) magnitudes.
- **Dot Product & Angle**: Evaluated similarity and direction alignment ($\theta$) between student vectors.
- **Cross Product & Projection**: Evaluated 3D spatial orthogonality ($\mathbf{a} \times \mathbf{b}$) and orthogonal vector projection ($\text{proj}_{\mathbf{b}}\mathbf{a}$).

### Part B: Matrix Operations
- Formed a $5 \times 4$ (Students $\times$ Subjects) matrix.
- Evaluated Matrix Addition, Transpose ($\mathbf{M}^T$), and Gram Matrix Multiplication ($\mathbf{M} \mathbf{M}^T$).
- Calculated Determinant ($\det(\mathbf{A})$) and Matrix Inverse ($\mathbf{A}^{-1}$) on square sub-matrices.

### Part C: Linear Transformations & Geometry
- Mapped score relationships across 2D (Lines), 3D (Planes), and 4D+ (Hyperplanes).
- Visualized multidimensional feature distribution using Matplotlib.

### Part D: Eigenvalues & Decomposition
- Constructed the $4 \times 4$ Subject Covariance Matrix.
- Extracted Eigenvalues ($\lambda$) and Eigenvectors ($\mathbf{v}$).
- Analyzed explained variance ratio for dimensionality reduction (PCA foundation).

---

## 💻 Tech Stack & Dependencies
- **Language**: Python 3.x
- **Libraries**: `numpy`, `pandas`, `matplotlib`

---

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone <your-github-repo-url>

---

#### 📄 **Deliverable 2: Summary of Theory Concepts for PDF Submission (Basic English)**

Tame aa section ni PDF banavi shako chhe (Word/Google Docs ma copy-paste karine PDF export karo):

1. **Vector Norms:**
   - **Norm-1 ($L_1$):** $\Vert{}\mathbf{v}\Vert{}_1 = \sum \vert{}v_i\vert{}$. Measures total score sum across attributes.
   - **Norm-2 ($L_2$):** $\Vert{}\mathbf{v}\Vert{}_2 = \sqrt{\sum v_i^2}$. Measures Euclidean distance from the origin.
2. **Dot Product & Similarity:**
   - $\mathbf{a} \cdot \mathbf{b} = \sum a_i b_i = \Vert{}\mathbf{a}\Vert{}_2 \Vert{}\mathbf{b}\Vert{}_2 \cos(\theta)$. Quantifies score directional similarity.
3. **Matrix Inverse & Singular Matrix:**
   - Inverse $\mathbf{A}^{-1}$ exists if and only if $\det(\mathbf{A}) \neq 0$.
4. **Hyperplanes & Dimensions:**
   - Boundary equation in $n$-dimensional space: $\mathbf{w}^T \mathbf{x} + b = 0$.
5. **Eigenvalues & Eigenvectors:**
   - $\mathbf{\Sigma} \mathbf{v} = \lambda \mathbf{v}$. Eigenvectors denote principal directions of maximum dataset variance; Eigenvalues represent the variance magnitude.

---

### 📋 **Final Checklist for Submission:**
- [x] All 4 Parts (Part A, B, C, D) executed in Python.
- [x] Interpretations written under code cells in Jupyter Notebook.
- [x] Push `.ipynb` notebook to GitHub Repository.
- [x] Add the structured `README.md` to GitHub.
- [x] Export Theory PDF document and upload to GitHub / Exam portal.

---

