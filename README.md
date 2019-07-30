# Image-Captioning-Model


Algorithm that uses transfer learning as its basic mechanism to train an Automatic Image Captioning Model.

Basically, it uses Flickr8k dataset to train the model.
It contains 8000 images from which 6000 of them used for training and the other 2000 split equally
for evaluating the model.

The final model contains two submodels.
The first one has the responsibility of extracting every possible feature from the training dataset. The algorithm
that used for that kind of job is Inception V3, a pretrained algorithm in ImageNet dataset.
The second one, given as an input the feature exctraction output from the first submodel and with the combination of Recurrent Neural Networks and
techinques of predicting the next word in a sequence such as Argmax and Beam Seach, it is capable of producing captions from
different points of view that captures the meaning of the image.
