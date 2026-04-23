# 🌪️ Cyclone Satellite Image Analysis System

This project analyzes satellite images of cyclones using classical computer vision and image processing techniques. It extracts texture, edge, and structural features to estimate cyclone intensity and provide an interpretable scientific analysis.

---

## 📌 Project Overview

Cyclones exhibit strong visual patterns in satellite imagery such as:
- Spiral cloud structures
- High texture variation
- Strong boundary edges

This system uses multiple image processing techniques to analyze these patterns and estimate cyclone severity.

---

## 🧠 Methods Used

The system is based on well-known image processing and remote sensing techniques:

### 1. Texture Analysis (GLCM)
- Measures image texture patterns
- Extracts:
  - Contrast
  - Energy
  - Homogeneity

### 2. Edge Detection (Sobel Filter)
- Detects cyclone boundaries
- Highlights structural shape and spiral formations

### 3. Laplacian Filter
- Captures intensity changes
- Represents energy distribution in cyclone regions

### 4. Structural Analysis
- Estimates cyclone center based on pixel intensity distribution

---

## ⚡ Cyclone Severity Score

A weighted fusion model combines multiple features:

- Texture complexity
- Edge strength
- Intensity variation

This generates a **Cyclone Severity Score (0–100)**:

| Score Range | Interpretation |
|-------------|----------------|
| 0–40        | 🌤️ Weak disturbance |
| 40–70       | 🌪️ Moderate cyclone |
| 70–100      | 🌪️ Severe cyclone |

---

## 📊 Output Features

The system provides:

- Cyclone severity score
- Feature analysis (GLCM + filters)
- Cyclone center estimation
- Visual plots of:
  - Original image
  - Edge map
  - Laplacian energy map
  - Intensity histogram


