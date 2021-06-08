# Image recognition using Deep Forward Neural Network
# Description of the project
In this Project, we are going to work with the Fashion-MNIST dataset for image recognition. The dataset contains 10 classes of 28x28 grayscale images.

# Task 1 Load the data

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/1.png'>

# Task 2 Understand the data

Counting unique labels
array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=uint8).

There are  60000 training img and  10000 test images.

The size for each train image (28, 28)
The size for each test image (28, 28)

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/2.png'>

From the image,we can observe the image pixel values ranging from 0 to 255 & hence we need to rescale the input so input range lies between 0 to 1,upon rescaling this image & dividing each pixel by 255.

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/3.png'>

Target tester (10,) and Shape of input tester (784,). To fit the model,we need to flatten the images.

# Task 3 Construct an input pipeline

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/4.png'>




# Task 4 Construct a deep forward neural network


# Task 4.1 Setting up a model for training

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/Images/5.png'>

# Task 4.2 Fitting the model

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/6.png'>



# Task 4.3 Check the convergence through gradient

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/7.png'>



# Task 5 Fine-tuning the model

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Image%20recognition%20using%20deep%20forward%20neural%20network/9.png'>

We ran 5 experiment as shown above.Most accurate was experiment 1. As we can see,Dropout 0.3 which is experiment 1,which makes it the most accurate experiment,& experiment 5 has the least impact

