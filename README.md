# faces-mtl
Multi Task Learning example with Keras

Multitask learning is powerful when the tasks could benefit from having
shared low-level features. For example predicting the age and gender
are different tasks, one being regression and the other being
classification. However, solving these tasks simultaneously makes the
network learn better low-level representations of the face than solving
these taks separately.

Here we use cropped face image data set from
[https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/](https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/). Each image is preprocessed to be of same size.

We have used Functional API of Keras to implement multi-output neural
network. we have a cross entropy loss for the gender output and RMSE
for age output.

Below is the model architecture.

<img src="model.png" alt="drawing" width="200" height="500"/>

All code and documentation is present in the jupyter notebook. Contact
[gr-arcrecipes@wpi.edu](mailto:gr-arcrecipes@wpi.edu) for questions.
