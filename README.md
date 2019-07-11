The book "Deep Learning", Goodfellow et al descirbe transfer learning as a "Situation where what has been learned in one setting is exploited to improve generalization in another setting". Basically it is a machine learning method where a model developed for some task is used as the starting point for a model on a second task.

It is a widely used approach in deep learning where pre-trained models are used as the starting point on computer vision and natural language processing tasks, as it takes a large amount of time and resources to train and develop these neural network models. Using a pre-trained models helps give a huge boost in predictions as these models would have already seen huge amounts of data in their respective training sets.

To put this method to test, we will use the MNSIT dataset to do the following:

 1. Create a model to and train it to learn digits from 0-4 in the MNIST dataset.
 2. Test its performance on digits 0-9.
 3. Freeze the layers from in the model to retain the trained weights that the model has learnt from training on 0-4 digits.
 4. Add new layers to this model and train on digits 5-9 and test its performace.
 5. Test its performance on digits 0-9.

We will do this using two approaches:

 - Using a fully connected dense layered model
 - Using a CNN model
