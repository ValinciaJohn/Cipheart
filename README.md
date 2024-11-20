**Cipheart: Secure Heart, Smart Start – Predicting with Privacy**
Cipheart is an innovative Streamlit application designed to classify heart disease risk based on the well-known UCI Heart Disease dataset. The app allows users to select between **Logistic Regression** and **Naive Bayes** machine learning models for heart disease prediction. To ensure the privacy and security of sensitive health data, Cipheart integrates **CKKS homomorphic encryption**, which allows computations to be performed on encrypted data without compromising privacy. 
This combination of machine learning and encryption empowers users to make informed health decisions securely. With a user-friendly interface, Cipheart caters to both technical and non-technical users, offering a seamless experience in predicting heart disease risk while maintaining high standards of data security and privacy.

Features

Data Preprocessing:
The Cipheart app provides users with the ability to upload a CSV file containing heart disease data. Once uploaded, the app performs several preprocessing steps to ensure the data is ready for analysis. It removes any duplicate entries, fills missing numerical values with the median, and fills missing categorical values with the mode. Additionally, categorical features (e.g., gender) are encoded to prepare them for model input. Numerical features are then scaled using StandardScaler to standardize the data for model training. Outliers in the numerical features are detected and removed based on the interquartile range (IQR), ensuring the quality of the dataset for better model performance.

Machine Learning Models:
Cipheart offers two machine learning models for heart disease prediction: Logistic Regression and Naive Bayes. The logistic regression model is trained and evaluated using the preprocessed data, with various performance metrics like accuracy, precision, recall, and F1-score displayed. Similarly, the Naive Bayes classifier, specifically Gaussian Naive Bayes, is available for prediction and performance evaluation. To help users interpret model performance, the app visualizes the evaluation metrics through bar plots, confusion matrix heatmaps, and plots the ROC curve for binary classification tasks.

Homomorphic Encryption with CKKS:
For enhanced data privacy, Cipheart incorporates CKKS homomorphic encryption. This feature allows users to make secure predictions while maintaining the confidentiality of sensitive health data. By applying CKKS encryption, the app ensures that user data is encrypted during model inference. Predictions are made using encrypted data, and the app can perform computations on the encrypted data without the need to decrypt it. Users have the option to apply encryption to both the Logistic Regression and Naive Bayes models, ensuring that even the model weights and biases are calculated in an encrypted form, preserving the privacy of the input data throughout the process.

Visualization:
Cipheart includes various visualizations to help users understand both the data and the model's performance. Boxplots are used to visualize the data before and after outlier removal, providing insight into the effect of this preprocessing step. Additionally, the model performance is assessed using confusion matrices and classification reports, which include metrics such as accuracy, precision, recall, and F1-score. For binary classification tasks, the app also visualizes the ROC curve, enabling users to evaluate the trade-off between the true positive rate and false positive rate.

User Interactivity:
The app is designed to be user-friendly and interactive. Users can upload a CSV file containing heart disease data using the File Uploader feature. They can select between Logistic Regression, Naive Bayes, or both models for prediction. Additionally, users have the option to enable encryption to ensure data privacy during prediction. The data preprocessing steps can be triggered manually, giving users control over cleaning, scaling, and outlier removal before proceeding to the modeling phase.

Conclusion:
Cipheart combines the power of machine learning and homomorphic encryption to offer secure, accurate heart disease predictions. It's the smart choice for privacy-conscious health data analysis.






