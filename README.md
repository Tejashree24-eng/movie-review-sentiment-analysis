# Movie Review Sentiment Analysis

A binary sentiment-classification project that predicts whether an IMDb movie review expresses a positive or negative opinion.

## Project overview
- Dataset: IMDb movie reviews provided by `tf.keras.datasets.imdb`
- Framework: TensorFlow / Keras
- Task: NLP text classification
- Classes: Negative (0) and Positive (1)

## Workflow
1. Load the IMDb training and test reviews.
2. Clean review text by lowercasing, removing HTML break tags and punctuation.
3. Convert text to integer sequences with Keras `TextVectorization`.
4. Train an embedding-based neural network using Embedding, Dropout, GlobalAveragePooling1D and a sigmoid output layer.
5. Evaluate the exported preprocessing-plus-model pipeline on the held-out test set.
6. Try sample reviews and inspect their predicted sentiment scores.

## Recorded result
**Test accuracy: 86.35%** (from the notebook's recorded evaluation output).

## Run
Open `movie_review_sentiment_analysis.ipynb` in Jupyter or Google Colab and run the cells in order. The first run downloads the IMDb dataset through Keras, so internet access is needed for that download.

## Dependencies
See [requirements.txt](requirements.txt).

## Notes
This is an educational NLP project. Results may vary with library versions, random seeds and runtime environment.
