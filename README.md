# Aneurysm-Hemodynamics-PIV-Study
Explores the impact of human body movement on aneurysm hemodynamics using Particle Image Velocimetry (PIV). 
## **Overview**  
This project focuses on **transforming real medical imaging data from AneuDesk into 3D-printed aneurysm models**, enabling detailed in-vitro hemodynamic studies. By leveraging **advanced segmentation techniques and CAD modeling**, we extracted aneurysm geometries from medical scans, processed them for smoothness and accuracy, and prepared them for 3D printing.  

These models closely mimic actual vascular structures, allowing researchers to **study blood flow behavior, velocity fields, and wall shear stress (WSS)** under controlled experimental conditions. This work bridges the gap between **patient-specific imaging and experimental research**, ensuring accurate aneurysm modeling for in-vitro analysis.  


## 🔬 **Key Objectives**
- ✅ **Source patient-specific aneurysm geometries** from **AneuDesk medical imaging datasets**.  
- ✅ **Segment and refine aneurysm models** for **CAD-based experimental use**.  
- ✅ **Optimize model accuracy** to match **in-vitro flow conditions**.  
- ✅ **Prepare high-resolution 3D-printable models** for fluid dynamics studies.  


## 🛠 **Tools & Technologies Used**
### **Software**
- **AneuDesk** – Sourcing real aneurysm imaging data.  
- **3D Slicer** – Segmentation of medical imaging data (DICOM) into 3D models.  
- **Meshmixer** – Refining, smoothing, and modifying aneurysm geometries.  
- **SolidWorks** – CAD modeling of patient-specific aneurysm structures.  
- **MATLAB** – Geometric validation and model optimization.  

### **Hardware**
- **Resin-Based 3D Printer** – High-resolution printing of vascular models.  

### **Techniques**
- **Medical Image Processing** – Extracting aneurysm structures from CT/MRI data.  
- **CAD Modeling & Refinement** – Ensuring **smooth, experimentally viable** models.  
- **Biomechanics & Flow Optimization** – Structuring models for **fluid analysis**.  


## 🔬 **Methodology**
### **1️⃣ Sourcing & Processing Medical Imaging Data**
- **Raw Data Source:** Obtained **patient-specific aneurysm datasets** from **AneuDesk**.  
- **Image Segmentation (3D Slicer):**  
  - Imported **DICOM files** (CT/MRI scans) into **3D Slicer**.  
  - Applied **threshold-based segmentation** to extract aneurysm geometry.  
  - Used **region-growing algorithms** to differentiate aneurysmal sac from surrounding vasculature.  
  - Converted segmented **vascular structures into 3D meshes** for CAD processing.  

### **2️⃣ Refining & Preparing 3D CAD Models**
- **Mesh Processing in Meshmixer:**  
  - **Removed artifacts and unnecessary vascular branches** to focus on the aneurysm sac.  
  - **Smoothed surfaces** to eliminate irregularities affecting flow dynamics.  
  - Adjusted **inlet and outlet diameters** to match experimental flow loop requirements.  

- **Final CAD Modifications in SolidWorks:**  
  - Optimized **stem diameter and aneurysm sac volume** for experimental testing.  
  - Ensured **wall thickness consistency** for accurate hemodynamic studies.  
  - Added **support structures** for stable 3D printing.  

### **3️⃣ 3D Printing & Model Validation**
- **Material Selection:**  
  - Printed **aneurysm models using high-resolution resin-based 3D printing**.  
  - Ensured **vascular smoothness and structural integrity**.  

- **Printing Process:**  
  - Used **resin-based SLA 3D printing** to capture intricate vascular details.  
  - Conducted **post-processing to remove residual resin and enhance accuracy**.  

- **Geometric Validation (MATLAB):**  
  - Measured **diameters, wall thickness, and curvature consistency**.  
  - Compared **segmented 3D models with original medical scan data** to ensure accuracy.  


## 📊 **Key Findings & Takeaways**
- ✅ **Accurately converted raw CT/MRI aneurysm data into high-resolution 3D models**.  
- ✅ **Optimized models for in-vitro hemodynamic studies** using CAD refinements.  
- ✅ **Validated model integrity** through MATLAB-based geometric analysis.  
- ✅ **Created a reproducible process** for future patient-specific aneurysm modeling.  
