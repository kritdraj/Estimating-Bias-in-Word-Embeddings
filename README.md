# Estimating-Bias-in-Word-Embeddings

The aim of the project is to replicate the results of the paper "A Transparent Framework for Evaluating Unintended Demographic Bias in Word Embeddings", Chris Sweeney et al. by following the framework outlined.

The paper proposes a transparent framework to evaluate the unintended bias in word embeddings and a metric to measure fairness of the models through the relative negative sentiment associated with neutral identity terms. The paper restricts the definition of bias to un-equal distributions of negative sentiment among demographic identity terms in word embeddings and aims to identify the bias in the embedding models that might lead to unfair downstream NLP systems. 

To isolate the unidentified bias, the paper uses the idea that neural identity terms that are associated with more negative sentiment words will be classified like their neighboring sentiment words, hence exhibiting some bias. To achieve this, a set of unbiased labeled words' word embeddings are extracted to train a model to predict the negative sentiment probability of any given neutral identity term. 

As an extended experiement, a set of LGBTQ+ identity terms and words are tested in the same way, to evaluate the unintended bias of these models for these terms.
