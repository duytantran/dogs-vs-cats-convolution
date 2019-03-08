# Classifying dog and cat pictures
We are given a huge dataset, which can be found from Kaggle, with dog and cat pictures. By applying the deep learning technique convolutional neural networks, we can seperate cats vs dogs. We are using 10'000 images to train a good model. We don't have any good rule of thumbs, but more images will give a better accuracy. Organize your pictures in a dataset folder with subfolders training_set and test_set. 

Since we have a binary outcome, we use the sigmoid function and binary cross-entropy loss function. If there are more than 2 outcomes, use softmax and categorial cross-entropy loss function. Used the Keras documentation a lot: https://keras.io/ . Especially the ImageDataGenerator, under Image Preprocessing, to avoid overfitting. Recommended to use as guideline!

The CNN model, step by step:
* Step 1: Convolution
* Step 2: Max Pooling
* Step 3: Flattening
* Step 4: Full Connection

This can also be applied to more general problems, for instance classifying different brain tumors. 
