---
title: CNN: Image Classification
summary: A convolutional neural network (`CNN`) using the CIFAR-10 dataset to classify 32x32 colour images in 10 classes
tags:
- CNN
- Neural Network
- Data Science
date: "2020-01-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
CNN: "https://github.com/claudia-nikel/Personal_Portfolio/tree/master/CNN_Image_Classification"

image:
  caption: Photo of CNN images
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

Created a convolutional neural network using the CIFAR-10 dataset to classify 32x32 colour images in 10 classes (airplanes, automobiles. birds, horses, trucks, etc). Each layer used the ReLU activation function and the He initilization and I used a 3-block VGG model for the CNN. I plotted the accuracy and cross-entropy loss for the model with increasing number of epochs. <br/><br/>


**Plot of the Accuracy:** 
In general, models improve with more epochs of training, but only to a point and then they will start to plateau in accuracy as they converge. Originally I tried using 100 epochs but it wouldn't run on my computer. I decided to slowly increase the number of epochs and was able to run the model with 40 epochs. The red line represents the model's performance on the training dataset and the blue line represents the models performance on the test dataset. The accuracy on the test data is around 62%. <br/><br/>

**Plot of the Cross Entropy Loss:**
You can see from this graph that the model overfits the test data because the models performance on the training data (red line) decreases (so it improves) whereas on the test data (blue line) improves slightly but then increases (gets worse) around 10 epochs. <br/><br/>

**Conclusion:**
Because the images are of very low resolution that could be a cause for the misclassification and lower accuracy. As well using a higher number of epochs, say 100, would definitely give an improved result. The model was able to learn the training data, which is a good sign. To improve the results of the model on the test data, you could add more VGG blocks. However, increasing the number of epochs (the number of complete passes through the training dataset) and the number of VGG blocks requires more computer power and time. This model also shows overfitting at around 10-15 epochs. <br/> <br/>

Code for the CNN can be found here: https://github.com/claudia-nikel/Personal_Portfolio/tree/master/CNN_Image_Classification
