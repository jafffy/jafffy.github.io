---
layout: project
title: "Automated Liver Fibrosis Classification"
subtitle: "Semi-automated CT image analysis for hepatic fibrosis"
date: 2021-01-01
period: "2019 - 2021"
status: "completed"
technologies: ["Python", "Medical Imaging", "Computer Vision", "CT Analysis", "PCA"]
links:
  - title: "Abdominal Radiology Paper"
    url: "https://link.springer.com/article/10.1007/s00261-020-02884-x"
---

## Project Overview

Developed a semi-automated algorithm for liver fibrosis classification from CT images, significantly reducing manual annotation workload while improving diagnostic accuracy.

## Publication

**"Combining hepatic surface nodularity and serum tests better predicts hepatic fibrosis stages in chronic liver disease"**  
*Abdominal Radiology* (2021) - Co-first author

## Key Innovation

### Semi-Automated ROI Selection

- Reduced manual annotation from every slice to single-click initialization
- Automated tracking of liver boundaries across CT slices
- Maintained high accuracy while drastically reducing physician workload

### Technical Approach

1. **Laplacian of Gaussian (LoG) Filter**
   - Edge extraction for liver surface detection
   - Robust to noise in CT images
   
2. **Principal Component Analysis (PCA)**
   - Surface orientation determination
   - Consistent measurement across patients
   
3. **Quantitative Surface Analysis**
   - Automated nodularity quantification
   - Reproducible measurements for clinical use

## Clinical Impact

- **Improved Reproducibility:** Reduced inter-observer variability
- **Time Efficiency:** 90% reduction in annotation time
- **Better Staging:** Combined with serum markers for accurate fibrosis staging
- **Patent Filed:** Korean Patent No. 10-2009233

## Research Outcomes

- Validated on large clinical dataset
- Demonstrated superior performance to manual methods
- Integrated into clinical workflow considerations
- Foundation for fully automated systems

## Skills Demonstrated

- Medical image processing
- Algorithm development for clinical applications
- Statistical analysis and validation
- Cross-disciplinary collaboration with radiologists
- Patent application and protection