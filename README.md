# A Comparative Study in Digits Recognition Through Convolutional Neural Network and Support Vector Machines

**Author:** Nizar Assad  
**Email:** Nizar.Assad@city.ac.uk

This study compares the performance of Convolutional Neural Network (CNN) and Support Vector Machine (SVM) models in classifying the MNIST dataset. The analysis explores the applicability of each model, including the hierarchical feature extraction of CNNs and the hyperplane optimization of SVMs. The results provide insights into the strengths and weaknesses of each model, offering guidance for selecting appropriate models for image classification tasks.


## Methods

### Dataset

The MNIST dataset contains 70,000 grayscale images of handwritten digits, each 28x28 pixels in size. The dataset is evenly distributed among ten classes (digits 0-9), ensuring a balanced training ground for model evaluation.

### Convolutional Neural Network (CNN)

- **Architecture:** Custom CNN with convolutional layers, ReLU activations, max-pooling, and fully connected layers.
- **Hyperparameters:** Optimized using grid search for learning rate, batch size, and number of epochs.
- **Performance Metrics:** Accuracy, confusion matrix, precision, recall, F1-score.

### Support Vector Machine (SVM)

- **Linear SVM:** Utilizes linear decision boundaries.
- **Non-linear SVM:** Employs Radial Basis Function (RBF) kernel to map data into a higher-dimensional space.
- **Hyperparameters:** Optimized gamma and regularization parameter (C) using K-Fold Cross-Validation.
- **Performance Metrics:** Accuracy, confusion matrix, precision, recall, F1-score.

## Results, Findings & Evaluation

### Model Selection

A systematic approach was used to evaluate the models, including a comparison of performance metrics, confusion matrices, and ROC analysis.

### Algorithm Comparison

#### Convolutional Neural Network (CNN)

- **Test Accuracy:** 0.9362
- **Observations:** Strong in identifying digits '0', '1', and '4'; challenges with '2' and '7', '5' and '3'.

#### Support Vector Machine (SVM)

- **Test Accuracy:** 0.9689 (Non-linear SVM with RBF kernel)
- **Observations:** High precision and recall, particularly accurate in identifying digits '0', '1', '2', and '4'.

### Comprehensive Evaluation

- **ROC Curve & AUC:** Both models achieved an AUC of 0.99, indicating high discriminative power.

### Visualizations

- **Figure 1:** Confusion Matrix for CNN  
_(Include visual representation here)_

- **Figure 2:** Confusion Matrix for SVM  
_(Include visual representation here)_

- **Figure 3:** Micro-Average ROC Curve  
_(Include visual representation here)_

## Conclusion

The study reveals that while CNNs offer robust performance with their hierarchical feature extraction, the Non-linear SVM with an RBF kernel excels in capturing intricate patterns and achieves superior accuracy. Both models demonstrate high discriminative power, with the SVM slightly outperforming the CNN in overall accuracy and precision.

## References

1. Virnodkar, S., et al. (2020). CaneSat dataset to leverage convolutional neural networks for sugarcane classification. *Journal of King Saud University - Computer and Information Sciences*.
2. Etzold, D. (2022). MNIST - dataset of handwritten digits. *Medium*.
3. Saini, A. (2023). Guide on Support Vector Machine (SVM) algorithm. *Analytics Vidhya*.
4. GeeksforGeeks. (2023). Introduction to convolution neural network.
5. Rendyk. (2023). Tuning the hyperparameters and layers of neural network deep learning. *Analytics Vidhya*.
6. LeCun, Y., Cortes, C., & Burges, C. (1998). The MNIST Database of Handwritten Digits.
7. Pedregosa, F., et al. (2011). Scikit-learn: Machine Learning in Python. *Journal of Machine Learning Research*.
