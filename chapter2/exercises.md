# Conceptual
## Question 1
### Part a
Flexible. With a large sample size and a low prediction count, you have a lot of information to train a flexible method. The few number of predictors leads to a lower risk of overfitting the data. 

### Part b
Since you don't have many observations, choosing a inflexible method would provide you with better results as more information is stored in the model itself. 
### Part c
If this relationship between predictors and response is highly non-linear, a flexible method might be able to fit these abnormal relations better with enough data. 
### Part d
Non-flexible. High variance in error terms means that a flexible method may attempt to overfit to these errors. Sticking with a non-flexible method will have a greater chance of underaccounting for these errors. That being said, if the underlying real-world relation is more complicated, a non-flexible model would fail to capture these relationships.  

## Question 2
### Part a
Regression; Inference; n = 500, p = 4
### Part b
Classification; Prediction; n = 20, p = 14
### Part c
Regression; Prediction; n = 52, p = 4

## Question 3
### Part a
![bias_variance_tradeoff](bias_variance_tradeoff.jpg)
### Part b
typical (squared) bias - bias is the error introduced by approximating a real world problem with a simple model. less flexible models introduce more error as they struggle to approximate highly complex problems. for this reason, the graph starts high. as the models become more flexible, the error they introduce due to oversimplication decreases.

variance - for less flexible models, the variance is extremely low as changes to the training data don't have a very strong effect on the underlying model. however, as flexibility increases, the effect that changes in training data have on a single data point increase due to the model having less information within itself.

training error - as model flexibility increases, the output of the model will more closely match the training data leading to it decreasing over time

test error - although training data decreases as model flexibility increase, after a certain point (where variance starts rising), overfitting will happen and the test error will begin to increase with model flexibility

Bayes (irreducible) error - the bayes irreducible error is always the same. irreducible error is constant and is not affected by model flexibility

## Question 4
### Part a
1. detecting spam or not spam emails. response would be boolean. predictors would be certain words or sentence structures. goal - prediction. 
2. coin sorter machine. repsonse would be 'quarter', 'penny', 'dime', 'nickel', 'half-dollar', 'dollar'. predictors would be the images. goal - prediction.
3. plant species identifier. response would be distinct plant types. predictors would be images of the plant. goal - prediction
### Part b
1. Home selling price. response would be price. predictors would be num rooms, bathrooms, location, etc. goal - prediction.
2. energy consumption. response would be kwh. predictors would be location, weather, num of people. goal could be inference or prediction
3. factory output. response would be number of items. predictors would be staff count, product, materials. goal - inference, what elements affect the production rate
### part c
1. city planning based on where populations are located.
2. earthquake locations to approximate fault locations
3. *todo*

## question 5
very flexible:
- advantages:
  - able to model more complex real world problems
- disadvantages:
  - more apt to overfit a simple problem if not enough data is present
less flexible:
  - not enough data can lead to underfitting
- advantages:
  - for simple real world problems with fewer data points, you can more easily model them with a lower risk of over fitting
- disadvantages:
  - no matter how much data is given, cannot model more complex / nonlinear real world problems

a more flexible approach would be preferred if the underlying problem is nonlinear, complex, large sample size, with a small number of predictors. on the other hand, a less flexible approach would be preferred if there is a small sample size, large predictor count or simpler model (prevents overfitting)

## question 6
a parametric approach utilizes a model with parameters and makes some assumptions of what the shape of the model is. a non-parametric approach makes no assumptions about the underlying model and therefore can be follow more complex problems. parametric advantages are that inference becomes easier its simpler to understand a parametric model for a real world scenario. 

## question 7
### part a
1. sqrt(0 + 9 + 0) = 3
2. sqrt(4 + 0 + 0) = 2
3. sqrt(0 + 1 + 9) = sqrt(10) ~3.16
4. sqrt(0 + 1 + 4) = sqrt(5) ~2.23
5. sqrt(1 + 0 + 1) = sqrt(2) ~1.41
6. sqrt(1 + 1 + 1) = sqrt(3) ~1.73
### part b
Green, observation 5 is the closest
### part c
Red, observation 2, 5, and 6 are the closest. 2 and 6 are red
### part d
the best value would be a smaller K. this is because high values of K would lead to using too many data points to guess the test which is almost like overfitting.