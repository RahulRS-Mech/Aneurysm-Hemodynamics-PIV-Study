# Aneurysm-Hemodynamics-PIV-Study
Explores the impact of human body movement on aneurysm hemodynamics using Particle Image Velocimetry (PIV).

## **Overview**  
This study investigates how **human body movement affects aneurysm hemodynamics**, specifically focusing on **velocity distribution, wall shear stress (WSS), and oscillatory shear index (OSI)** using **Particle Image Velocimetry (PIV).**  

We employ **Prana (PIV tool)** for **velocity field extraction and multi-pass image correlation**, allowing precise analysis of flow structures under **static and dynamic conditions**. Using **high-speed imaging**, we capture fluid motion inside **aneurysm models** under **controlled pulsatile flow** and apply **multi-pass cross-correlation** in Prana to obtain high-accuracy velocity vectors.  

This research enhances our understanding of how **real-world movement alters aneurysm flow patterns**, paving the way for **better risk assessment and medical device designs.**


## 🔬 **Key Objectives**
- ✅ **Use PIV to measure velocity fields** inside patient-specific aneurysm models.  
- ✅ **Apply Prana multi-pass image correlation** to extract accurate flow velocity data.  
- ✅ **Analyze WSS and OSI** to understand how movement affects aneurysm rupture risks.  
- ✅ **Compare static vs. motion conditions** to quantify movement-induced hemodynamic changes.  


## 🛠 **Tools & Technologies Used**
### **Software**
- **Prana code (PIV)** – Multi-pass cross-correlation for velocity field extraction.  
- **MATLAB** – WSS and OSI post-processing, velocity field visualization.  

### **Hardware**
- **High-Speed Camera (100k dcb16 Mega Speed)** – Capturing PIV images at **1000+ fps**.  
- **Harvard Apparatus Pulsatile Blood Pump** – Generating controlled pulsatile flow at **60–80 bpm**.  
- **K40 40W Optical Power Laser** – Creating a laser sheet for precise **PIV measurements**.  

### **Techniques**
- **Particle Image Velocimetry (PIV)** – Velocity field measurements using **tracer particles**.  
- **Multi-Pass Cross-Correlation (Prana)** – Refining velocity vector accuracy.  
- **High-Performance Computing (HPC)** – Processing large datasets efficiently.  


## 🔬 **PIV Study & Prana Processing**
### **1️⃣ High-Speed Image Acquisition**
- **Illumination Setup:** A **K40 40W Optical Power Laser** creates a **thin laser sheet** aligned with the aneurysm model’s flow plane.  
- **Seeding Particles:** **Neutrally buoyant tracer particles** (diameter ~10 µm) suspended in **blood analog fluid** for **flow visualization**.  
- **High-Speed Recording:**  
  - **Frame Rate:** 1000+ fps for capturing **high-resolution flow structures**.  
  - **Exposure Time:** Adjusted for **sharp particle tracking** while minimizing motion blur.  
  - **Frames per Experiment:** ~8000 frames processed per test case.  

### **2️⃣ Image Preprocessing for PIV**
- **Background Removal:**  
  - Captured images processed to remove static noise and reflections.  
  - Enhancing **particle contrast** for better **cross-correlation accuracy**.  
- **Filtering:**  
  - **Gaussian smoothing** applied to reduce high-frequency noise.  
  - **Thresholding and edge detection** improve tracer particle detection.  

### **3️⃣ Velocity Field Extraction (Prana)**
- **Multi-Pass Cross-Correlation Analysis**:  
  - **Pass 1 (128×128 grid):** Coarse estimation of velocity vectors.  
  - **Pass 2 (96×96 grid):** Refined calculation with overlapping interrogation windows.  
  - **Pass 3 (64×64 grid):** High-resolution velocity vector refinement.  
  - **Vector Validation:** Eliminating spurious vectors using **median filtering**.  

- **Velocity Vector Calculation**:  
  - Extract **U (X-direction) and V (Y-direction) velocity components**.  
  - Generate **instantaneous and time-averaged velocity fields**.  

### **4️⃣ WSS & OSI Calculation (MATLAB Post-Processing)**
- **Wall Shear Stress (WSS) Computation:**  
  - WSS calculated from velocity gradients **near aneurysm walls**.  
  - Compared between **static vs. dynamic conditions**.  

- **Oscillatory Shear Index (OSI) Analysis:**  
  - Quantifies flow disturbances caused by motion.  
  - High OSI regions **correlate with potential aneurysm rupture zones**.  

### **5️⃣ Data Visualization**
- **MATLAB plots for velocity profiles:**  
  - Contour plots of **U, V components** at multiple time frames.  
  - **Streamline visualizations** to track flow recirculation patterns.  

- **Comparison of Static vs. Motion Conditions:**  
  - Quantifies differences in **flow acceleration, turbulence, and wall stress**.  
  - Highlights how motion **creates high WSS zones** leading to possible aneurysm rupture risks.  


## 📊 **Key Findings**
- ✅ **Motion increases localized turbulence**, leading to **higher WSS and OSI**.  
- ✅ **Prana's multi-pass correlation method improves velocity vector accuracy**, reducing **false vectors and noise artifacts**.  
- ✅ **Static vs. Dynamic Analysis:** Movement **significantly alters recirculation patterns** in aneurysms.  
- ✅ **PIV provides high-resolution velocity data**, enhancing **in-vitro hemodynamic modeling**.  

