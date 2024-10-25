# Rock-Paper-Scissors
creating a convolutional neural network (CNN) model to classify images from the rock_paper_scissors dataset


# Image Resizing and Consistency:
The rock_paper_scissors images vary in size, so resizing is essential to standardize them for model input. However, only the training and test sets are resized to (32, 32). You should also resize the validation set.
Adjust the MLP model’s input shape to match the resized images as well.
# Output Layer Adjustments:
Since the dataset has only three classes (rock, paper, scissors), your output layer should have 3 neurons, not 10.
Validation Data in the CNN Model:
The CNN model currently uses the resized X_test and y_test as validation data in model.fit(). Instead, you could split the training data for a proper validation set, or use X_val and y_val.
