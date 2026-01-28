# item-greenwashing-detection: A Multimodal Data Integration Framework for Detecting Greenwashing

## Project Overview
This project establishes a research framework to detect **"Greenwashing"** in household cleaning products. By integrating front-facing retail data with back-end chemical safety data (SDS) and regulatory records (EPA), this pipeline quantifies the "gap" between a product's marketing claims and its actual environmental and chemical reality.

## The Data Integration Framework
The project utilizes a **Tri-Layer Data Model** to cross-reference products:

1.  **The Marketing Layer (Amazon):** Raw consumer-facing data including product titles, bullet points, and visual cues.
2.  **The Chemical Layer (SDS):** Safety Data Sheets providing GHS hazard codes (e.g., H318 for Eye Damage) to establish ground-truth toxicity.
3.  **The Regulatory Layer (EPA):** Safer Choice and DfE databases used to verify if "eco-friendly" claims are backed by federal certification.



## Repository Structure
* `data/raw/`: Contains the three primary source files (`Raw_Amazon_Product_Dataset_1000.csv`, `EPA_RawDataSet.csv`, `sds_raw_extraction-2.csv`).
* `data/processed/`: Stores the final output (`Final_Integrated_Dataset_1000.csv`) after the integration script runs.
* `notebooks/`: Python code for data cleansing, Exploratory Data Analysis (EDA), visualization of the "Greenwashing Gap and Resarch questions methodologies implementation"


## Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/greenwashing-detection.git](https://github.com/yourusername/greenwashing-detection.git)
