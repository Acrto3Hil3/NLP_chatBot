# Chatbot using NLP

## Overview
This project implements a chatbot using **Natural Language Processing (NLP)** techniques. The chatbot is designed to understand user intents and provide meaningful responses based on predefined patterns and responses. The project utilizes modern libraries for NLP, machine learning, and a user-friendly web interface for interaction.

---

## Features
- **Intent Recognition**: Identifies user intents like greetings, farewells, gratitude, and more.
- **Interactive Web Interface**: Built with Streamlit for a seamless user experience.
- **Customizable Intents**: Easily extendable `intents.json` file for adding new patterns and responses.
- **Conversation History**: Tracks and stores chat logs for future analysis or reference.
- **Scalable Design**: Built with modular code for easy maintenance and enhancements.

---

## Technologies Used
- **Python**: Core programming language for development.
- **NLTK**: Library for tokenization and text preprocessing.
- **Scikit-learn**: For machine learning model implementation.
- **Streamlit**: Framework for creating a web interface.
- **JSON**: Used for defining chatbot intents.

---

## Installation

### Prerequisites
Ensure you have the following installed on your system:
- Python 3.8 or above
- pip (Python package manager)

### Steps to Install

#### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-directory>
```

#### 2. Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

#### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

#### 4. Download NLTK Data
Run the following script to download essential NLTK data files:
```python
import nltk
nltk.download('punkt')
```

---

## Usage

### Running the Application
To start the chatbot, execute:
```bash
streamlit run app.py
```

Access the chatbot through the local web server URL provided in the terminal (usually `http://localhost:8501`).

### How to Interact
- Enter your message in the input field on the web page.
- View chatbot responses in real time.
- Check conversation history from the sidebar for past interactions.

---

## Configuration

### `intents.json`
The chatbot's logic is defined in the `intents.json` file. This file contains:
- **Tags**: Categories of user intents.
- **Patterns**: Sample inputs representing user queries.
- **Responses**: Bot replies for corresponding intents.

#### Example:
```json
{
    "tag": "greeting",
    "patterns": ["Hello", "Hi there", "Good morning"],
    "responses": ["Hi! How can I assist you today?", "Hello! What can I do for you?"]
}
```

### Conversation Logs
Chat logs are stored in a CSV file (`chat_log.csv`) in the project directory. Modify the file path in the code if needed.

---

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a new branch (`feature/your-feature-name`).
3. Make and commit changes.
4. Push to your branch.
5. Submit a pull request.

---

## Troubleshooting

### Common Issues
#### `Permission Denied` when Pushing Code
Ensure that your Git credentials are correctly configured:
```bash
git config --global user.name "YourUsername"
git config --global user.email "YourEmail"
```

#### Dependencies Not Found
Double-check that all dependencies are installed via:
```bash
pip install -r requirements.txt
```

### FAQ
**Q: How can I add new intents?**  
A: Update the `intents.json` file with new tags, patterns, and responses. Restart the application to apply changes.

**Q: Can I use this project for other languages?**  
A: Yes, modify the patterns and responses in the `intents.json` file to support your desired language.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **NLTK**: For text preprocessing and tokenization.
- **Scikit-learn**: For implementing classification models.
- **Streamlit**: For an intuitive user interface.
- **Contributors**: Thanks to all contributors for their valuable input.

---

### Replace `<repository-url>` and `<repository-directory>` with your repository's actual URL and directory name. If you’d like to adjust or refine this further, let me know!
