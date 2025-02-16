## Research: Privacy-Preserving Heart Disease Detection Using Federated Random Forest

### Overview
We worked on a federated learning-based heart disease detection system using Python. The goal was to create a machine-learning model that predicts heart disease while ensuring patient data privacy. The project utilized `Horizontal Federated Learning (HFL)` and a Random Forest classifier to enable multiple hospitals to collaboratively train a model without sharing sensitive data.

[Publication Link](https://ieeexplore.ieee.org/document/9929490)


<p align="center"><img title="a title" alt="Alt text" src="https://www.dailydoseofds.com/content/images/2023/11/federated-gif.gif" width="50%"></p>



### Execution Steps

**1. Dataset Preparation**

    - Used a heart disease dataset with 1,190 patient records from five hospitals.
    
    - Preprocessing: Removed outliers using Z-score normalization and handled missing values.
    
    - Data Partitioning: Divided data across multiple clients (hospitals) to simulate decentralized data storage.
    
**2. Model Development**

    - Algorithm: Implemented Random Forest, which is robust against overfitting and performs well with tabular medical data.
    
    - Federated Learning Approach:
    
        - A global model was trained on a central federated server.
        
        - The model was distributed to local hospital clients, where it was trained on their private data.
        
        - Clients sent back only the model parameters (not raw data) to update the global model.
        
    - Helper Functions: Developed Python functions to filter and aggregate non-repetitive model parameters from clients.
    
**3. Hyperparameter Tuning**

    - Used Grid Search to optimize parameters like the number of decision trees (estimators) and depth of the Random Forest model.
    
    - Evaluated performance using Accuracy, Precision, Recall, and F1-score metrics.
    
**4. Experimental Evaluation & Results**

    - Conducted experiments in two phases:
    
        1. Initial model training and parameter exchange between clients and the central server.
        
        2. Retraining with additional data to enhance model accuracy.
        
    - Achieved 92.41% accuracy after iterative training, improving performance over standalone hospital models.


***Key Takeaways***

**Data Privacy:** Patients’ data remained local, ensuring compliance with regulations like GDPR. 

**Federated Learning Efficiency:** Model performance improved with each iteration without requiring centralized data collection. 

**Scalability:** This approach can be extended to other diseases and healthcare applications.
