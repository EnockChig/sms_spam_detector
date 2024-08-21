# sms_spam_detector

Refactoring code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model, model is created and trained. Hosted on Gradio to use the application, enabling users to test text messages. The application will provide feedback to users, indicating whether the text is classified as spam or not, based on the model's performance.


Challenge Instructions
The starter files consist of the following files: gradio_sms_text_classification.ipynb, sms_text_classification_solution.ipynb, and SMSSpamCollection.csv.

Create the SMS Classification Function
The sms_classification function in the gradio_sms_text_classification.ipynb was created by setting the features variable to the text message column of the DataFrame and setting the target variable to the "label" column of the DataFrame.

Data was split into training and testing and the test_size set to 33%.

Model uses a conditional statement that determines if the text message is "ham" or “spam”. If the message is “ham”, the function should return the following message: f'The text message: "{text}", is not spam.'

If the message is spam, the function should return the following message: f'The text message: "{text}", is spam.'

