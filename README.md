
# TalentScout Hiring Assistant Chatbot

## Project Overview
The TalentScout Hiring Assistant is an interactive chatbot built to assist candidates in applying for tech positions. The chatbot collects candidate details, such as name, contact information, tech stack, and experience. It then generates relevant technical questions based on the candidate’s declared tech stack using the **Google Gemini API**.

Additionally, the assistant supports **multilingual** interactions, allowing candidates to interact in their preferred language. The app also includes **sentiment analysis** to gauge the candidate's response.

## Installation Instructions

### 1. Install required libraries
Make sure you have the following libraries installed:
- `google-generativeai`
- `streamlit`
- `googletrans`
- `textblob`
- `pyngrok`

To install these dependencies, run:

```bash
pip install google-generativeai streamlit googletrans==4.0.0-rc1 textblob pyngrok
```

### 2. Set up your Google API key
You need a Google API key for interacting with **Google Gemini**. Replace `YOUR_GOOGLE_API_KEY` in the code with your actual API key.

### 3. Running the Streamlit App
To run the app:

```bash
streamlit run /path/to/hiring_assistant.py
```

This will start the app and provide you with a URL to access the chatbot.

## Usage Guide

1. **Select Language**: Choose your preferred language from the available options (English, Tamil, Telugu, Kannada, Malayalam, Hindi).
2. **Provide Candidate Details**: Enter your full name, email, phone number, years of experience, desired position, and current location.
3. **Tech Stack Declaration**: Specify your tech stack, including programming languages, frameworks, and tools.
4. **Receive Technical Questions**: Based on your tech stack, the assistant will generate relevant technical questions to assess your proficiency.
5. **Sentiment Analysis**: The assistant will perform sentiment analysis of the questions to gauge the emotional tone of the interaction.
6. **Multilingual Support**: All interactions are translated into the selected language.
7. **End the Conversation**: At any time, you can end the conversation, and the assistant will thank you for participating.

## Technical Details

- **Backend**: Google Gemini API (for generating technical questions)
- **Frontend**: Streamlit (interactive UI)
- **Sentiment Analysis**: TextBlob
- **Translation**: Googletrans

## Prompt Design

- The assistant generates technical questions by sending a prompt to **Google Gemini API** with the candidate’s tech stack. 
- The assistant provides translated prompts for tech stack declaration and displays technical questions in the selected language.
