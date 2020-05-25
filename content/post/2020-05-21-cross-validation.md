---
title: Cross-validation gotchas
author: ~
date: '2020-05-21'
slug: cross-validation
categories: [models, statistics, machine learning]
tags: [model selection, model validation, machine learning]
description: ~
summary: "Cross-validation is elegant and simple, but that doesn't mean there aren't pitfalls."
publishDate: '2020-05-21T12:19:13-07:00'
DisableComments: no
draft: true
---

# Background

One of the most crucial aspects of a model is its ability to generalize to unseen data. A model has to learn its training data well enough to identify underlying patterns, but not learn it so aggressively that it cannot accurately predict data it has not seen before. This is the classic bias-variance tradeoff.

![Hand-drawn graph]()

Cross-validation is one technique by which a model can be evaluated on its generalizeability. To cross-validate a model, you divide your data up into a training portion, a validation portion, and ideally a test portion that goes into an impregnable vault until the very end of model development. The model is then trained on the training portion of the data (imagine that!) and asked to predict the validation set and its performance evaluated according to the metric of interest.


![Data divisions]()

In cross validation, this train-validate process is repeated many times, each time with a different training and validation set. In the end you have an average performance of this model on data it was not trained on. You can use this cross-validation performance to evaluate a model, select a model from several alternatives, or select hyperparameter values.

_K-fold cross validation_ is a commonly used variant of this procedure. In k-fold cross validation, you divide your data up into some number of "folds." One of these folds is designated as the validation set, and the rest are the training sets. You train the model on the training folds, evaluate in on the valiadtion fold, and then designate a different fold to serve as the validation fold on the next go-round.

![Folds]()

## How many folds?

# Pitfalls and gotchas
