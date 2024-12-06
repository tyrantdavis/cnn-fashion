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

- What strategies could be employ to retrain this CNN model and enhance its performance?




#### Why use a Convolutional Neural Network algorithm to predict the outcome?
A conventional multi-layer perceptron (MLP) neural network connects every neuron in one layer to all neurons in the adjacent layers, making it effective for a variety of tasks with diverse input types. However, this architecture struggles with image processing, which can limit its performance in visual applications.

One significant drawback of traditional neural networks is the necessity to convert a two-dimensional image into a one-dimensional vector before inputting it into the network. This flattening process can lead to the loss of essential information, particularly the spatial relationships that exist between individual pixels, which are crucial for understanding images.

In contrast, convolutional neural networks (CNNs) utilize a unique structure that allows for partial connections between neurons through convolutional layers. This design is inspired by human vision, where each neuron responds to a specific area of stimuli, gradually building a more intricate representation of the image as the data progresses through the network. As a result, CNNs are particularly well-suited for tackling challenges in computer vision, effectively processing complex, pixel-rich images.


## Data
A dataset that can be used to train the machine-learning model has been found. This is dataset of a dataset of 60,000 28x28 grayscale images of 10 fashion categories, along with a test set of 10,000 images..

## Conclusions

- What happens to the layer sizes as the model approaches the final output layer?
    - The size of each layer appears to diminish as the final output layer(dense network) is approached.  
- How accurate is the model's performance?
    - 89% 
- What is the moel's loss?
    - .032

- What insights can you share regarding the inaccurate predictions? Considering human perspective, is it reasonable that images could be categorized incorrectly as they have been?
    - In the last two instances of misclassification, the clothing items predicted by the model appeared quite similar to their actual counterparts. For instance, the image located in row 6, column 1 was identified as a shirt, yet it is actually a coat. The resemblance between a shirt and a coat is notable, and upon viewing the image, one might struggle to spot the distinction. On the other hand, the first misclassification (row 5, column 4) is significantly off the mark. The model labeled this image as a sandal, but it is unmistakably a type of boot, specifically an ankle boot.
- What strategies could be employ to retrain this CNN model and enhance its performance?
    - Adjusting the dimensions of the convolutions and the size of their filters could contribute to creating a more proficient model. Since precise values for these hyperparameters might not be available, it could be beneficial to try out various combinations to discover what yields the best outcomes. 