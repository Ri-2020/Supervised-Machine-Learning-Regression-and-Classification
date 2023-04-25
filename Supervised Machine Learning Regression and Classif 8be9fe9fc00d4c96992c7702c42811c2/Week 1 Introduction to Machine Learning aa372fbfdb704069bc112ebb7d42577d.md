# Week 1: Introduction to Machine Learning

# Table of contents

---

# Overview of Machine Learning

## State of AI

The **State of AI Report** analyses the most interesting developments in AI. We aim to trigger an informed conversation about the state of AI and its implication for the future.

[State of AI Report 2022](https://www.stateof.ai/)

*AI has the market of 20Trillion Dollars by 2030*

---

# ****Supervised vs. Unsupervised Machine Learning****

## Machine Learning

> Field of study that gives computer the ability to learn without explicitly programmed
-**Arthur Samuel (1959).**
> 

## Types of machine learning

### **Supervised Learning**

Supervised learning ****is a type of machine learning in which *the algorithm learns to make predictions based on labeled data.* The algorithm is trained on a dataset that includes both input data and the corresponding output data. The goal of the algorithm is to learn a function that can map inputs to outputs, so that it can make accurate predictions on new, unseen data.

Some common applications of supervised learning include image classification, speech recognition, and natural language processing.

It is used most in real-world applications. It has seen most rapid advancements

### **Unsupervised Learning**

Unsupervised learning is a type of machine learning in which *the algorithm learns to identify patterns and relationships in data without being given explicit labels.* The algorithm is trained on a dataset that includes only input data, and the goal is to identify underlying structures and groupings in the data.

Some common applications of unsupervised learning include clustering, anomaly detection, and dimensionality reduction.

### **Recommender System**

Recommender systems are a type of machine learning algorithm that is used to recommend items to users based on their past behavior, preferences, and other data. These systems are commonly used in e-commerce and content delivery applications, where they help users discover new products or content that they are likely to be interested in. There are several different types of recommender systems, including content-based systems, collaborative filtering systems, and hybrid systems that combine multiple approaches.

### **Reinforcement Learning**

Reinforcement learning is a type of machine learning that involves an agent learning to make decisions in an environment in order to maximize a reward signal. The agent interacts with the environment by selecting actions, and receives feedback in the form of rewards or penalties. The goal of the agent is to learn a policy that will maximize its cumulative reward over time. Reinforcement learning has been successfully applied to a variety of tasks, including game playing, robotics, and autonomous driving.

## Supervised Machine Learning

Supervised learning ****is a type of machine learning in which *the algorithm learns to make predictions based on labeled data.* The algorithm is trained on a dataset that includes both input data and the corresponding output data. The goal of the algorithm is to learn a function that can map inputs to outputs, so that it can make accurate predictions on new, unseen data.

Some common applications of supervised learning include image classification, speech recognition, and natural language processing.

It is used most in real-world applications. It has seen most rapid advancements

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled.png)

********Let’s get a more specific example********

We can use regression to estimate the price of a House. **********************Regression********************** predict a number infinitely many possible output.

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%201.png)

### Classification Algorithm

Classification algorithms are a type of machine learning algorithm that is used to predict the class of an input data point. The input data is classified into one of several predefined classes based on its features. Some common applications of classification algorithms include spam filtering, sentiment analysis, and image classification. Some popular classification algorithms include decision trees, support vector machines, and logistic regression.

Opposite to regression it predict a small finite number.

## Unsupervised Machine Learning

Unsupervised machine learning is a type of machine learning in which the algorithm learns to identify patterns and relationships in data without being given explicit labels. Unlike supervised learning, there is no output or target that the algorithm is trying to predict. Instead, the algorithm is tasked with finding structure or patterns in the input data on its own. Some common applications of unsupervised learning include clustering, anomaly detection, and dimensionality reduction.

### Clustering Algorithm

Clustering algorithms are a type of unsupervised machine learning algorithm that are used to identify groups, or clusters, within data. The algorithm examines the input data and groups together data points that are similar to each other based on some metric, such as distance or similarity. Some common applications of clustering algorithms include customer segmentation, image segmentation, and anomaly detection.

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%202.png)

### Anomaly Detection

Anomaly detection is a technique used to identify data points that deviate from the norm or expected pattern. It is commonly used in fraud detection, intrusion detection, and system health monitoring. Dimensionality reduction is a technique used to reduce the number of features or variables in a dataset while retaining as much of the original information as possible. This can help to simplify the data and make it more manageable, while also reducing the risk of overfitting and improving the performance of machine learning algorithms.

