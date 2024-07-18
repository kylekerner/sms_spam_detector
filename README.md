# **sms_spam_detector**
### By: Kyle Kerner

In this program we refactor code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model.  After creating a model and traing the model, the Gradio app is used to host the application and enable users to test text messages. The application provides feedback to users, indicating whether the text is classified as spam or not, based on the model's performance. 

Using the sms_text_classification_solution file we create the sms_classification function in the gradio_sms_text_classification file.  First we set the features variable to the text message column and set the target variable to the label column of the DataFrame. Next, we split the data in traing and testing and set the test_size to 33%.  Building a pipeline we transform the test data to compare to the training data.  Finally, we fit the model to the transfromed training data and retunred the model from the function. 

We loaded the SMSSpamCOllection.csv file into the DataFrame and called the sms_classification function with the DataFrame and set the result to text_clf. 

After, using the sms_prediction function to predict the classification of a new text by creating a variable of the prediction of a new text using a conditional statement. 

Lastly, using a Gradio Interface application we use inputs to determine whether the model deems a text to be spam or not spam.

# Sources
Source code provided in class as well as the use of Chat GPT to help with code direction was used in the making of the program.  