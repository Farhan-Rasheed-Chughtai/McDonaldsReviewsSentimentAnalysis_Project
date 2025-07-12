Overview:

This project aimed to analyze customer reviews from McDonald’s stores across the U.S. using natural language processing (NLP) and machine learning techniques. The goal was to extract sentiment insights, identify regional trends, and evaluate performance over time to help McDonald's improve customer experience.

Dataset & EDA:

Source: Kaggle dataset of 33,000 Google reviews from 39 stores across 26 cities and 11 states.
Key features: Reviewer ID, store name, address, location coordinates, review text, rating (1–5 stars).

EDA revealed:

Equal proportion of 5-star and 1-star reviews.
Florida had the highest number of reviews.
Best and worst-rated stores were distributed mostly along the East and West coasts.

Low-Risk Goals (Location & Sentiment Analysis):

Calculated average ratings by city and state:

Best-rated city: Annadale.
Worst-rated cities: Miami Beach, Salt Lake City.
Worst states: Florida and Utah.

Created word clouds:

Positive reviews emphasized “service,” “food,” and “fast.”
Negative reviews highlighted “rude,” “bad,” “drive,” and “order,” indicating service quality was a major driver of sentiment.
Suggested improvements should focus on staff attitude and delivery speed, especially in low-performing locations.

Medium-Risk Goals (Sentiment Classification Models):

Converted ratings into three classes:

Negative (1–2), Neutral (3), Positive (4–5)
Trained five models: Logistic Regression, Random Forest, MultinomialNB, BernoulliNB, SVC
Random Forest performed best but struggled with neutral sentiment (low recall).

Used BERT embeddings to enhance model input:
Significantly improved classification performance, especially for neutral reviews.

High-Risk Goals (Time-Series Analysis):

Attempted to identify trends in ratings over time.
Found increasing ratings from 2017 to 2020.
Significant decline post-2020, likely due to COVID-19 impact on service and operations.
ARIMA-based forecasting failed due to uneven time distribution in the data.
Recommendation: McDonald's should invest in improving online and drive-through services, which may have driven the post-2020 decline.
