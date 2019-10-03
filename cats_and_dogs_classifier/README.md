# Simple classifier in Tensorflow 2.0

I wrote this notebook following the [Tensorflow tutorial](https://www.tensorflow.org/tutorials/images/classification) on classification in order to experience the new features of the 2.0 version.

That's also the reason for which I did not put too many comments in the code. If you want to better understand the concepts go directly to the official website.

By the way, the notebook shows how to classify cats or dogs from images. It builds an image classifier using a *tf.keras.Sequential* model and load data using *tf.keras.preprocessing.image.ImageDataGenerator*. It contains some interesting insights, like how to handle **overfitting** with **data augmentation** and **dropout**.

## References

- [Tensorflow Tutorial](https://www.tensorflow.org/tutorials/images/classification)
- [Install TF 2.0](https://www.tensorflow.org/install)