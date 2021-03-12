### What's in this repo

This repo contains this README and my previous notebooks. The data was too large to include and there is an external link provided below.


### External packages used


Since I'm not sure what packages you have installed, I will link to resources on all the packages that were used in this package.


Efficient Net: https://keras.io/api/applications/efficientnet/
MatPlotLib: https://pypi.org/project/matplotlib/
NumPy: https://pypi.org/project/numpy/
TensorFlow: https://www.tensorflow.org/install/pip
requests: https://pypi.org/project/requests/


### Data Source

The following link leads to the full dataset:

https://data.mendeley.com/datasets/tywbtsjrjv/1

In this project, I chose only to use the tomato images. This dataset can be found here:


https://drive.google.com/drive/folders/1gmjIk6JbsijxJ6zA_CZzWEtfMGuQA5vW?usp=sharing


### Executive Summary


    What is your goal?

My goal is to develop a convolutional neural network that can classify tomato plant disease based on images of the repspective plant's leaf.

    What are your metrics?

My metrics are train loss and accuracy and test loss and accuracy.

    What were your findings?

The model that I built was able to beat the baseline score, but there is improvement to be made.

    What risks/limitations/assumptions affect these findings?

One risk is that I am not very proficient with neural networks so it's difficult for me to diagnose and effectiely mitigate errors.

A big limitation is my computing power. To date, I have not been able to use GPUs on GCP or AWS to speed up the model testing process.

An assumption that would affect these findings is that a production model would not be able to look at each leaf in teh way the leaves are looked at tin the data. So, without removing leaves and taking pictures of them individually, this model would not be practical.



### Implementation, Evaluation, and Inference


    implementation

The model I used was a convolutional neural net built in Keras.

    evaluation

To date, the highest epoch accuracy my model reached was 0.9. However, 0.9 was treached with very sporadic validation loss and accuracy. After more tests, this number is more realistic around 0.7. This score still beats the baseline (0.295) and would require more knowledge of neural networks and better processing pwoer to improve.

    inference

The conclusion I can draw from this information is that it is possible to classify leaves based on image, but I need more experience and better udnerstanding of neural networks to improve the accuracy.



### Sources used

Throughout this project I used multiple resources to develop code. They are listed below:

https://www.tensorflow.org/tutorials/images/classification

https://keras.io/api/optimizers/adam/

https://www.youtube.com/watch?v=Sq_cYIlm_pM