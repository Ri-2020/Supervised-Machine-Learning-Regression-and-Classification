# Week 2: Regression With Multiple Variable

# Table of Content

---

# Multiple Linear Regression

## Multiple Features

Multiple linear regression is an extension of simple linear regression, allowing us to model relationships between several independent variables and a dependent variable. In this way, we can capture more complex relationships and make more accurate predictions. However, it becomes more difficult to interpret the model's coefficients when we have multiple features.

******************Notation****************** 

- $**X_j =  jth**$  feature
- **n** = number of features
- $x^i =$  feature of ith training example (this is not a number it is vector or array of features value )
- $x^i_j$ = value of feature j in ith example

in this type of equation, we use more than one W 

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled.png)

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%201.png)

## **Vectorization**

It will make our code shorter and easy to understand.

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%202.png)

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%203.png)

<aside>
💡 using ******np. dot(w,x)****** is after during computation then using the for loop without it vectorization works differently than for loop it a way lot smarter to compute the dot products so it saves a lot of time

</aside>

so, using numpy vectorization is a lot better choice instead of using the for loop

## **Gradient descent for multiple linear regression**

Same as the previous gradient descent just a little addition of → sign on the vector form of w and x

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%204.png)

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%205.png)

---

# ****Gradient descent in practice****

## Feature Scaling Part 1 and 2

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%206.png)

When the possible value of the feature is big, or the **range is big** in that case the ****W**** is ********associated with that attribute will be **smaller** and if the **range is small** then the ****W**** associated with the will be **relatively bigger**, so that the line fit is good. 

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%207.png)

### There are two ways to scale

******************************************Normal Normalization:****************************************** Divide the attribute by the highest value  ************************************************************************************

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%208.png)

******Mean Normalization :****** subtract the average from the attribute and divide it by the subtract range.

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%209.png)

********************************Z-score normalization:******************************** subtract the attribute with the mean and divide it by standard deviation. 

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%2010.png)

too Larger or too smaller the range of a feature more rescaling is required.

## Checking Gradient Descent for Convergence

### Learning Curve

Basically learning curve is a graph between the j value and number of iterations

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%2011.png)

### Choosing a learning rate

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%2012.png)

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%2013.png)

Use 0.001 as alpha and then increase it by roughly 3X (three times) and check for best alpha that is just right for the example.

## **Feature engineering**

Using intuition to design new features, by transforming or combining original features.

Choosing the most significant features for the algorithm to perform best is known as feature engineering.

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%2014.png)

### Question

if you have measurements for the dimensions of a swimming pool (length, width, height), which of the following two would be a more useful engineered feature?

Ans : Volume

## Polynomial Regression

![Untitled](Week%202%20Regression%20With%20Multiple%20Variable%20ceb0cbbab20b48c898f43a07d3da77ee/Untitled%2015.png)