# invasive-non_invasive-identifier
This project use Convolutional Neural Network on invasive plant species "parthenium hysterophorus" to help detect whether given plant is invasive or not.
This project implements Convolutional Neural Network using Keras to ease labelling of images.
I have used images of most common and abundant invasive plant species of India named "parthenium hysterophorus" or "carrot grass" or "Gajar ghans" in regional language.
This project will help detect invasive species by common people thus minimising precious time and efforts by scientists.
The image dataset used is self-created and you can contact me for images of "parthenium hysterophorus".

# HOW TO RUN CODE
Convolution layer, max pooling layer , flattening layer as well as fully-connected has been created in this code and could easily be spotted by following the comments.
Whereas to load images:
training_set = train_datagen.flow_from_directory('dataset/tr_set',
                                                 target_size = (64, 64),
                                                 batch_size = 32,
                                                 class_mode = 'binary')


test_set = test_datagen.flow_from_directory('dataset/t_set',
                                            target_size = (64, 64),
                                            batch_size = 32,
                                            class_mode = 'binary')
one have to change path of images accordingly in the manner....Run.py should be in the same folder where datset folder is present.
In t_set and tr_set i.e, testing and training dataset subfolder one should have images in the respective folder of the image to be labelled
i.e, I have invasive and non-invasive folder in both t_set and tr_set containing invasive and non-invasive image dataset.

Change the value of epoch accordingly.
