# Notes on Extending Prior Correction to Multinomial Logit Models

Prior correction is a method used to correct predictions made from a logistic regression model when oversampling was used to create the training dataset. Essentially, we use information about the marginal distribution of the target before and after oversampling to correct modeled predictions as if we had built the model on the pre-sampled data.

These notes extend the method to multinomial logistic regression and propose a method to estimate the full density of the prior distribution when only a subset of levels have assigned prior probabilities.