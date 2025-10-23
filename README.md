# Chromatography Data Analysis Workflow

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/brown-ccv/deeps-chromatography/blob/main/agilent_chromatogram_data_parsing_colab.ipynb)

This repository contains a workflow for parsing and analyzing LC-MS chromatography data from Agilent .D files using the rainbow-api library. The workflow demonstrates parallel data processing, visualization, and export capabilities.

## 📁 Main Files

### **Notebooks**
- **`agilent_chromatogram_data_parsing.ipynb`** - Local version for desktop Jupyter environments
- **`agilent_chromatogram_data_parsing_colab.ipynb`** - Google Colab version with repository cloning and cloud setup

### **Sample Data**
- **`sample-data/`** - Directory containing example Agilent .D chromatography files for testing and demonstration

## 🚀 Quick Start

### Option 1: Google Colab (Recommended)
Click the **"Open in Colab"** badge above to run the workflow in your browser with no setup required.

### Option 2: Local Installation
1. Clone this repository
2. Install dependencies, preferably in a separate environment: `pip install .`
3. Open `agilent_chromatogram_data_parsing.ipynb` in Jupyter

## 🔬 Workflow Features

- **Parallel Processing**: Efficient batch reading of multiple .D files
- **Data Inspection**: Complete analysis of MSD2.MS data structure and metadata
- **Visualizations**: Single trace and multi-trace chromatogram plots
- **Export Capabilities**: CSV export using rainbow-api's native methods

## 📊 Data Structure

Each .D folder contains chromatography data with:
- **Time points**: Retention times in minutes (xlabels)
- **m/z traces**: Mass-to-charge ratios monitored (ylabels)
- **Intensity matrix**: Raw detector responses (data)

## 🛠️ Dependencies

- `rainbow-api`: For reading Agilent .D files