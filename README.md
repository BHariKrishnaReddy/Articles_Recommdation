### Medium Article Recommendation Project

##### 1. Introduction

1.1 Data Set Description
The dataset, post feature engineering, comprises 192,365 entries with 12 columns, capturing essential aspects of Medium articles. The dataset is enriched with individual tags (T1 to T5), and textual content and tags are combined into a unified 'content' column. This detailed dataset serves as the foundation for a comprehensive analysis of Medium's diverse content landscape.

1.2 Problem Statement
The project aims to not only explore traditional aspects of the dataset but also incorporate advanced text analysis using BERT-based sentence embeddings. This addition allows for a more nuanced understanding of semantic similarities and relationships within article content.

##### 2. Motivation and Research Questions

2.1 Motivation
The primary motivation behind this project is to extract meaningful insights from medium articles data by performing feature engineering analysis and encoding the data. This analysis can help businesses, policymakers, and researchers understand public sentiment, identify trends, and respond effectively to emerging issues.

2.2 Research Questions
The research questions for this project encompass a broad spectrum of inquiries aimed at understanding the dynamics of Medium articles.

What are the prevalent categories and topics covered in Medium articles?
How are articles distributed across these themes, and what is the impact of associated tags?
What is the prevalence and potential influence of articles with multiple authors on engagement metrics?
What are the temporal trends in article distribution over different years?
What are the popularity and frequencies of tags (T1 to T5), and what themes do they represent?
How does textual content vary across categories and tags, and what insights can be gained using BERT-based sentence embeddings?
Is there a correlation between user engagement metrics (claps and comments) and the number of tags and authorship patterns?
How effective is the proposed webpage extension in summarizing content and suggesting related websites based on page rank similarity?


##### 3. Methods Used

3.1 Data Cleaning and Feature Engineering
The initial steps involve dropping null values, typecasting, and feature engineering on the 'timestamp.' Data cleaning is applied to 'title,' 'author,' and 'text,' involving the removal of invalid characters and lowering the case. The enriched dataset enables a robust analysis of various facets of Medium articles.

3.2 Exploratory Data Analysis (EDA)
Traditional EDA is complemented by advanced analysis, including the examination of articles with multiple authors and the temporal distribution of articles. The average number of tags per article is also explored.

3.3 Text Analysis with Sentence Embeddings
The introduction of BERT-based sentence embeddings, specifically 'bert-base-nli-mean-tokens,' enriches the analysis. The model, inspired by BERT and RoBERTa, utilises a mean pooling layer and siamese network structure for semantically meaningful sentence representations.

3.4 Word Clouds
Word clouds are generated for each sentiment category, providing a visual representation of the most frequent words. This aids in identifying key themes and understanding the language used in articles associated with different categories.

3.5 Model Architecture and Training
The model architecture utilizes the 'bert-base-nli-mean-tokens' pre-trained Sentence Transformer model. The architecture employs a siamese network structure, inspired by BERT and RoBERTa, enhancing semantic understanding for sentence embeddings. The model is fine-tuned on Natural Language Inference (NLI) data to optimize performance.

##### 4. Findings

4.1 Data Preprocessing
The preprocessing steps effectively clean the Articles data, ensuring that the subsequent analysis is based on high-quality input.

4.2 Exploratory Data Analysis
Discoveries from the EDA provide valuable insights into the content landscape of Medium articles. The analysis unveils the distribution of article categories and tags, shedding light on the prevalence of diverse themes. Collaborative authorship patterns, temporal evolution, and popularity of individual tags (T1 to T5) are also highlighted.

4.4 Key Findings
Categories: The dataset exhibits a diverse range of articles across various categories, highlighting the richness of Medium's content.
Tag Distribution: Tags T1 to T5 exhibit varying popularity, offering insights into prevailing topics.
Temporal Trends: Fluctuations in article publications over years reflect evolving trends or seasonal patterns.
Text Analysis: BERT-based sentence embeddings unveil semantic similarities between articles, providing a deeper understanding of content relationships.
4.5 Predictions
The trained model recommends articles, showcasing its potential for real-world applications.

##### 5. Conclusion and Future Work

5.1 Conclusion
In conclusion, the comprehensive analysis of the Medium articles dataset has provided multifaceted insights into the platform's content landscape. Exploratory Data Analysis (EDA) revealed diverse categories and tags, showcasing the richness of themes covered in articles. Collaborative authorship patterns and temporal trends illuminated the dynamic nature of Medium's content creation over the years. The incorporation of advanced text analysis, utilizing BERT-based sentence embeddings, allowed for a deeper understanding of semantic relationships between articles.

5.2 Future Work
Advanced NLP Analysis: Exploration of sentiment analysis, topic modeling, and more advanced NLP techniques for a deeper understanding of article content.
Recommendation Systems: Implementation of sophisticated recommendation systems based on advanced text analysis for personalized content recommendations.
User Engagement Analysis: Investigation into user engagement patterns, considering factors such as reading times, claps, and comments.
5.3 Limitations
Content Scope: The analysis focuses on metadata and textual patterns, not delving into the actual content of articles.
Representativeness: While extensive, the dataset may not encompass the entire spectrum of Medium's content, potentially introducing biases.
5.4 Additional Text Analysis
BERT-Based Sentence Embeddings
The utilization of 'bert-base-nli-mean-tokens' in sentence embeddings enriches the project by:

Providing a state-of-the-art model based on the BERT architecture.
Incorporating a mean pooling layer for contextualized word embeddings.
Utilizing siamese network structures to deliver semantically meaningful sentence vectors.
Enabling advanced text analysis, including semantic similarity comparisons and more.
5.5 Webpage Extension Proposal
Considering the potential applications of advanced text analysis, an extension or app is proposed. This extension would read and preprocess data from webpages, train models on the information, and subsequently offer summaries or answer questions based on the content. Additionally, by leveraging G-API (not free), the extension could suggest websites based on pagerank similarity.
