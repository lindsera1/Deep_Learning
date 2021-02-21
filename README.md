# Deep_Learning

## Overview and Purpose

In this project, we sought to help Alphabet Soup, a philanthropic organization, determine how their resources could be best placed in order to make the greatest
impact. In other words, which companies are too high risk, and which are promising? After deciding noticing the complexity of the data, we thought using a 
neural network that was more powerful and able to handle complex data could more easily handle this task. So with this in mind, we set out to solve the 
classification problem at hand.

## Results

We created a multilayered neural network known as a deep neural network, to evaluate over 34,000 organizations that Alphabet Soup has given to in the past. We 
looked at factors ranging from application type, to money put up front. 

### Data Preprocessing

+ The targets for our model were the successful organizations that Alphabet Soup funded. We wanted to know what made these succeed?
+ The features we're all the other variables. Everything from classifcation, to application type, income, etc was weighted by our model to determine the proper
classification of data points.
+ Some features were rather noisy and did not contribute to the overall story the data was trying to tell, like Affiliation. We omitted this data so as to give
 our model a clearer picture.
### Compiling, Training, and Evaluating the Model

+ Our best performing model had two layers, 8 neurons each layer, and used selu and sigmoid activation functions. We used binary crossentropy and adam optimizers
to help reduce loss and increase performance.

+ While we did not reach the marked 75% goal, we did reach approximately 71%; depending on who you ask, this could be sufficient. 

+ To increase the performance of the initial model, I tweaked the input data to remove those affiliation columns, and I added three more neurons to the second 
layer. I also changed the activation functions for each layer from relu to selu. Below is a picture of the performance metrics of our model.

![model-performance](https://github.com/lindsera1/Deep_Learning/blob/main/Screen%20Shot%202021-02-21%20at%201.08.54%20AM.png)

## Summary:

The overall results were a .704 percent accuracy. After multiple tweaks, and a few attempts, I decided to go with our best attempt for sake of time constraints; 
however, with a little more research, I believe I could have changed a few of the parameters to help it perform better. I think Alphabet Soup would be happier
with 20% more predictability than random chance when it comes to funding the organizations they care about.
