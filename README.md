# IIT-PKD-INTERNSHIP

This repository contains internship projects undertaken at **IIT Palakkad**. Currently, the repository includes two independent projects. Below is a detailed description.

---

## 📁 Project 1: Commercial GaN/HEMT Die Characterization

### 🔬 Overview

This project involves the characterization of a **commercial GaN/HEMT die**, the **CGHV60040D**, focusing on physical measurement, fixture design, and DC electrical probing.

---

### 📐 1. Die Dimension Collection

The initial step was to collect the die's physical dimensions (cross sectional dimensions) using available documentation. A PowerPoint file summarizing the dimensions is included. The PowerPoint file also includes the reference for each dimensions.

📎 **[Die Dimensions PPT](Project-1-GaN-HEMT-Die/Die-Dimensions.pptx)**

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

### 📂 Folder Structure for Project 1

