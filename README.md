# HW5_2210357124_idilsevis
Visual comparison of linear and non-linear SVMs (RBF, Poly, Sigmoid) on a concentric circle dataset. Includes 2D/3D visualizations, support vector analysis, and kernel evaluation. 

# SVM Kernel Comparison on Non-Linearly Separable Data

This repository contains the implementation for an extra credit homework assignment from the ELE 489: Fundamentals of Machine Learning course at Hacettepe University. The task involves designing, training, and comparing **linear and kernel-based SVM classifiers** using a 2D synthetic dataset shaped as **concentric circles**, which is not linearly separable.

---

##  Objectives

- Generate a synthetic non-linearly separable 2D dataset.
- Fit and evaluate a **Linear SVM**.
- Apply and compare different **non-linear kernels** (RBF, Polynomial, Sigmoid).
- Visualize decision boundaries in **2D** and **3D**.
- Analyze accuracy, margin, and support vectors.

---

## Dataset

- **Type**: Synthetic 2D Toy Dataset
- **Structure**:  
  - **Class 0**: Inner circle  
  - **Class 1**: Outer ring
- **Size**: 200 points (100 per class)


---

## Kernels Evaluated

| Kernel      | Accuracy | Support Vectors |
|-------------|----------|-----------------|
| Linear      | 71.0%    | 184             |
| RBF         | 100.0%   | 25              |
| Polynomial  | 68.5%    | 187             |
| Sigmoid     | 50.5%    | 124             |

---

##  Visualizations

- **Figure 1**: Input dataset with concentric circles  
- **Figure 2**: Linear SVM decision boundary with margins  
- **Figure 3**: 3D decision surface for RBF kernel  
- **Figure 4**: 2D decision boundary for RBF kernel

---

##Insights

- **Linear SVM** fails due to its inability to model circular decision boundaries.
- **RBF kernel** perfectly separates the two classes with a small number of support vectors.
- **Polynomial** and **sigmoid** kernels perform poorly on this data.

---

## File Structure

├── q1.png # Q1: Dataset plot
├── q2.png # Q2: Linear SVM
├── q3.png # Q3: RBF Kernel 3D surface
├── q4.png # Q4: RBF Kernel 2D boundary
└── svm_implementation.py # Full Python code
