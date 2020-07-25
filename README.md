# Mobile-Apps-using-TensorFlow-Lite-and-Android-Studio
Implement two mobile apps on Android phones using Tensorflow Lite

## Description
Steps to implement two mobile apps on Android phones
-	Classify plants : this app is adapted from the tensorflow codelabs tutorial [Recognize Flowers with TensorFlow Lite on Android](https://codelabs.developers.google.com/codelabs/recognize-flowers-with-tensorflow-on-android/#0)

-	Transfer learning: App to apply transfer learning to a picture taken with your mobile. This is a tensorflow Lite app example from the following [tensorflow repo](https://github.com/tensorflow/examples/tree/master/lite/examples/style_transfer/android). For other examples, you can check what is available [here](https://www.tensorflow.org/lite/examples)

## Dependencies
-	Google Colab
-	Android Studio installed on the PC

## Implementation
-	Plant Classifier: Follow instructions from tensorflow tutorial “Recognize Flowers with TensorFlow Lite on Android”
    - I modified the classifier by a plant classification.
    - I used a pre-trained plant classifier available on tensorflow hub and using MobileNet architecture. This model is trained to recognize **2101 plants species** from images.
    - The model converted to tfl can be found [here](https://tfhub.dev/google/aiy/vision/classifier/plants_V1/1). This allows to skip the training of a model and conversion steps.
    - I adjusted the list of labels in the provided text file. The original labels can be found [here]( https://www.gstatic.com/aihub/tfhub/labelmaps/aiy_plants_V1_labelmap.csv)
    
-	Style transfer: Follow instructions from github tensorflow repo [here](https://github.com/tensorflow/examples/tree/master/lite/examples/style_transfer/android)
