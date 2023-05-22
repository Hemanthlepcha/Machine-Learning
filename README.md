# Machine-Learning
This one my first project based on machine learning where i have built a sequential model which classifies the emotion ( Binary classification)
## how to run this project?
To load and use a saved model in Keras, you can use the `load_model()` function from the `keras.models` module. Here's an example code snippet to load a saved `.h5` file and make predictions on new data:

```python
import tensorflow as tf
from keras.models import load_model

# Load the saved model
model = load_model('path/to/saved/model.h5')

# Make predictions on new data
yhat = model.predict(np.expand_dims(resize/255,0))

# Do something with the predictions
if yhat < 0.5:
    print("Image you have entered is feeling happy")
else:
    print("Image you have entered is feeling low, Help them :-(")
```

In the above code, `new_data` represents the data on which you want to make predictions. The `predict()` method of the loaded model can be used to make predictions on new data. You can then use the predictions for further processing as per your requirements.

Note that when loading the saved model, it's important to use the same version of TensorFlow and Keras that were used to train and save the model.
