# ai-powered-qa
A question-answering chatbot powered by the RoBERTa model, capable of providing contextual answers and searching Google for information.
Welcome to the ROBERTa Question Answering Chatbot with Google Integration!

This project implements a question-answering chatbot using the pre-trained RoBERTa model from Hugging Face's Transformers library. It can answer questions based on a provided context. If the answer is not found in the context, the chatbot attempts to find relevant information by searching Google.

## Features

* **Contextual Question Answering:** Answers questions directly from a given text context using the RoBERTa model (`deepset/roberta-base-squad2`).
* **Google Search Integration:** When an answer is not found in the provided context, the chatbot uses Google Search to find relevant information.
* **Interactive Chatbot Loop:** Allows users to have a continuous conversation with the chatbot.
* **Dynamic Context Update:** Users can set or update the context for the chatbot during the session using the command `set context: your context here`.

## Prerequisites

* **Python 3.6 or higher**
* **pip installed**

## Installation

1.  Clone this repository (if you haven't already):
    ```bash
    git clone <your_repository_link>
    cd <your_repository_directory>
    ```
    *(Remember to replace `<your_repository_link>` and `<your_repository_directory>` with your actual link and directory.)*
2.  Install the required Python libraries:
    ```bash
    pip install transformers torch googlesearch-python
    ```
    * `transformers`: For using the RoBERTa pre-trained model.
    * `torch`: PyTorch framework required by the Transformers library.
    * `googlesearch-python`: For performing Google searches. You might need to install it specifically as `pip install google-search-python`.

## How to Run the Chatbot

1.  Save the provided Python code as a `.py` file (e.g., `chatbot.py`).
2.  Run the script from your terminal:
    ```bash
    python chatbot.py
    ```
3.  The chatbot will start, and you can begin asking questions.

## Usage

* **Ask a question:** Simply type your question and press Enter. The chatbot will first try to find the answer in the initial context or any context you have set.
* **Set the context:** To provide a specific context for the chatbot to answer from, use the command `set context: your context here`. Replace `your context here` with the actual text context.
* **Exit the chatbot:** Type `exit` and press Enter to end the conversation.

## Example Interaction
