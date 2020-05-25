---
date: "2020-03-01T19:47:09+02:00"
description: Predicting product recalls from consumer safety complaints.
jobDate: 2020
projectUrl: https://github.com/katherinemwood/insight
techs:
- python
- scikit-learn
- pandas
- seaborn
- streamlit
- AWS
thumbnail: precall/alert.png
title: PRecall
work:
- machine learning
- natural language processing
- logistic regression
---

Unsafe or defective products cost over a trillion dollars each year in deaths, injuries, property damage, and lost productivity. It's imperative that consumers be able to avoid unsafe products, but it's currently extremely difficult to find relevant information about recalls or complaints about products.

Using recall announcements and consumer complaints filed to the CPSC, I developed an app that surfaces information related to a product. A consumer can search for a product and receive all the related complaints about that product. If it's been recalled, they also receive the recall notice. If it hasn't been recalled, they get a prediction of the recall probability based on the other complaints about that product.