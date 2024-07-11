# Spatial Data Processing and Analysis

This repository contains a series of Jupyter Notebooks that detail a comprehensive workflow for spatial data processing, analysis, and modeling. The steps include raster reprojections, dataframe generation, interpolation, and modeling.

## Table of Contents

- [Introduction](#introduction)
- [Abstract](#abstract)
- [Installation](#installation)
- [Usage](#usage)
- [Notebooks](#notebooks)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project is developed in the context of a thesis investigating the potential of integrating Artificial Intelligence (AI) and spatial datasets to predict and analyze poverty in Malawi. It aims to provide precise, actionable insights into poverty dynamics using advanced machine learning models and high-resolution data.

## Abstract

Eradicating extreme poverty remains one of the most pressing global challenges. This study investigates the potential of integrating Artificial Intelligence (AI) and spatial datasets to predict and analyze poverty in Malawi. By using advanced machine learning models and high-resolution data, this research aims to provide precise, actionable insights into poverty dynamics. The study focuses on using infrastructure-related datasets such as nightlights, roads, healthcare facilities, and built-up areas to predict poverty levels accurately.

The methodology starts with data collection from diverse sources, including satellite data and socio-economic surveys. Key datasets include nightlights data reflecting economic activity, road density data indicating accessibility, healthcare facilities data providing health service locations, and built-up areas data distinguishing between urban and rural regions. The Integrated Household Panel Survey (IHPS) offers detailed socio-economic data for model validation. Data preprocessing ensures consistency and accuracy, involving cleaning, standardizing, merging, and reprojecting raster datasets to a common coordinate system. Interpolation techniques align the gap poor percentage data with the spatial datasets.

In the model development phase, a Random Forest Regressor machine learning model is trained to identify patterns influencing poverty. The model's performance is evaluated using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score. Validation is achieved through cross-validation techniques and comparing model predictions against interpolated poverty data.

Results demonstrate a strong predictive capability for poverty levels in Malawi, with high R² values indicating robust model performance (0.825). The correlation analysis reveals significant relationships between various infrastructure datasets and poverty levels, underscoring the relation between infrastructure and socio-economic conditions. The study highlights the scalability of AI-driven models, offering potential for broader application in other regions facing similar challenges and contributes to the broader field of AI for social good, demonstrating practical applications of AI in poverty eradication.

## Installation

To use the notebooks in this repository, you need to have Python and the necessary libraries installed. Follow the steps below to set up your environment.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/spatial-data-processing.git
   cd spatial-data-processing
Create and activate a new conda environment:

bash
Copy code
conda create --name spatial-env python=3.11.9
conda activate spatial-env
Install the required libraries:

bash
Copy code
pip install -r requirements.txt
Usage
Activate the conda environment:

bash
Copy code
conda activate spatial-env
Open Jupyter Notebook:

bash
Copy code
jupyter-notebook
**Navigate to the notebook you want to run and follow the instructions within each notebook.

Notebooks
1_rasters_reprojections_merging.ipynb:

Focuses on raster reprojection and merging using libraries such as rasterio, geoio, and gdal.
2_dataframe_generation.ipynb:

Details the process of generating dataframes from spatial data, including the use of pandas, geopandas, and various preprocessing techniques.
3_gap_poor_IDW_interpolation_and_alignment.ipynb:

Covers interpolation techniques and alignment of spatial data, focusing on methods like IDW interpolation.
4_modelling.ipynb:

Demonstrates the process of building and evaluating models using the processed spatial data, with tools such as RandomForestRegressor and LinearRegression.
Contributing
Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are reviewed on a regular basis.

Fork it (https://github.com/yourusername/spatial-data-processing/fork)
Create your feature branch (git checkout -b feature/your-feature)
Commit your changes (git commit -am 'Add some feature')
Push to the branch (git push origin feature/your-feature)
Create a new Pull Request
License
This project is licensed under the MIT License - see the LICENSE file for details.
