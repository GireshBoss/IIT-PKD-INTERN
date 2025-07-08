# IIT-PKD-INTERNSHIP

This repository contains internship projects undertaken at **IIT Palakkad**. Currently, the repository includes two independent projects. Below is a detailed description.

---

## 📁 Project 1: Commercial GaN/HEMT Die Characterization

### 🔬 Overview

This project involves the characterization of a **commercial GaN/HEMT die**, the **CGHV60040D**, focusing on physical measurement, fixture design, and DC electrical probing.

---

### 📐 1. Die Dimension Collection

The initial step was to collect the die's physical dimensions (cross sectional dimensions) using available documentation. A PowerPoint file summarizing the dimensions is included. The PowerPoint file also includes the reference for each dimensions.

📎 **[Die Dimensions PPT](/Project_1_CGHV60040D/CGHV60040D-Die.pptx)**

---

### 🧰 2. Custom Stainless Steel Carrier Design

The DC Probe Station in the institue, has a vacuum chuck, with a vacuum hole diameter of 2mm. But the DUT (Device Under Test) is 1.8mm x 0.8mm, unabling us to do regular measurements. 
The vacuum chuck was itself necessary, to hold the DUT in place while probing. 
It was necessary that the chuck was electrically grounded, since the source contact of the DUT, was under the die, with gold plating.
Due to handling challenges with the small die on a vacuum chuck, custom **stainless steel carriers** were fabricated. Two versions were designed:

- **250 µm hole diameter**
- **500 µm hole diameter**

📁 Folder: `Project-1-GaN-HEMT-Die/Stainless-Steel-Carrier/`

---

### 📊 3. DC Probing & Measurements

DC measurements were performed after mounting the die on the custom carrier. 
The Output Characteristics (Id-Vd), and the Transfer Characteristics (Id-Vg) were measured.
**It is to be noted that the, DUT was not tested for its full potential, as the maximum measureable drain current was 100mA(0.1A).**
But the device was capable of producing 3.2A of current.
The collected data is available in CSV format.

📄 **[Download DC Measurements CSV](Project-1-GaN-HEMT-Die/DC-Measurements/measurements.csv)**

---

## 📁Project 2: Maury 2640D Slide Screw Tuner Simulation & Modeling

### 📡 Overview

This project involves the **3D electromagnetic simulation** and **machine learning modeling** of the **Maury 2640D slide screw tuner**, a precision impedance tuner used in RF testing environments, and load pull measurements.

The project is divided into three phases:

---

### 📏 1. Physical Measurement

The physical **Maury 2640D tuner** was measured manually using a Vernier Caliper to gather all critical dimensional data. These dimensions were used as input for simulation modeling.

📎 **[Dimensional Data PPT](./Tuner-Dimensions.pptx)**

---

### 🧪 2. HFSS Simulation

Using the collected measurements, the tuner was modeled and simulated in **ANSYS HFSS (Student Version)** to study its electromagnetic behavior.

📁 **HFSS Design File:**
- `Maury_Tuner_Simulation.aedt`

> Note: You need **Ansys HFSS Student Version** or higher to open this file.

---

### 🤖 3. Regression Model for Tuner Probe Prediction

A regression model was developed to **predict the probe position** of the tuner based on:

- Input frequency
- Desired VSWR (Voltage Standing Wave Ratio)

This helps in automating tuner configuration for specific impedance matching tasks.

📁 Files included:
- `tuner_model.ipynb` – Jupyter Notebook with regression model code
- `sample_dataset.csv` – Sample training/testing dataset

---




