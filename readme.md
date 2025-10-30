# Enhanced Q&A Chatbot

A lightweight question-answer web app built using **Streamlit**, **LangChain**, and **OpenAI models**.  
It allows you to type any question, select a model, tune parameters like temperature and token limit, and get clear text responses — all from a simple browser interface.

---

## 🧩 Overview

This project is designed to interact with large language models through an easy-to-use interface without writing repetitive code.  
The app combines a conversational prompt pipeline with Streamlit’s layout features to provide a minimal but functional Q&A chatbot.

---

## ⚙️ How It Works

1. **User Input:**  
   The user enters a question into the text box on the main screen.

2. **Model Configuration:**  
   In the sidebar, you can:
   - Enter your OpenAI API key securely
   - Choose the model (`gpt-4o`, `gpt-4-turbo`, or `gpt-4`)
   - Adjust temperature (controls randomness)
   - Set the maximum number of tokens (controls response length)

3. **Prompt Processing:**  
   The app uses a `ChatPromptTemplate` from LangChain to format the question and pass it to the selected model.

4. **Response Generation:**  
   The output is processed through `StrOutputParser` and displayed in real time in the Streamlit interface.

---

## 🧠 Core Components

| Component | Description |
|------------|-------------|
| `Streamlit` | Handles the web interface, sidebar controls, and real-time updates. |
| `LangChain` | Manages the message template, model connection, and output parsing. |
| `dotenv` | Loads environment variables from `.env` (optional, for local setup). |
| `OpenAI` | Provides the text generation models for answering questions. |

---


