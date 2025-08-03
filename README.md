# Power System Fault Detection and Classification

## Overview
This project involves designing and implementing a machine learning solution to detect and classify faults in power distribution systems. Using voltage and current phasor data, the model distinguishes between normal operating conditions and various types of faults such as line-to-ground (LG), line-to-line (LL), double line-to-ground (LLG), three-phase (3P), and no-fault conditions.

The system aims to provide rapid and accurate fault identification, which is essential for maintaining power grid stability, reliability, and enabling swift operational responses.

## Dataset
The project utilizes the **Power System Faults Dataset** from Kaggle, which contains voltage and current phasor data labeled for different fault types. The dataset includes features such as voltage (Ua, Ub, Uc), current (Ia, Ib, Ic), fault labels, fault locations, power loads, temperature, and wind speed.

## Features
- Data preprocessing including noise filtering, handling missing values, and feature normalization.
- Feature engineering such as symmetrical sequence component extraction and statistical feature calculations.
- Model training and evaluation using multiple classifiers, with a focus on Random Forest for robustness and interpretability.
- Hyperparameter tuning with cross-validation.
- Deployment of the trained model as a real-time REST API on IBM Cloud using IBM Watsonx.ai Runtime.

## Technology Stack
- Python 3.11
- Libraries: pandas, scikit-learn, LightGBM
- IBM Watsonx.ai Studio and Watsonx.ai Runtime (Lite plan)
- Jupyter Notebooks for development and experimentation

## Key Components
- **Data Collection**: Phasor measurements and operational/environmental parameters under various fault conditions.
- **Model Training**: Random Forest Classifier trained on 80% of the data with cross-validation.
- **Evaluation**: Uses metrics such as accuracy, precision, recall, and confusion matrix to assess classification performance.
- **Deployment**: Model is deployed as a REST API service on IBM Cloud for real-time fault detection and classification.

## Results
The model achieved high accuracy in differentiating between normal operation and multiple fault types, enabling faster detection and response to power system anomalies.

## Future Enhancements
- Integration with real-time PMU (Phasor Measurement Units) data streams for live fault detection.
- Fault localization to estimate fault distance on power lines.
- Incorporating unsupervised learning techniques for detecting novel or unseen fault types.
- Edge deployment using Kubernetes for ultra-low latency fault identification.

## References
- Power System Faults Dataset – Kaggle (Ziya07)
- IBM Watsonx.ai Studio & Watsonx.ai Runtime Documentation
- Li, S. et al., “Sparse Representation–Based Fault Classification in Power Systems,” IEEE Transactions on Power Systems, 2015.
- Breiman, L., “Random Forests,” Machine Learning, 2001.

## Author
**Sai Lalith Palagummi**  
Sreenidhi Institute of Science and Technology  
Department of Computer Science and Engineering (CSE)

---

Thank you for exploring this project! Feel free to contribute or raise issues for improvements.
