# Credit-Card-Fraud-Detection-Analysis

## Introduction

In the digital age, fraudulent activities have become increasingly sophisticated, posing significant challenges to financial institutions and consumers alike. This project aims to enhance the accuracy of fraud detection models by implementing advanced data preprocessing techniques and machine learning algorithms. Our goal is to develop a robust model capable of accurately distinguishing between legitimate and fraudulent transactions, thereby reducing financial losses and improving security measures.

## Methodology

To achieve our objectives, we employed the following steps:

1. **Data Collection**: Acquired a kaggle dataset containing transaction records labeled as legitimate or fraudulent by the Machine Learning Group.

2. **Data Preprocessing**:
   - **Handling Class Imbalance**: Utilized Synthetic Minority Over-sampling Technique (SMOTE) to address the imbalance between legitimate and fraudulent transactions.
   - **Noise Reduction**: Applied Edited Nearest Neighbors (ENN) to remove mislabeled or noisy instances from the dataset.

3. **Feature Scaling**: Standardized the 'Amount' feature using StandardScaler to ensure all features contribute equally to the model's performance.

4. **Model Training**: Implemented and trained a machine learning model (e.g., RandomForestClassifier) on the preprocessed dataset.

5. **Evaluation**: Assessed the model's performance using metrics such as Precision, Recall, F1-score, and the area under the Precision-Recall curve (PR AUC).

## Results

After implementing the above methodology, the enhanced model achieved the following performance metrics:

- **Precision**: 0.90
- **Recall**: 0.92
- **F1-score**: 0.91
- **PR AUC**: 0.8547

The Precision-Recall curve below illustrates the trade-off between precision and recall:

![Precision-Recall Curve](path_to_pr_curve_image)

## Conclusion

By integrating SMOTE and ENN for data preprocessing and employing a robust machine learning algorithm, we significantly improved the model's ability to detect fraudulent transactions. These enhancements contribute to more reliable fraud detection systems, ultimately aiding in the prevention of financial fraud.

## Future Work

To further improve the model's performance, future efforts could focus on:

- Exploring additional feature engineering techniques.
- Implementing ensemble methods to combine multiple models.
- Conducting hyperparameter tuning to optimize model parameters.

## How to Use

1. **Installation**: Clone this repository and install the required dependencies listed in `requirements.txt`.

2. **Data Preparation**: Place the transaction dataset in the designated data folder.

3. **Training the Model**: Run the `train_model.py` script to preprocess the data and train the model.

4. **Evaluating the Model**: Execute the `evaluate_model.py` script to assess the model's performance and generate evaluation metrics.

## Contributing

We welcome contributions to further enhance this project. Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

## Acknowledgments

We extend our gratitude to the collaborators for the Credit Card Fraud Detection Dataset and the developers of the SMOTE and ENN techniques, as well as the contributors to the machine learning libraries utilized in this project.