### Dimensionality reduction

Dimensionality reduction is a technique used to reduce the number of features or variables in a dataset while retaining as much of the original information as possible. This can help to simplify the data and make it more manageable, while also reducing the risk of overfitting and improving the performance of machine learning algorithms. Some common techniques for dimensionality reduction include principal component analysis (PCA), t-distributed stochastic neighbor embedding (t-SNE), and linear discriminant analysis (LDA).

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%203.png)

---

# Regression Model

## Linear Regression Model

Linear Regression Model is a type of supervised learning algorithm that is used to predict a continuous output variable based on one or more input variables. The model uses a linear function to approximate the relationship between the input variables and the output variable, and can be used for both simple and multiple regression problems. The goal of the algorithm is to find the best-fit line that minimizes the difference between the predicted values and the actual values in the training data.

![It is a type of supervised learning model known as Regression model that predicts number](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%204.png)

It is a type of supervised learning model known as Regression model that predicts number

<aside>
💡 There is one other model in supervised learning known as Classification model that predict categories for example by looking an image it can tell if the image is cat or dog.

</aside>

## Terminology

- ************************Training Set:************************ The data which is used to train the model.
    - **************************Notation:**************************
        - **************************“*x*” :** Variable and also known as ********feature********
        - ******“*y*” : Target** or **output** variable
        - ******“*y-hat(^)*” : Estimated** output value
        - **“*m*” :** Total **number of training examples**
        - ****( *x , y* ) :** single training example
        - ****( *x$^i$ , y$^i$* ) :** Tells the i$^t$$^h$ index of single training example
        - ************f**** :** is known as function that takes ******x****** as input and return ***y-hat*** as output

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%205.png)

## Lab(optional): Model Representation

[Machine-Learning-Specialization-Coursera/C1_W1_Lab03_Model_Representation_Soln.ipynb at main · greyhatguy007/Machine-Learning-Specialization-Coursera](https://github.com/greyhatguy007/Machine-Learning-Specialization-Coursera/blob/main/C1%20-%20Supervised%20Machine%20Learning%3A%20Regression%20and%20Classification/week1/Optional%20Labs/C1_W1_Lab03_Model_Representation_Soln.ipynb)

---

## Cost Function Formula

[Cost Functions [6 types] (opengenus.org)](https://iq.opengenus.org/cost-functions-in-machine-learning/#:~:text=What%20are%20different%20types%20of%20cost%20functions%3F%201,3.%20N%20is%20the%20total%20number%20of%20observations.)

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%206.png)

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%207.png)

### Cost Function: Squared error cost function

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%208.png)

**Our main goal is to minimize the cost.**

### Question

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%209.png)

## Cost Function Intuition

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2010.png)

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2011.png)

## Visualizing the cost function

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2012.png)

This graph is generated when the cost function depend on both W and B 

we can visualize this graph in 2D in which we have some rings in which the smallest ring will have the minimum possible J(w,b)

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2013.png)

---

# ****Train the model with gradient descent****

## Gradient Decent

Gradient descent is an optimization algorithm that is commonly used to train machine learning models. The goal of gradient descent is to find the values of the model's parameters that minimize a cost function. The algorithm works by iteratively adjusting the parameters in the direction of the steepest descent of the cost function. This process continues until the algorithm converges to a minimum of the cost function, at which point the model's parameters are considered to be optimized.

### Outline

- Start with some w,b (set w =0, b = 0)
- Keep Changing w,b to reduce j(w,b)
- Until we settle at or near a minimum

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2014.png)

## **Implementing gradient descent**

 = is not mathematics = it is assignment operator in any programming language means it assigns the value.

In the equation,, alpha means how big the step we are taking to the next cost

and other term is the derivative term telling in which direction you need to take the baby step

we Simultaneously update the new W and B 

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2015.png)

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2016.png)

## Learning Rate $(alpha)$

ALPHA should not be too small

- If the W is at the local minima it will not change later more.

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2017.png)

- As we reach near to the local minima the slope will decrease and the change in W will keep decreasing. and as the minima become 0 the change in W will also become 0

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2018.png)

## Gradient descent for linear regression

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2019.png)

### Convex function

A convex function is a function that does not have any local minima it only has one global minima.

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2020.png)

## Running Gradient Descent

![Untitled](Week%201%20Introduction%20to%20Machine%20Learning%20aa372fbfdb704069bc112ebb7d42577d/Untitled%2021.png)

### Batch Gradient Descent

Each step of gradient descent uses all the training examples not a subset of the data.