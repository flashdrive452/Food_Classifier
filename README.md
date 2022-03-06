# Food_101_Classifier
An image classification neural network trained to classify 10 food classes. (Work is currently on-going to upscale to 101 food classes)

We started by downloading a zipped dataset of two food classes (pizza and steak).
We created a function to view random images from both classes. This enabled us to understand the data we were about to model.

We commenced our modelling experiments by stacking 4 convolutional neural network (layers) on each other.
This model utilized the Binary CrossEntropy as the loss function with an Adam optimizer.

Training this model for 5 epochs yielded a validation accuracy of 77%.

We upscaled to 10 food classes and unzipped the new dataset.

We built a transfer learning model using the efficientNetB0 feature extractor.
The loss function and optimizer used was Categorical CrossEntropy and Adam respectively.

This model achieved a validation accuracy of 90%.

We reviewed various evaluation metrics for all 10 classes: f1-score, recall and precision.
We also exposed some wrong labels by visualizing some of our predictions using the Matplotlib library.
