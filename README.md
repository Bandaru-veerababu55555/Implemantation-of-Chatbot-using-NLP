# Implemantation-of-Chatbot-using-NLP

## Overview
This project implements a chatbot using Natural Language Processing (NLP) techniques. The chatbot is designed to understand user intents and provide appropriate responses based on predefined patterns and responses. It utilizes the `nltk` library for natural language processing, `scikit-learn` for machine learning, and `streamlit` for creating an interactive web interface.

---

## Features
- Understands various user intents such as greetings, farewells, gratitude, and more.
- Provides relevant responses based on user input.
- it containes specigic Data guide for Data Analyst
- Maintains a conversation history that can be viewed by the user.
- Built using Python and leverages popular libraries for NLP and machine learning.

---

## Project Structure
```base
chatbot-nlp/
│
├── chat_bot.png               # Contains training user interface image
├── hello.txt                  
├── intents.json               # contains intents Data
├── Chat_log.csv            # contains chat log history
├── app.py                  # Streamlit app script
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation

```
---

## Technologies Used
- **Python**
- **NLTK**
- **Scikit-learn**
- **Streamlit**
- **JSON** for intents data

---

## Installation

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-directory>
```

### 2. Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install Required Packages
```bash
pip install -r requirements.txt
pip install streamlit
pip install pandas
pip install numpy
pip install nltk
```

### 4. Download NLTK Data
```python
import nltk
nltk.download('punkt')
```

---

## Usage
To run the chatbot application, execute the following command:
```bash
streamlit run app.py
```

Once the application is running, you can interact with the chatbot through the web interface. Type your message in the input box and press Enter to see the chatbot's response.

---

## Intents Data
The chatbot's behavior is defined by the `intents.json` file, which contains various tags, patterns, and responses. You can modify this file to add new intents or change existing ones.

```bash
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": ["Hello", "Hi", "Greetings"],
      "responses": ["Hello! How can I help you?", "Hi there!"]
    },
    {
      "tag": "goodbye",
      "patterns": ["Bye", "See you"],
      "responses": ["Goodbye! Take care.", "See you soon!"]
    }
  ]
}

```
---

## Extending the Chatbot
- Modify the' intents.json' file in the 'data/ 'folder to add new patterns and responses.
- Update the logic in 'src/intent_classifier.py' or 'src/response_generator.py' for more advanced behavior.
---

## Conversation History
The chatbot saves the conversation history in a CSV file (`chat_log.csv`). You can view past interactions by selecting the "Conversation History" option in the sidebar.

---

## Contributing
Contributions are welcome! Please create a pull request with detailed explanations of your changes.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **NLTK** for natural language processing.
- **Scikit-learn** for machine learning algorithms.
- **Streamlit** for building the web interface.

---

