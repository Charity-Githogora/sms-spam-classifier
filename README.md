SMS Spam Classifier – Neural Network

This project is part of the FreeCodeCamp Machine Learning with Python certification. It uses a neural network to classify SMS messages as either "ham" (not spam) or "spam", trained using the SMS Spam Collection dataset.


Project Overview

The goal of this project is to build a machine learning model that can predict whether an SMS message is spam or ham. It uses a Bidirectional LSTM neural network implemented with TensorFlow/Keras and trained on pre-split data.


What the Model Does

Tokenizes and pads input text messages

Trains on labeled SMS messages (ham/spam)

Uses a Bidirectional LSTM network for sequence understanding

Predicts a probability + label using the predict_message() function

Files Included
File	Description
SMS_Spam_Classifier.ipynb	Google Colab notebook with all the code and explanations
train-data.tsv	Training data provided by FreeCodeCamp
valid-data.tsv	Validation data provided by FreeCodeCamp
README.md	This file

How to Use It
Open the notebook in Google Colab

Run each cell in order (make sure to train the model before testing)

Use the predict_message("your message here") function to classify new SMS messages

Run the test cell to check if the model passes all test cases

Model Architecture
Embedding Layer (input_dim=1000, output_dim=32)

Bidirectional LSTM Layer (units=32)

Global Max Pooling

Dense Layer (ReLU)

Output Layer (Sigmoid)

Result
Once trained correctly, the model passes the final test and prints:

nginx
Copy
Edit
You passed the challenge. Great job!

Example Usage
python
Copy
Edit
predict_message("Congratulations! You've won a free iPhone.")
# Output: [0.91, 'spam']
👩🏽‍💻 Author
Charity Nyambura Githogora
LinkedIn • Nairobi, Kenya
Google Developer Student Club | She Code Africa

📜 License
This project follows the freeCodeCamp open-source guidelines.

