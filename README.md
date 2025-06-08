# AI-CHATBOT-WITH-NLP

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: MOOLISWATHI

*INTERN ID*: CT04DN1447

*DOMAIN*: PYTHON PROGRAMMING

*DURATION*: 4 WEEKS 

*MENTOR*: NEELA SANTOSH

DESCRIPTION: Chatbot Using NLTK in Python
This Python program is a basic rule-based chatbot created using Natural Language Toolkit (NLTK), a powerful library used for working with human language data (text). The chatbot is designed to understand simple user queries and provide suitable responses based on predefined patterns. The project demonstrates how Natural Language Processing (NLP) can be used to create interactive programs that respond to user inputs in a conversational manner.

 How It Works
The chatbot uses pattern matching to recognize user inputs. It checks if the user’s message contains specific keywords or phrases, and if it matches a predefined pattern, it provides a relevant answer. If the input does not match any pattern, it responds with a default message like “Sorry, I don’t understand that. Can you rephrase?”

The logic is implemented using the Chat and reflections classes from the nltk.chat.util module. These classes allow developers to create simple rule-based chatbots by defining a list of input-output pairs.

 Main Components of the Code
1. Importing Libraries
The script begins by importing necessary modules from NLTK:

python
Copy
Edit
import nltk
import random
import string
from nltk.chat.util import Chat, reflections
Here, Chat is used to create the conversation engine, and reflections is a built-in dictionary that automatically maps words like “I” to “you”, “am” to “are”, etc., to make the responses sound more natural.

2. Downloading NLTK Data
The following lines are used to download the required NLTK data files:

python
Copy
Edit
nltk.download('punkt')
nltk.download('wordnet')
These resources support tokenization and lemmatization, though they are not used directly in this version but are necessary for some NLTK features if you choose to expand the bot later.

3. Defining Chat Pairs
The pairs list contains tuples. Each tuple has two elements:

A regular expression pattern to match user input.

A list of responses the bot can choose from randomly.

For example:

python
Copy
Edit
[
    r"(.*)(your name|who are you)(.*)",
    ["I am a chatbot created using NLTK!", "You can call me NLTKBot."]
]
This pattern checks if the user's input contains phrases like “your name” or “who are you”.

4. Main Function
The main() function sets up and starts the chatbot:

python
Copy
Edit
def main():
    print("Hi! I'm your NLP Chatbot. Type 'quit' or 'bye' to exit.")
    chatbot = Chat(pairs, reflections)
    chatbot.converse()
The Chat object is initialized with the pairs list and reflections dictionary. Then the converse() method starts an interactive loop where the bot keeps reading user input and responding until the user types “bye” or “quit”.

 Running the Chatbot
To run this chatbot:

Save the code in a file named chatbot_nltk.py.

Open the terminal or command prompt.

Run the command: python chatbot_nltk.py.

You can now chat with the bot by typing messages and getting responses.

Example interaction:

vbnet
Copy
Edit
> hello
Sorry, I don't understand that. Can you rephrase?

> what is your name?
I am a chatbot created using NLTK!
 Features
Rule-based interaction using regex.

Predefined responses for basic questions.

Reflection for more human-like replies.

Easy to extend and customize.

 Future Improvements
This chatbot is simple, but it can be extended in many ways:

Use spaCy or transformers for more intelligent NLP.

Add intent detection using machine learning.

Store conversation history.

Integrate with GUI or web applications.

 Conclusion
This project gives a beginner-friendly introduction to creating a chatbot using NLTK. It covers the basics of pattern matching, input handling, and generating responses. Although it is not AI-powered, it helps understand how early chatbots worked and lays the foundation for more complex conversational agents.

##OUTPUT

![Image](https://github.com/user-attachments/assets/7035103c-79c1-494b-b475-f5e7bed4bf3d)
