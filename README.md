# Word-Embedding

## Introduction

We experiment how to obtain a Embedding Matrix, by creating a simple Movie Review Sentiment Classifier which achieved 83% accuracy.

## Model

It was trained with TensorFlow build-in "imdb", which is a movie review database for binary sentiment classification.
imdb supplies a set of 25,000 highly polar movie reviews for training, and 25,000 for testing.

A byproduct of the classifier is an "Embedding Matrix",
which has vocabulary size 10,000 and dimension 16.

<img src="https://github.com/yuhang2685/Word-Embedding/blob/main/model.png" width="55%">

## Performance

The simple classifier achieves 83% accuracy.

<img src="https://github.com/yuhang2685/Word-Embedding/blob/main/MovieReview-Accuracy.png" width="35%">

## Visualization of Embedding

We visualized it with Google Embedding Projector.

<img src="https://github.com/yuhang2685/Word-Embedding/blob/main/embedding-imdb.png" width="35%">
