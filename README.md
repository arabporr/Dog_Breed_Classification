# Dog Breed Classification

## Introduction
This project was my first project in Udacity's AI programming nano degree. We used pre-trained models such as ResNet, VGG, Alexnet, and our own designed architecture to check if an image is a picture of a dog and then recognize its breed.

## Usage
The input images should be:
In jpeg format with extension jpg.
In approximately square in shape (their height and width are approximately the same numbers of pixels).
If you want to check the accuracy, name the files like this: Animal_Name_01.jpg or Object_Name_01.jpg

Then Put all images you want to classify in the uploaded_images folder, open a terminal window in the project directory and type the following, then hit enter:
```
sh run_models_batch_uploaded.sh
```

To do this, you will be calling the following shell script that will output the following results files:
resnet_uploaded-images.txt - that contains the results using CNN model architecture ResNet
alexnet_uploaded-images.txt - that contains the results using CNN model architecture AlexNet
vgg_uploaded-images.txt - that contains the results using CNN model architecture VGG

## Results
In this project, we had two main objectives:
Identifying which pet images are of dogs and which pet images aren't of dogs
Classifying the breeds of dogs, for the images that are of dogs

In the table below, you will find our results for each of the model architectures.

For objective 1, notice that both VGG and AlexNet correctly identify images of "dogs" and "not-a-dog" 100% of the time.
For objective 2, VGG provides the best solution because it classifies the correct breed of dog over 90% of the time.

![Results Table]()

Given our results, the "best" model architecture is VGG. It outperformed both of the other architectures when considering both objectives 1 and 2. You will notice that ResNet did classify dog breeds better than AlexNet, but only VGG and AlexNet were able to classify "dogs" and "not-a-dog" at 100% accuracy. The model VGG was the one that was able to classify "dogs" and "not-a-dog" with 100% accuracy and had the best performance regarding breed classification with 93.3% accuracy.
