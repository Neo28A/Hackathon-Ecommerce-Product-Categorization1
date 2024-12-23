# Ecommerce Product Categorization

This repository contains the solution to the **Ecommerce Product Categorization** hackathon challenge. The project focuses on developing an efficient text classification model to categorize eCommerce products based on their descriptions.

## Problem Statement

In the fast-paced eCommerce industry, accurate product categorization is critical for improving customer experience, reducing search friction, and enhancing product discoverability. The challenge lies in handling ambiguities, unconventional naming conventions, and multi-language data. This project addresses these challenges with an innovative and scalable solution.

## Approach

1. **Data Handling:**
   - Loaded and explored the dataset for valuable insights.
   - Addressed class imbalance using stratified sampling and SMOTE oversampling.
   
2. **Text Preprocessing:**
   - Used **NLTK** for natural text preprocessing.
   - Converted textual descriptions to numerical features using techniques like **TF-IDF** and **Word2Vec**.
   
3. **Model Development:**
   - Performed train-test split using stratified sampling.
   - Trained and evaluated various machine learning models:
     - Support Vector Machine (SVM)
     - Logistic Regression
     - Random Forest
     - Decision Tree
     - K-Nearest Neighbors (KNN)
   - Fine-tuned the models using hyperparameter optimization to improve performance.

4. **Evaluation:**
   - Compared models based on their train and test accuracy.
   - Selected **SVM** as the best-performing model with a test accuracy of **98%**.

## Key Insights

- **Price Correlation:** Higher retail prices correspond to higher discount prices.
- **Top Sellers:** Clothing and Jewelry are the highest-selling categories.
- **Low Sellers:** Bags, Wallets & Belts, and Baby Care show the lowest sales.
- **Jewelry Pricing:** Jewelry has the highest average retail and discounted price.

## Results

| Model                | Train Accuracy | Test Accuracy |
|----------------------|----------------|---------------|
| SVM                 | 99.78%         | 98.19%        |
| Logistic Regression | 99.52%         | 98.04%        |
| Random Forest       | 99.90%         | 97.85%        |
| Decision Tree       | 99.90%         | 96.29%        |
| KNN Classifier      | 99.50%         | 95.11%        |

### Combined Model Performance

- The combined model (SVC, Logistic Regression, and Random Forest) achieved:
  - **Test Accuracy**: 98.44%
  - **F1 Score**: 98.43%
- The classification report highlights:
  - High precision and recall across most classes.
  - Weighted average F1-score of **98%**, demonstrating balanced performance.
- The ensemble model effectively handles class imbalances while maintaining high predictive accuracy.

## Benefits of Accurate Categorization

1. **Improved Customer Experience:** Enhanced browsing and navigation for seamless product discovery.
2. **Increased Product Discoverability:** Broader exposure to relevant products, boosting sales and satisfaction.
3. **Reduced Search Friction:** Faster and frustration-free searches, reducing abandoned sessions.

## Conclusion and Future Work

The accurate categorization model developed in this project is a crucial tool for improving eCommerce platforms. Future enhancements may include:
- Exploring advanced deep learning models.
- Integrating visual features, such as product images, for better accuracy.
