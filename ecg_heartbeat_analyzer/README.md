# ECG Heartbeat classification
My initial goal was that to classify entire ecg signals to detect possible defects, but I ran into trouble finding some nice dataset I want to work with.
Finally I found [**this one**](https://www.kaggle.com/shayanfazeli/heartbeat) on Kaggle and even if it contains "only" heartbeats I decided to use it, just for fun and to learn something new.

![ecg](https://images.ecosia.org/GRTFxzVdgx0izZCAuB_GPNjy_eg=/0x390/smart/http%3A%2F%2Fa-fib.com%2Fwp-content%2Fuploads%2F2012%2F08%2FSchematic-diagram-of-normal-sinus-rhythm-for-a-human-heart-as-seen-on-ECG-Wikipedia-free-to-use.png)

The dataset contains classic csv files with all numerical values. However, to make the things a bit different, I decided to take every heartbeat (i.e. a row in the csv file) and transform it into an image, using **CV2** library.
After obtaining all the images I need (I stopped the execution at ~22000, only for time reason), I trained a simple **CNN** with **Keras**.

##### An image generated from the data and used to train the CNN:
![example](https://image.ibb.co/nsTXz9/0_21763.png)

### Dataset
https://www.kaggle.com/shayanfazeli/heartbeat

### References
- [Keras Image Classifier](https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html)