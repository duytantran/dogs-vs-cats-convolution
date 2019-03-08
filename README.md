# Image Recognition
We are given a huge dataset, which can be found from Kaggle, with dog and cat pictures. By applying the deep learning technique convolutional neural networks, we can recognize cats vs dogs. We are using 10'000 images to train a good model. We don't have any good rule of thumbs, but more images will give a better accuracy. Organize your pictures in a dataset folder with subfolders training_set and test_set, and this solution can be reused. 

Since we have a binary outcome, we use the sigmoid function and binary cross-entropy loss function. If there are more than 2 outcomes, use softmax and categorial cross-entropy loss function. Used the Keras documentation a lot: https://keras.io/ . Especially the ImageDataGenerator, under Image Preprocessing, to avoid overfitting. Recommended to use as guideline!

Started with a single convolutional layer, which gave an accuray ~75%. This was immensely improved after adding a second one, which gave an accuracy of 85% for the training set and 82% for the test set! The accuracy can of course be increased by adding more layers, and/or increasing the target_size and input_shape dimensions. In my case, I used 64, but if you have a GPU and a lot of coffee, go for it!
BEWARE: the input_shape parameter is only run once in the Convolution2D function. 

The CNN model, step by step:
* Step 1: Convolution
* Step 2: Max Pooling
* Step 3: Flattening
* Step 4: Full Connection

This can also be applied to more general problems, for instance classifying different brain tumors.  
As a final note, we can of course use R to build a CNN with the H2O package, with the framework Deep Water. However, this framework is still in the early stages, and it is advisable to use Python for Deep Learning with their amazing libraries.
