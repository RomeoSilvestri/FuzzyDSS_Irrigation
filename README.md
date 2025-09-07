# ML - DSS

# Soil Moisture Prediction & Decision Support System for Irrigation Scheduling

**Repository Name:** ML-DSS

**Author:** Romeo Silvestri

## Overview

This repository contains machine learning models developed to predict soil moisture levels using tensiometer data and to create a Decision Support System (DSS) for irrigation management. The project is part of the IRRITRE initiative by FBK (Fondazione Bruno Kessler), aimed at optimizing irrigation practices for various agricultural consortia in the Trentino-Alto Adige region.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Content](#content)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Effective irrigation management is crucial for sustainable agriculture, especially in regions with varying water availability. This project leverages machine learning techniques to predict soil moisture levels based on tensiometer readings and weather data. It uses these predictions to inform irrigation decisions. The aim is to support agricultural consortia in the Trentino-Alto Adige region by providing actionable insights that enhance water use efficiency and crop yield.

## Project Structure

The project structure "ML-DSS" is designed to clearly separate the different components and areas of work within the project.

- .idea: This folder contains all the requirements and specifications of the project, typically managed by IDEs or project management tools.

- dss: This folder contains everything related to the Decision Support System (DSS).

- ml_models: This folder contains everything related to the machine learning (ML) for Soil Moisture Forecasting.

- presentation: This folder contains resources used for project presentations.

- spatial_interpolation: This folder contains everything related to spatial interpolation.

- LICENSE: This file contains the project's license, specifying the terms of use for the code and data.

- README.md: This file contains the project documentation, including an overview of the project, installation and usage instructions, and other useful information.

- requirements.txt: This file contains a list of all the dependencies required to run the project.

Additionally, each of the folders "dss", "ml_models", and "spatial_interpolation" contain subfolders for "data", "deployment", "research" and a special folder for "package". This structure helps to keep the various aspects of the work organized, facilitating collaboration among team members, simplifying code and data management-maintenance.

The project structure is as follows:
```
ML-DSS
├── .idea
├── dss
│ ├── data
│ ├── deployment
│ ├── package
│ ├── research
├── ml_models
│ ├── data
│ ├── deployment
│ ├── package
│ ├── research
├── presentation
│ ├── notebook
│ ├── pdf
│ ├── powerpoint
├── spatial_interpolation
│ ├── data
│ ├── deployment
│ ├── research
├── LICENSE
├── README.md
└── requirements.txt
```

## Installation

The Project requires Python 3.10 or higher.

To get started, clone this repository and install the required dependencies.

```bash
git clone https://gitlab.com/romeo_silvestri/ml-dss.git
cd ml-dss
pip install -r requirements.txt
```

## Content

This project employs various machine learning models to predict soil moisture levels, including:
- Linear Regression
- ARIMAX
- Random Forest
- Gradient Boosting
- Neural Networks

On the other hand, geo-statistical methods such as Ordinary Kriging are used for spatial interpolation of soil moisture data.

Finally, the project integrates these models into a Decision Support System (DSS) for irrigation management. The DSS follows the Fuzzy Logic approach to provide actionable insights to farmers, defining a handful of irrigation rules to observe. There are many stages for developing the DSS, including architecture definition, creation of a Feedback & Improvement System, and model deployment.

Data

The data used in this project includes tensiometer readings collected from various agricultural fields in the Trentino-Alto Adige region. The data is divided into training and test sets to validate the model performance.

Evaluation Metrics

Model performance is evaluated using metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² score.

Results

The models developed in this project provide accurate predictions of soil moisture levels, which are used to create a Decision Support System (DSS) for irrigation management. The DSS provides farmers with recommendations on when and how much to irrigate, optimizing water use and improving crop yields.

## Contributing

We welcome contributions to enhance the functionality and performance of the models and the DSS. Please follow the standard GitLab workflow for contributions:

1) Fork the repository.
2) Create a feature branch (git checkout -b feature/your_feature).
3) Commit your changes (git commit -m 'Add some feature').
4) Push to the branch (git push origin feature/your_feature).
5) Open a Merge Request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

For more information or any queries, please contact Romeo Silvestri at rsilvestri@fbk.eu.