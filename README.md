# NLP_Application

**Report: Clause Extraction and Classification from Legal Contracts**

**Objective**: The goal is to develop an NLP-based solution to:
1.	Extract legal clauses from contracts.
2.	Classify them into predefined categories.
3.	Summarize effectively for better contract analysis.
    
**Dataset**: Legal Clause Dataset containing labeled legal clauses

**Preprocessing**: Steps taken for text preprocessing:
•	Tokenization: Splitting text into tokens using NLTK.
•	Stopword Removal: Filtering out common words like "the", "and", etc.
•	Stemming: Reducing words to their base forms using PorterStemmer.
•	Lemmatization: Further normalization for meaningful word forms.

**Feature Extraction:**
•	TF-IDF Vectorization:
o	Transformed processed text into numerical features.
o	Limited to the top 5,000 features to balance model complexity and performance.

**Model Training and Evaluation**
•	Classifier Used: Random Forest Classifier.
•	Train-Test Split:
  o	Training Data: 80%.
  o	Test Data: 20%.

**Evaluation Metrics**
Metric	Value
Accuracy	0.60
Precision	0.63
Recall	0.60
F1-Score	0.57

**Insights from Feature Importance**: Top features contributing to predictions:
1.	agreement
2.	shall
3.	term
4.	compani
5.	parti 
 
**Example Inference**
A new clause was tested:
**Clause**: "The supplier must deliver the goods within 30 days of receiving the purchase order."
**Predicted Label**: good-reason
This demonstrates the model's ability to classify clauses accurately for the sample example.

**Conclusion**
1.	Strengths:
o	The pipeline effectively preprocesses and classifies legal clauses.
o	Visualizations provide useful insights into data distribution and model performance.
2.	Areas for Improvement:
o	Handle class imbalances using techniques like oversampling or class weights.
o	Explore advanced models for better clause classification.
3.	Next Steps:
o	Assess other classifiers to test model performance.
o	Explore clause summarization.
![image](https://github.com/user-attachments/assets/816cff0b-48ba-4962-93ad-d642f34440fe)
