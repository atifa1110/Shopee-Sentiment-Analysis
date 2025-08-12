# Shopee Sentiment Analysis

## Data Collection:
Data obtained via web scraping using Google Scraping, totaling 50,000 review samples.

## Sentiment Classes:
The sentiment analysis results were categorized into three main classes:
- Positive — reviews expressing satisfaction or praise.
- Negative — reviews containing complaints, dissatisfaction, or criticism.
- Neutral — reviews that are informative, ambiguous, or do not convey a strong positive or negative sentiment.

## Methods and Models Tested:
1. Logistic Regression with Bag of Words (BoW) representation
2. Logistic Regression with TF-IDF representation
3. Support Vector Machine (SVM)
4. CNN-LSTM (Convolutional Neural Network + Long Short-Term Memory)

## Model Evaluation Results:
1. CNN-LSTM:
    - Best performance with highest accuracy at 92.4%
    - Balanced F1-score across all classes
2. SVM:
    - Second best with stable performance
    - Accuracy of 91.5%
3. Logistic Regression (BoW):
    - Reliable with 90.2% accuracy
    - Suitable for resource-constrained scenarios
4. Logistic Regression (TF-IDF):
    - Lowest accuracy at 86.8%
    - Less accurate, especially on neutral class

## Additional Insights:
- For new text predictions, Logistic Regression (both TF-IDF and BoW) shows better consistency in understanding neutral and ambiguous contexts.
- Recommended Model Usage:
    - CNN-LSTM for maximum performance
    - SVM for balance between performance and stability
    - Logistic Regression (BoW) for computational efficiency

## Suggestions:
1. Experiment further with advanced architectures such as transformers or attention-based models for improved understanding of context.
2. Perform data augmentation or use external sentiment lexicons to enrich training data.
3. Explore hyperparameter tuning and ensemble methods to boost model robustness.
4. Investigate real-time deployment feasibility and model inference speed for production use.
5. Incorporate user feedback loops to continually improve model accuracy and relevance.

