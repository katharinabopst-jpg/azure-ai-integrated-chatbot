# Azure AI-Integrated Student Support Chatbot

This project was developed for **MSAI 631: Artificial Intelligence for Human-Computer Interaction** at the University of the Cumberlands.

## Project Overview

This project extends a traditional rule-based student support chatbot by integrating **Microsoft Azure AI Language**. The chatbot combines deterministic Python rules with cloud-based sentiment analysis to demonstrate a hybrid approach to conversational artificial intelligence.

## How It Works

The system uses two components:

1. **Traditional rule-based chatbot logic** identifies topics such as assignments, deadlines, office hours, contact information, and study tips.
2. **Azure AI Language sentiment analysis** analyzes each user message and classifies its sentiment as positive, neutral, negative, or mixed.

The chatbot uses the Azure sentiment result to adapt the tone of its rule-based response.

**Architecture:**  
User Input → Azure AI Language Sentiment Analysis → Rule-Based Topic Detection → Sentiment-Aware Response

## Technologies

- Python
- Google Colab
- Microsoft Azure AI Language
- Azure AI Text Analytics Python SDK
- GitHub

## Azure AI Integration

The project uses the **Free F0 tier** of Azure AI Language. Sentiment analysis returns both a sentiment classification and confidence scores for positive, neutral, and negative sentiment.

## Security

Azure credentials are **not stored in the source code**. The API key is entered securely at runtime using Python's `getpass()` function. This prevents the Azure API key from being exposed when the notebook is shared through GitHub.

## Testing

The chatbot was tested with:

- Positive user input
- Negative user input
- Neutral user input
- Unsupported input
- Empty input
- Exit commands

Testing demonstrated successful communication between the Python chatbot and Azure AI Language while preserving the chatbot's traditional rule-based response logic.

## Project File

`Azure_AI_Integrated_Chatbot_Project.ipynb`

## Author

Katharina Bopst  
University of the Cumberlands  
MSAI 631: Artificial Intelligence for Human-Computer Interaction
