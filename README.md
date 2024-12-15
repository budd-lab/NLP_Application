### Project Title: Clause Extraction and Classification from Legal Contracts

**Author - Buddhendra Shukla**

#### Executive summary

#### Rationale
Why should anyone care about this question?

Contracts run businesses and unstructured data form the backbone of business operations, capturing critical business information, obligations, and risks. Manual review of contracts is time-intensive and prone to errors. By automating this process, businesses can reduce the time and cost of contract review and minimize risks by consistently identifying and addressing key contractual clauses. This will also empower non-legal personnel with tools to quickly understand contract obligations. This analysis could help bridge the gap between AI tools and real-world usability, translating complex legal documents into actionable insights that can be understood and leveraged by diverse stakeholders.

#### Research Question
What are you trying to answer?

#### Data Sources
What data will you use to answer you question?

Legal Clause Dataset containing labeled legal clauses

#### Methodology
What methods are you using to answer the question?

Preprocessing: Steps taken for text preprocessing:

- Tokenization: Splitting text into tokens using NLTK.
- Stopword Removal: Filtering out common words like "the", "and", etc.
- Stemming: Reducing words to their base forms using PorterStemmer.
- Lemmatization: Further normalization for meaningful word forms.

**Feature Extraction**: TF-IDF Vectorization:
- Transformed processed text into numerical features.
- Limited to the top 5,000 features to balance model complexity and performance.

**Model Training and Evaluation**
- Classifier Used: Random Forest Classifier.
- Train-Test Split: (Training Data: 80% and Test Data: 20%)

#### Results
What did your research find?

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
- **Clause**: "The supplier must deliver the goods within 30 days of receiving the purchase order."
- **Predicted Label**: good-reason

This demonstrates the model's ability to classify clauses accurately for the sample example.

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()

##### Contact and Further Information
