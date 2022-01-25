# Image Captioning
![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)

>The main goal of this project model is to assign each pixel of an image in a category label. This network provides a complete understanding of the scene. It predicts the label, location as well as shape of each element in the image. 

#### Image captioning is the process of generating textual description from an image.
The first part is handled by CNNs and the second is handled by RNNs. Use both Natural Language Processing and Computer Vision to generate the captions.

If we are told to describe this image,

![intro](https://user-images.githubusercontent.com/30392912/150976529-ae642f1a-14f6-49a0-9b49-1e778c8ae134.png)
>“মাঠের মধ্যে একটি ছেলে বল ধরে আছে ।” or “খালি গায়ে শিশুটি খুশিতে বল নিয়ে দাড়িয়ে আছে।"

While forming the description, we are seeing the image but at the same time, we are looking to create a meaningful sequence of words.

### Model
- Developing Deep Learning Model  -> Google Colab
- Generate New Captions
- Preparing Photo Data
- Preparing Text Data
	- Each photo has two described captions
- Evaluate Model

### Design Approach
- RNN + CNN
- Encoder-decoder model

### EncoderCNN
- Extract feature vector from input image
- Based on pretrained ResNet50
- Only require very small modifies
### DecoderRNN
- LSTM: Long Short Term Memory networks
- Multiple Copies of the same network
- Contained three gates to control the cell state
- Capable of learning long-term dependencies.

![encdr_dcdr_model](https://user-images.githubusercontent.com/30392912/150977998-eeef9d94-9562-4105-9c4b-6ec007b0e19a.png)

### Tools
![tools](https://user-images.githubusercontent.com/30392912/150977964-100257a7-9eed-4572-b3be-bf7fcc7c8312.png)

Notepad++, Avro (Bangla Writings), Flatten, Convolution2D, Dropout, LSTM, TimeDistributed, Embedding, Bidirectional, Activation, RepeatVector, Concatenate.

### Result Analysis
![result_analysis](https://user-images.githubusercontent.com/30392912/150978502-71a08dbc-6956-49e3-8942-5586212588d7.png)
![result_analysis2_with_BLEU-score](https://user-images.githubusercontent.com/30392912/150978518-85cfa309-8b94-4d19-bd6e-c4d1ccc075bf.png)

# Poster
![499B_Poster_Bangla_Image_Captioning](https://user-images.githubusercontent.com/30392912/150978544-91324bfa-fed8-4ed9-a5ea-e9b9104e03b1.png)

