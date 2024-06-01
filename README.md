# SMS Spam Detector

SMS Spam Detector is a simple Python script that checks whether a given message is spam or not. It utilizes machine learning techniques to classify messages based on their content.

## Installation

Clone the repository:

   ```
   git clone https://github.com/Aditya-Ranjan1234/SMS_Spam_Detector.git
   ```

## Usage

To use the SMS Spam Detector, follow these steps:

1. Prepare your message data.
2. Enter the message you want to classify in the end of jupyter notebook.
3. The script will output whether the message is spam or not.

Example:

```
# Enter SMS Message
sms = 'Aft i finish my lunch then i go str down lor. Ard 3 smth lor. U finish ur lunch already?'

transformed_sms = tfidf.transform([transform_text(sms)]).toarray()

for name,clf in clfs.items():
    
    answer=clf.predict(transformed_sms)  
    print("For ",name)
    print("Result",answer)

    if(answer[0]==0):
        print("ham")
    else:
        print("spam")
```

## Dataset

The SMS Spam Detector is trained on the [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) available from the UCI Machine Learning Repository. This dataset contains a collection of SMS messages that are labeled as spam or ham (not spam).

## Dependencies
Python 3.x
pandas
numpy
scikit-learn 
Installation

## Credits

This code was originally created by CampusX (@campusx-official).
Many lines of code have been added and modified.
