This repository contains the final project for the ENS491-492 Graduation Project, titled Classification of Background Events in X-ray Imaging Detectors with Machine Learning. The project aims to enhance the sensitivity of the iXRD (Improved X-ray Detector) onboard the Sharjah-Sat-1 CubeSat, focusing on distinguishing between source signals and background noise in X-ray data using advanced computational methods.

Project Overview

The project addresses key challenges in X-ray astronomy, specifically the high levels of background radiation affecting the detectors. It leverages machine learning models to classify and reduce background events, improving detection accuracy. Various machine learning models, including k-means clustering, linear and non-linear models, and neural networks, are applied to simulation data generated using the GEANT4 software.

Methodology

Data Simulation & Preprocessing:

GEANT4 simulations generate different event types, such as source (Crab), Cosmic X-ray Background (CXB), and albedo photons.
The simulation data is processed to calculate event positions and energies, forming labeled datasets for training.

Clustering & Classification:

Initial clustering using k-means helps identify features and patterns in the data.
Supervised models, including XGBoost, Random Forest, and Neural Networks, are trained for binary classification of source and background events.

Detector Response Calculation:

The response matrix of the iXRD is computed to account for the detector's internal characteristics, converted into FITS format for use in standard analysis tools.

Results & Impact

The models demonstrate successful classification of simulated data with high accuracy, paving the way for real data analysis once Sharjah-Sat-1 is operational. This approach can be extended to other CubeSat missions, enhancing the reliability of compact X-ray detectors in space research.
