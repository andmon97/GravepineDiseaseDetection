# Gravepine Disease Detection

This was an exercise to try how Transfer Learning work for a simple Computer Vision task.

In this exercise we classify the gravepine lead into 4 classes (to detect if there is a disease or not):
1) Black Rot disease;
2) Esca disease;
3) Blight leafe disease;
4) Healthy.



## Data used

I used this [dataset](https://www.kaggle.com/datasets/piyushmishra1999/plantvillage-grape) hosted on Kaggle.



## Model Used

I used [MobileNetV2](https://arxiv.org/abs/1801.04381) trained on [Imagenet](https://www.image-net.org/) as base model, used as feature extractor.
The top layers, are classic fully connected layers that make the multi-class classification.

With this configuration, I reached 98% of validation accuracy  in very few epochs. See the notebook for more info.
