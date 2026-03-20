# Week 01 Progress Report: Project Foundation
**Project:** AI for Prediction of Desertification Patterns  
**Group ID:** 101  
**Date:** [23/01/2026]

## 1. Project Problem Statement & Objectives
During this initial phase, the team finalized the scope of the project to ensure a "Proactive" approach rather than a "Reactive" one.

* **Problem Statement:** Conventional methods for monitoring desertification are retrospective. This project aims to develop a predictive AI framework to identify future land degradation patterns using multi-temporal satellite data.
* **Finalized Objectives:**
    1.  Perform spatio-temporal analysis of arid regions using 10+ years of satellite data.
    2.  Implement a Deep Learning model (ConvLSTM) to forecast desertification frontiers.
    3.  Develop a visualization tool for environmental risk assessment.

## 2. Literature Survey & Technical Foundation
We conducted a preliminary review of existing research to establish a baseline for our AI model.

* **Remote Sensing Indices:** We identified **NDVI (Normalized Difference Vegetation Index)** and **LST (Land Surface Temperature)** as the primary input features.
* **Algorithmic Research:** Studied the effectiveness of **CNNs** for spatial feature extraction and **LSTMs** for temporal sequence prediction.
* **Gap Analysis:** Found that most current literature lacks integrated "Frontier Prediction" models, which confirms the **Novelty** of our project.



## 3. Tools & Technologies Understood
The following tech stack has been finalized and configured for the development environment:

| Category | Tool Selected | Justification |
| :--- | :--- | :--- |
| **Language** | Python 3.10+ | Standard for AI/ML development. |
| **Data Engine** | Google Earth Engine (GEE) | To process petabytes of satellite data via API. |
| **Deep Learning** | TensorFlow / Keras | For building the predictive neural network layers. |
| **GIS Mapping** | QGIS / GeoPandas | For spatial data visualization and final output rendering. |

## 4. Work Planned for Week 02
* **System Architecture:** Finalize the data flow diagram from ingestion to prediction.
* **Dataset Acquisition:** Start collecting Landsat-8 and Sentinel-2 tiles for the study area.
* **Detailed Literature Review:** Complete a comprehensive bibliography of at least 10 high-impact research papers.
