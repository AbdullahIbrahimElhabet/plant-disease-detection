# plant-disease-detection
Plant Disease Detection Using Deep Learning Graduation Project

## Setup for Python:

1. Install Python ([Setup instructions](https://wiki.python.org/moin/BeginnersGuide))

2. Install Python packages

3. Install Tensorflow Serving ([Setup instructions](https://www.tensorflow.org/tfx/serving/setup))

## Training the Model

1. Download the data from [kaggle](https://www.kaggle.com/arjuntejaswi/plant-village).
2. Only keep folders related to Potatoes.
3. Run Colab 
4. Upload data to Google Drive 
4. Connect Colab to Google Drive
5. In cell #2, update the path to dataset.
6. Run all the Cells one by one.

## Deployment Model
Load the saved model: Load the model from the H5 file using a framework or library that supports deep learning, such as TensorFlow or Keras. Here's an example using TensorFlow:

python
Copy
import tensorflow as tf

# Load the model
model = tf.keras.models.load_model('saved/potato.h5')
Preprocess the input: If your model requires any specific preprocessing steps, such as resizing or normalization, make sure to apply those to the input data before passing it to the model for inference.

Perform inference: Use the loaded model to make predictions on new data. Pass the preprocessed input to the model's predict method to obtain the predictions. Here's an example:

python
Copy
# Assuming you have preprocessed input data stored in `input_data`
predictions = model.predict(input_data)


