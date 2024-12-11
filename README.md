Chatbot using NLP

Overview

This project implements a chatbot using Natural Language Processing (NLP) techniques. The chatbot is designed to understand user intents and provide appropriate responses based on predefined patterns and responses. It utilizes the nltk library for natural language processing, scikit-learn for machine learning, and streamlit for creating an interactive web interface.

Features

Dynamic Intent Recognition: Understands user intents such as greetings, farewells, gratitude, and more.

Customizable Responses: Provides relevant responses based on user-defined intents in the intents.json file.

Interactive Web Interface: Built using streamlit for an easy-to-use chatbot interface.

Conversation History Tracking: Maintains a conversation log in a CSV file for future reference.

Extensible Architecture: Easily add new intents or customize the chatbot's behavior.

Technologies Used

Programming Language: Python

Libraries:

nltk for natural language processing tasks like tokenization and stemming.

scikit-learn for training machine learning models.

streamlit for building the chatbot's web interface.

json for defining intents and their patterns and responses.

Installation

1. Clone the Repository

git clone <repository-url>
cd <repository-directory>

2. Create a Virtual Environment (Optional but Recommended)

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. Install Required Packages

pip install -r requirements.txt

4. Download NLTK Data

import nltk
nltk.download('punkt')

Usage

To run the chatbot application, execute the following command:

streamlit run app.py

Once the application is running, you can interact with the chatbot through the web interface. Type your message in the input box and press Enter to see the chatbot's response.

Intents Data

The chatbot's behavior is defined by the intents.json file, which contains various tags, patterns, and responses. This file allows you to customize the chatbot by:

Adding new intents.

Modifying existing intents.

Defining more patterns and responses for each intent.

Sample intents.json format:

{
    "intents": [
        {
            "tag": "greeting",
            "patterns": [
                "Hi",
                "Hello",
                "Hey",
                "Good morning",
                "Good evening"
            ],
            "responses": [
                "Hello! How can I assist you today?",
                "Hi there! What can I do for you?",
                "Hey! How can I help?"
            ]
        },
        {
            "tag": "goodbye",
            "patterns": [
                "Bye",
                "See you later",
                "Goodbye",
                "Take care"
            ],
            "responses": [
                "Goodbye! Have a great day!",
                "See you soon!",
                "Take care! Bye!"
            ]
        }
    ]
}

Conversation History

The chatbot saves the conversation history in a CSV file (chat_log.csv). This feature is useful for analyzing past interactions and improving the chatbot's responses. You can view the conversation history by selecting the "Conversation History" option in the sidebar.

Project Structure

NLP_chatBot/
├── app.py               # Main application script for running the chatbot
├── intents.json         # JSON file defining chatbot intents
├── chat_log.csv         # File to store conversation history
├── requirements.txt     # List of dependencies
├── README.md            # Project documentation
└── other_files/         # Additional scripts and resources

Future Enhancements

Advanced NLP Techniques: Incorporate deep learning models like RNNs or Transformers for better intent recognition.

Multilingual Support: Enable the chatbot to understand and respond in multiple languages.

Contextual Understanding: Improve the chatbot's ability to handle multi-turn conversations.

Integration with APIs: Enhance the chatbot's capabilities by integrating external APIs (e.g., weather, news).

Contributing

Contributions to this project are welcome! If you have suggestions for improvements or features, feel free to open an issue or submit a pull request. Please ensure that your contributions align with the project's goals and follow coding best practices.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments

NLTK for natural language processing.

Scikit-learn for machine learning algorithms.

Streamlit for building the web interface.

Replace <repository-url> and <repository-directory> with the actual URL of your repository and the name of the directory where the project is located. Adjust any sections as necessary to better fit your project's specifics.
