# Image Captioning
![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)

>The main goal of this project model is to assign each pixel of an image in a category label. This network provides a complete understanding of the scene. It predicts the label, location as well as shape of each element in the image. 

###Image captioning is the process of generating textual description from an image.
The first part is handled by CNNs and the second is handled by RNNs. Use both Natural Language Processing and Computer Vision to generate the captions.

If we are told to describe this image,
![intro](https://user-images.githubusercontent.com/30392912/150976529-ae642f1a-14f6-49a0-9b49-1e778c8ae134.png)
>“মাঠের মধ্যে একটি ছেলে বল ধরে আছে ।” or “খালি গায়ে শিশুটি খুশিতে বল নিয়ে দাড়িয়ে আছে।"

While forming the description, we are seeing the image but at the same time, we are looking to create a meaningful sequence of words.

###Model
- Developing Deep Learning Model  -> Google Colab
- Generate New Captions
- Preparing Photo Data
- Preparing Text Data
	- Each photo has two described captions
- Evaluate Model

###Design Approach
- RNN + CNN
- Encoder-decoder model

###EncoderCNN
- Extract feature vector from input image
- Based on pretrained ResNet50
- Only require very small modifies
###DecoderRNN
- LSTM: Long Short Term Memory networks
- Multiple Copies of the same network
- Contained three gates to control the cell state
- Capable of learning long-term dependencies.
![Encoder-DecoderModel](img\encdr_dcdr_model.png)









[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
