# Conversational AI Assistant with Langchain & Langgraph

This repository presents a foundational Python project for building a conversational AI assistant using the Langchain and Langgraph frameworks. The `main.py` script sets up a reactive agent that can interact with users, providing a versatile base for various AI-powered applications.

## 📂 Files in This Repository

* `main.py`: The core Python script that initializes and runs the AI assistant.
* `.env`: A file for securely storing environment variables like API keys (e.g., `OPENROUTER_API_KEY`).

## 🎯 Objective

The primary objective of this project is to demonstrate the setup of a basic, extensible AI conversational agent. It serves as a starting point for developers to build more complex AI assistants by integrating custom tools and enhancing conversational capabilities.

## 🧰 Tools & Technologies Used

* **Python 🐍**: The primary programming language for the project.
* **Langchain**: A powerful framework for developing applications powered by large language models.
* **Langgraph**: A library built on Langchain for constructing robust and stateful multi-actor applications with LLMs.
* **OpenRouter.ai**: Utilized for accessing various large language models, specifically configured for `mistralai/mistral-7b-instruct` in this example.
* **`python-dotenv`**: Employed for efficient and secure management of environment variables.

## 🧪 Key Analysis Performed (Implicit in Project Setup)

While this project is primarily an application setup, its design implicitly addresses key aspects of conversational AI system development:

1.  **Agent Initialization and Configuration**: Demonstrates the process of setting up a `ChatOpenAI` model with specific configurations (e.g., `mistralai/mistral-7b-instruct` via OpenRouter.ai API).
2.  **Reactive Agent Architecture**: Showcases the use of `langgraph.prebuilt.create_react_agent` to enable dynamic reasoning and response generation based on user input.
3.  **Tool Integration Design**: Although no tools are actively enabled in the provided `main.py`, the commented-out `calculator` and `say_hello` functions, and the `tools = []` placeholder, illustrate the mechanism for integrating external functionalities into the agent. This highlights the extensibility of the architecture.
4.  **Interactive Loop for User Input**: Implements a continuous loop to accept user queries and stream responses from the agent, demonstrating a basic conversational flow.
5.  **Environment Variable Management**: Utilizes `python-dotenv` for secure handling of API keys, a best practice in AI development.

## 📊 Sample Interaction & Insights

To interact with the assistant, simply run `python main.py` in your terminal after setting up your environment variables.

Welcome! I'm your AI assistant. Type 'quit' to exit.
You can chat with me or ask anyting.

 **You: Hello there!**<br />
 **Assistant: Hello! How can I assist you today?**<br />

This interaction demonstrates the fundamental conversational capability of the agent. While currently limited without active tools, it forms the basis for more sophisticated interactions once tools are integrated.

## 🚀 Future Scope

* **Integrate and Activate Custom Tools**: Implement and enable tools like `calculator` or `say_hello`, or new ones for web search, data retrieval, etc., to significantly expand the assistant's functional capabilities.
* **Implement Conversational Memory**: Add memory components (e.g., `ConversationBufferMemory`) to allow the agent to remember past turns in the conversation, leading to more coherent and context-aware interactions.
* **Enhance Error Handling**: Improve the robustness of the application by adding more specific error handling for API calls or agent failures.
* **Modularize Codebase**: Refactor `main.py` into smaller, more manageable modules for better organization and scalability.
* **Containerization**: Use Docker to containerize the application for easier deployment and environment consistency.

## 🧾 License

This project is for educational and experimental purposes. 
