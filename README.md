# Image-Captioning
Image captioning is a technology that combines LSTM text generation with the computer vision powers of a convolutional neural network.  I first saw this technology in [Andrej Karpathy's Dissertation](https://cs.stanford.edu/people/karpathy/main.pdf). Images from his work are shown in Figure 10.ACAP.

**Figure 10.ACAP: Andrej Karpathy's Dissertation**
![Captioning](https://raw.githubusercontent.com/jeffheaton/t81_558_deep_learning/master/images/karpathy_thesis.jpg "Captioning")

In this part, we will make use of LSTM and CNN to create a basic image captioning system. Transfer learning will be used to bring in these two projects:

* [Resnet50]
* [Glove]

Resnet50 is used to extract features from the images.  Glove is a set of Natural Language Processing (NLP) vectors for common words.

Figure 10.CAP-FLOW gives a high-level overview of captioning.

**Figure 10.CAP-FLOW: Captioning with a Neural Network**
![Captioning with a Neural Network](https://raw.githubusercontent.com/jeffheaton/t81_558_deep_learning/master/images/caption-1.png "Captioning with a Neural Network")

### Needed Data

You will need to download the following data and place it in a folder 

* [glove.6B] - Glove embeddings.
* [Flicker8k_Dataset](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip) - Flicker dataset.
* [Flicker8k_Text](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_text.zip)

Note, the original Flickr datasets are no longer available, but can be downloaded from [this article](https://machinelearningmastery.com/prepare-photo-caption-dataset-training-deep-learning-model/). 
We begin by importing the needed libraries.
