# Word-Embedding

## Introduction

We experiment how to obtain a Embedding Matrix, by creating a simple Movie Review Sentiment Classifier which achieved 83% accuracy.

## Model

It was trained with TensorFlow build-in "imdb", which is a movie review database for binary sentiment classification.
imdb supplies a set of 25,000 highly polar movie reviews for training, and 25,000 for testing.

A byproduct of the classifier is an "Embedding Matrix",
which has vocabulary size 10,000 and dimension 16.

```
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
embedding_1 (Embedding)      (None, 120, 16)           160000    
_________________________________________________________________
conv1d (Conv1D)              (None, 116, 128)          10368     
_________________________________________________________________
global_average_pooling1d (Gl (None, 128)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 6)                 774       
_________________________________________________________________
dense_3 (Dense)              (None, 1)                 7         
=================================================================
Total params: 171,149
Trainable params: 171,149
Non-trainable params: 0
_________________________________________________________________
```

## Performance

The simple classifier achieves 83% accuracy.

<img src="https://github.com/yuhang2685/Word-Embedding/blob/main/MovieReview-Accuracy.png" width="30%">

## Visualization of Embedding

We visualized it with [Google Embedding Projector](https://projector.tensorflow.org/).

<img src="https://github.com/yuhang2685/Word-Embedding/blob/main/embedding-imdb.png" width="25%">
