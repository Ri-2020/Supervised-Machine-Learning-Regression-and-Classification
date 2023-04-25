# Week 3: Classification

---

# Classification with logistic regression

> Classification is a machine learning task that **predicts a category** for input data.
> 

> It is **useful for problems** like spam detection, face recognition, or medical diagnosis.
> 

> Many classification algorithms exist, such as logistic regression, naïve Bayes, or decision trees.
> 

## Motivation

### Binary Classification

In this type of classification, the has only two options of *classes or categories*, for example, in the example below there are only two possibilities. 

| Question | Possible Answers (Classes or Category) |
| --- | --- |
| Is this email spam? | Yes / No |
| Is the transaction fraudulent? | Yes / No |
| Is the tumor malignant? | Yes / No |

******************************************************************Negative and Positive Classes******************************************************************

**0** shows negative classes and **1** shows positive classes. 

btw these choices are arbitrary.

### Question

**Which of the following is an example of a classification task?**

- Decide if an animal is a cat or not a cat.
- Estimate the weight of a cat based on its height.
****

## **Logistic regression**

Logistic regression is a statistical method used for analyzing a dataset in which there are one or more independent variables that determine an outcome. The outcome is measured with a dichotomous variable (in which there are only two possible outcomes). In logistic regression, the dependent variable is binary or dichotomous, i.e., it only contains data coded as 1 (TRUE, success, pregnant, etc.) or 0 (FALSE, failure, non-pregnant, etc.).

### Sigmoid Function

A sigmoid function is a mathematical function having a characteristic "S"-shaped curve or sigmoid curve. A common example of a sigmoid function is the logistic function shown in the first figure and defined by the formula: *(the formula which is written at the bottom of the image given below)*

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled.png)

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%201.png)

### (image) Interpretation of logistic regression output

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%202.png)

### Question

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%203.png)

## **Decision boundary**

The function g(z) gives values between 0 and 1 and when g(z) ≥ 0.5, the predicted Y is 1 and when g(z) < 0.5 the predicted Y is 0. now the value of G where the value of g(z) is 0.5 is known as decision boundary and that boundary is when z = 0.

### (image) Linear Decision Boundary

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%204.png)

### (image) Non-Linear Decision Boundaries

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%205.png)

Here the polynomial is of the order of two, we can make more complex decision boundaries using the more complex or higher order of polynomial.

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%206.png)

---

# Cost function for logistic regression

## Cost Function for logistic regression

The question arises that in ‘z’ we have got ‘w’ and ‘b’ as some parameters, how we will get that.

To get those values we need to find the squared error cost of each W and B and find the best suited.

### (image) Squared Error Cost

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%207.png)

<aside>
💡 Squared error cost function does not work in this type of problems so we use logistic loss function.

</aside>

### Logistic loss function

**if Y(i) =0**

### (image) Logistic Loss Function

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%208.png)

**if Y(i) =0**

### (image) Logistic Loss Function

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%209.png)

<aside>
💡 **So, the cost function we are using in the logistic regression is the logistic loss function.**

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2010.png)

</aside>

## Question

**Question: Why is the squared error cost not used in logistic regression?**

**Answer:** The non-linear nature of the model results in a “wiggly”, non-convex cost function with many potential local minima.

## Simplified Cost Function for Logistic Regression

the loss function can also be written as:

### (image) Simplified Loss function

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2011.png)

In the above image we can see that when Y is 1 the second term is vanished and when Y is 0 the first term of the equitation is vanished. so, the equation become similar and easier for further calculations.

### (image) Simplified cost Function

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2012.png)

---

# ****Gradient descent for logistic regression****

We will learn how to find a good choice of **W** and **B**.

### (image) Gradient Descent

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2013.png)

Although the gradient descent function looks the same for both Linear Regression and Logistic Regression, they are not,  because the definition of **F** is different in both functions.

### (image) Gradient Descent for logistic Regression

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2014.png)

But the concept is same in both the way we find the best W and B.

---

# **The problem of overfitting**

## The problem of overfitting

Overfitting is a common problem in machine learning where a model is trained too well on the training data and performs poorly on new, unseen data. This can happen when the model is too complex or when there isn't enough data for the model to generalize well. Regularization techniques, such as L1 and L2 regularization, can help prevent overfitting by adding a penalty to the loss function that discourages the model from becoming too complex.

| Fitting | Also known as |
| --- | --- |
| Underfitting | High Bias |
| Overfitting | High Variance |
| Just Right Fitting | Generalization |

### (image) The notion of overfitting and underfitting using the Regression Model

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2015.png)

### (image) The notion of overfitting and underfitting using the Classification model.

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2016.png)

## **Addressing overfitting**

### Fight Against Overfitting

1. **Collecting More training data or Training Examples** so that the model can have a variety in the data and predict more wisely.
2. **Select features to include/exclude** to use just the most appropriate features to predict the output of the model. This model also has some ***disadvantage*** like sometimes excluding important feature.
3. **Reduce the size of the parameter.** This will help to decrease the effect of the feature in the model as they have a very small impact on the model. just decrease the Wj of that feature.
    
    ![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2017.png)
    

## **Cost function with regularization**

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2018.png)

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2019.png)

<aside>
💡 We have to choose ʎ in such a way it is not too small or too big. Because if it is too small then the not impacting w’s will not get small and if it become too big then all the w’s in the equation will get very small.

</aside>

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2020.png)

## **Regularized linear Regression**

There is a **slight change in the gradient descent** equation because we have added regularization term in the equation.

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2021.png)

## **Regularized Logistic Regression**

![Untitled](Week%203%20Classification%20fd6116b6df5c418088400b35b16f2462/Untitled%2022.png)