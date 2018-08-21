---
title: "Probabilistic Machine Learning"
abstract: "In this talk we review the *probabilistic* approach to machine learning. We start with a review of probability, and introduce the concepts of probabilistic modelling. We then apply the approach in practice to Naive Bayesian classification. 

In this lecture we review the Bayesian formalism in the context of linear models, reviewing initially maximum likelihood and introducing basis functions as a way of driving non-linearity in the model."
ipynb: 2018-08-25-probabilistic-machine-learning.ipynb
reveal: 2018-08-25-probabilistic-machine-learning.slides.html
author:
- family: Lawrence
  given: Neil D.
  gscholar: r3SJcvoAAAAJ
  institute: Amazon Cambridge and University of Sheffield
  twitter: lawrennd
  url: http://inverseprobability.com
date: 2018-08-25
venue: AI Saturdays, Lagos
transition: None
---

\include{talk-macros.tex}

\include{_ml/includes/what-is-ml.md}
\include{_ml/includes/probability-intro.md}
\include{_ml/includes/probabilistic-modelling.md}

### INTRODUCE DATASET EARLIER. HERE!

\include{_ml/includes/graphical-models.md}
\include{_ml/includes/classification-intro.md}
\include{_ml/includes/classification-examples.md}
\include{_ml/includes/bayesian-reminder.md}
\include{_ml/includes/bernoulli-distribution.md}
\include{_ml/includes/bernoulli-maximum-likelihood.md}
\include{_ml/includes/bayes-rule-reminder.md}
\include{_ml/includes/naive-bayes.md}

### Other Reading

* Chapter 5 of @Rogers:book11 up to pg 179 (Section 5.1, and 5.2 up to 5.2.2).

### References