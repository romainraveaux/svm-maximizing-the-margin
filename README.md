Maximizing the margin
===============

Often in machine learning, we introducce a parametrized distribution and we search the parameters that maximize the likelihood over some data. This can be equivalent to minimize an error function defined on the data (mean square error, mean cross entropy).

In this notebook, we describe the Support Vector Machines (SVM) Problem.
Previously we have seen that many loss functions in machine learning are related to Maximum Likelihood. 
See : 
1. Minimizing the cross entropy : a nice trip from Maximum likelihood to Kullback–Leibler divergence (http://romain.raveaux.free.fr/document/CrossEntropy.html)
2. Overfitting phenomenon of the maximum likelihood (http://romain.raveaux.free.fr/document/Overfittingbiaisedandunbiaisedvariance.html)
3 Gaussian Mixture and Expectation Maximization algorithm (http://romain.raveaux.free.fr/document/GaussianMixtureandExpectationMaximization.html)
4. Relation between the least squares error the Maximum Likelihood (http://romain.raveaux.free.fr/document/LeastSquaresError.html)

The maximum likelihood can suffer from a severe over fitting phenomenon, for instance: 
1. A data set is not well fitted by Gaussian models (under estimation of the variance)
2. In Gaussian mixture models, a Gaussian distribution can be fitted to a single data point

We have showed that the maximum likelihood can be equivalent to minimize an average error on a given data set (mean square error, mean cross entropy).

But instead of minimizing a mean error, would it be more interesting to minimize the largest error? Would it offer a better generalization property....

This is where the idea of maximizing the margin comes from ....

