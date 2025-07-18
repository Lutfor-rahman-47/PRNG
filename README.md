# 🎲 Custom Pseudorandom Number Generator (PRNG) Analysis

This project demonstrates and compares two pseudorandom number generation approaches — one using a **uniform distribution**, and the other using a **non-uniform (beta)** distribution — to analyze randomness, uniformity, and clustering.

---

## 📌 Objectives

- To simulate and visualize random number generation using:
  - **Uniform Distribution**: `np.random.uniform()`
  - **Beta Distribution**: `np.random.beta(2, 2)`
- To analyze:
  - The **uniformity** of the distribution.
  - The **dependency and clustering** behavior.
- To generate **scatter plots** and **histograms** for visualization.
- To provide basic **statistical summaries** of the generated data.

---

## 🧮 Algorithm Details

### 1️⃣ Uniform Distribution Generator:
- Random values generated in the range **[0, 1)** for both X and Y.
- Method: `np.random.uniform(0, 1, size=n)`

### 2️⃣ Beta Distribution Generator (Non-uniform):
- Uses **Beta(2,2)** to simulate clustering around the center (0.5).
- Method: `np.random.beta(2, 2, size=n)`

---

## 📊 Visualizations

### ✅ Scatter Plots:
- Shows the spread of points for both generators in 2D space.

### ✅ Histograms:
- Displays the frequency distribution of X and Y values separately.

### 📄 PDF Outputs:
- `t1.pdf`: Scatter plot comparison.
- `tt.pdf`: Histograms of each axis for both distributions.

---

## 📈 Statistical Summary

| Metric         | Uniform X | Uniform Y | Beta X | Beta Y |
|----------------|-----------|-----------|--------|--------|
| Mean           | ~0.50     | ~0.50     | ~0.50  | ~0.50  |
| Std Deviation  | ~0.29     | ~0.29     | < 0.29 | < 0.29 |

> 🎯 Beta distribution is more **clustered around the mean**.

---

## 📂 Files in Repository

