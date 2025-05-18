#  Banknote Authentication using K-Means Clustering

This project presents an unsupervised learning model using the K-Means algorithm to classify banknotes as genuine or forged, based on statistical features extracted from wavelet-transformed images.

---

##  Project Objective
To build a model capable of distinguishing between genuine and forged banknotes without using labeled data during training.

---

##  Technologies Used
- K-Means Clustering Algorithm
- Data Normalization
- Confusion Matrix Analysis
- Data Visualization with Matplotlib

---

##  Dataset Description
- Source: [Kaggle - Bank Note Authentication](https://www.kaggle.com/datasets/ritesaluja/bank-note-authentication-uci-data)
- Total records: 1372
- Features:
  - Variance
  - Skewness
  - Curtosis
  - Entropy
- Label (class): 0 = Genuine, 1 = Forged

---

##  Implementation Steps

1. Import necessary libraries (pandas, numpy, matplotlib, sklearn)
2. Load and preprocess the dataset
3. Normalize feature values to a [0, 1] range
4. Apply K-Means clustering with 2 clusters
5. Compare predicted clusters with actual labels to calculate accuracy
6. Visualize the clustering results

---

##  How Does K-Means Work Without Labeled Data?
K-Means does not use actual labels during training. Instead, it relies on statistical features (like variance and skewness) to group similar data points into clusters. If forged and genuine banknotes differ significantly in these features, the algorithm will naturally separate them into two clusters. After clustering, the results are compared with the real labels to evaluate performance. This method is effective when the data has clear patterns.

---

##  Results
- Classification Accuracy: **87.24%**



---

##  Requirements
To install the required dependencies, run:
```bash
pip install -r requirements.txt
```

---

##  Conclusion
The K-Means algorithm proved effective in identifying forged banknotes based solely on statistical features, without needing labeled training data. It is a simple and efficient approach that can be extended to build intelligent fraud detection systems.

