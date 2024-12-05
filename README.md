# Fashion - Neural Network

## Scenario
You are part of a team at an online clothing retailer that aims to create an automated system for categorizing new clothing items as they are introduced to the inventory. The product management team should simply upload an image of a new clothing piece, and the system will generate a suitable category for that item, which can then be linked to its database entry. This categorization will enhance the shopping experience by making it easier for customers to locate the items they desire in the online store.

To achieve this, you have access to a substantial collection of existing product images that have already been categorized and processed. This dataset will serve as the foundation for training a convolutional neural network (CNN) to effectively classify new product images. Once the model demonstrates satisfactory performance, it will be ready for deployment in a live environment.

**Data Sources:**

- [Fashion MNIST Dtatset](https://keras.io/api/datasets/fashion_mnist/)
  

            
| LABEL | DESCRIPTION |
|-------|-------------|
| 0     | T-shirt/top |
| 1     | Trouser     |
| 2     | Pullover    |
| 3     | Dress       |
| 4     | Coat        |
| 5     | Sandal      |
| 6     | Shirt       |
| 7     | Sneaker     |
| 8     | Bag         |
| 9     | Ankle boot  |


        


## Project Goals
The objective is to create a system that automatically categorizes new clothing items..


Several questions will be asked:

- What happens to the layer sizes as the model approaches the final outputlayer?
- How accurate is the model's performance?
- What is the moel's loss?
- What insights can you share regarding the inaccurate predictions? Considering human perspective, is it reasonable that images could be categorized incorrectly as they have been?
- What strategies could you employ to retrain this CNN model and enhance its performance?




#### Why use a Convolutional Neural Network algorithm to predict the outcome?
1. A conventional multi-layer perceptron (MLP) neural network connects every neuron in one layer to all neurons in the adjacent layers, making it effective for a variety of tasks with diverse input types. However, this architecture struggles with image processing, which can limit its performance in visual applications.

2. One significant drawback of traditional neural networks is the necessity to convert a two-dimensional image into a one-dimensional vector before inputting it into the network. This flattening process can lead to the loss of essential information, particularly the spatial relationships that exist between individual pixels, which are crucial for understanding images.

3. In contrast, convolutional neural networks (CNNs) utilize a unique structure that allows for partial connections between neurons through convolutional layers. This design is inspired by human vision, where each neuron responds to a specific area of stimuli, gradually building a more intricate representation of the image as the data progresses through the network. As a result, CNNs are particularly well-suited for tackling challenges in computer vision, effectively processing complex, pixel-rich images.


## Data
A dataset that can be used to train the machine-learning model has been found. This is dataset of a dataset of 60,000 28x28 grayscale images of 10 fashion categories, along with a test set of 10,000 images..

## Conclusions
TBD...