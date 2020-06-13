# Image-Captioning
Image Captioning with Keras and TensorFlow
Image captioning is a technology that combines LSTM text generation with the computer vision powers of a convolutional neural network. I first saw this technology in Andrej Karpathy's Dissertation. Images from his work are shown in Figure 10.ACAP.

Figure 10.ACAP: Andrej Karpathy's DissertationCaptioning

In this part, we will make use of LSTM and CNN to create a basic image captioning system. Transfer learning will be used to bring in these two projects:

[Resnet50]
[Glove]
Resnet50 is used to extract features from the images. Glove is a set of Natural Language Processing (NLP) vectors for common words.

Figure 10.CAP-FLOW gives a high-level overview of captioning.

Figure 10.CAP-FLOW: Captioning with a Neural NetworkCaptioning with a Neural Network

We begin by importing the needed libraries.

Needed Data
You will need to download the following data and place it in a folder

[glove.6B] - Glove embeddings.
Flicker8k_Dataset - Flicker dataset.
Flicker8k_Text
Note, the original Flickr datasets are no longer available, but can be downloaded from this article.
