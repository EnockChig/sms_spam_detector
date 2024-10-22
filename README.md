# sms_spam_detector

SMS Spam Classification with SVC Model
This project refactors an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model. The model is trained to classify text messages as "spam" or "not spam" and is deployed using Gradio to provide an interactive interface. Users can input text messages to test the model, and the application will provide real-time feedback on whether the message is classified as spam or not.

Project Files
The following starter files are included in the project:
gradio_sms_text_classification.ipynb: 
This notebook contains the Gradio interface setup and the function for SMS classification.
sms_text_classification_solution.ipynb: This notebook contains the original solution code for SMS classification.
SMSSpamCollection.csv: The dataset containing labeled SMS messages for training and testing.

Project Overview
1. SMS Classification Function
The main function, sms_classification, is implemented in gradio_sms_text_classification.ipynb.
It uses the SMSSpamCollection.csv dataset to classify SMS text messages as either "ham" (not spam) or "spam".

Key Steps:

Feature Selection: The text messages are used as the feature, and the target variable is set to the "label" column ("ham" or "spam").
Data Splitting: The dataset is split into training and testing sets, with 33% of the data reserved for testing.
Model Construction: A linear Support Vector Classification (SVC) model is created and trained on the training set.

Classification Logic:
If the message is classified as "ham", the function returns:
The text message: "{text}", is not spam.
If the message is classified as "spam", the function returns:
The text message: "{text}", is spam.

2. Gradio Interface
The application is hosted on Gradio to create an interactive user interface. Users can input text messages, and the model will classify the input as "spam" or "not spam" and provide feedback based on the classification result.

3. Model Training
The model is trained on the provided dataset, which contains SMS messages labeled as either "ham" or "spam". After training, the model's performance is evaluated on the test set, and the application is ready for deployment using Gradio.

Instructions

Open the gradio_sms_text_classification.ipynb notebook.
Ensure that all dependencies are installed, including Gradio, pandas, scikit-learn, etc.
Load the SMSSpamCollection.csv dataset.
Train the SVC model by splitting the data into training and testing sets.
Test the model using the Gradio interface by running the notebook.
Input your own text messages to see if they are classified as spam or not.

Dependencies

Make sure the following Python libraries are installed:

gradio
pandas
scikit-learn
numpy
Running the Application

To run the SMS classification application:

Launch the gradio_sms_text_classification.ipynb notebook.
Follow the instructions in the notebook to train the model and start the Gradio interface.
Input an SMS text into the Gradio UI, and the model will classify it as spam or not spam.

Example Output:
Input: "Win a free iPhone now!"

Output: The text message: "Win a free iPhone now!", is spam.

Input: "Hey, are we still on for lunch?"

Output: The text message: "Hey, are we still on for lunch?", is not spam.

Conclusion

This project provides a hands-on implementation of a linear SVC model to classify SMS messages. By using Gradio, it enables users to interact with the model in real time, making it a practical tool for identifying spam messages.








