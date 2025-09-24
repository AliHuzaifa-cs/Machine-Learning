# K-Nearest Neighbors (KNN) Algorithm  

## Introduction  
The **K-Nearest Neighbors (KNN)** algorithm is a **supervised learning algorithm** used for both **classification** and **regression** problems.  
It is a **non-parametric, lazy learning algorithm** which means it does not make strong assumptions about the data and does not explicitly build a model.  

Instead, it memorizes the training data and makes predictions based on the **similarity (distance)** between data points.  

---

## How KNN Works (Step by Step)  
1. Choose the number of neighbors **K**.  
2. Calculate the **distance** (usually Euclidean distance) between the new data point and all training points.  
3. Select the **K nearest neighbors**.  
4. For **classification**:  
   - Take the **majority vote** of the neighbors’ classes.  
   - Assign the class with the highest votes.  
5. For **regression**:  
   - Take the **average** of the neighbors’ values.  

---

## Distance Metrics Used in KNN  
- **Euclidean Distance**:  
  \[
  d(p, q) = \sqrt{\sum_{i=1}^{n} (p_i - q_i)^2}
  \]  

- **Manhattan Distance**:  
  \[
  d(p, q) = \sum_{i=1}^{n} |p_i - q_i|
  \]  

- **Minkowski Distance** (generalized form).  

---

## Choosing the Right K  
- Small **K** → High variance (can lead to overfitting).  
- Large **K** → High bias (can oversmooth results).  
- Use **cross-validation** to select the best value of K.  

---

## Advantages of KNN  
- Simple to implement and understand.  
- No training phase required (lazy learning).  
- Works well with small datasets.  

---

## Disadvantages of KNN  
- Computationally expensive for large datasets.  
- Sensitive to irrelevant features and data scaling.  
- Performance decreases with high-dimensional data (curse of dimensionality).  

---

## Applications of KNN  
- Handwriting recognition.  
- Recommender systems.  
- Medical diagnosis.  
- Customer segmentation.  

---


