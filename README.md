# 🚀 SolTraider: Your Agentic Platform for Any Market! 🌐🧠

## 🌟 Introduction

G'day legends! 👋 Are you ready to ride the wild waves of the markets? 🌊 *SolTraider* is a cutting-edge, modular, and extensible Python platform that uses AI to conquer any market! Forget spreadsheets and hunch-based decisions; this is a whole new level of data analysis and intelligent trading.

Built from the ground up using a multi-agent architecture, *SolTraider* is like having a team of highly skilled experts, each with its own job and all working together in perfect harmony. 🎶 With Google Gemini as the brains of the operation 🧠, you’ve got a system that can adapt, learn, and conquer. 💪

## ✨ Key Features

*   **Multi-Agent System:** 🤖 A network of independent agents, all working together with clearly defined roles, ensuring that no task is missed.
*   **Gemini-Powered Insights:** 🧠 Leverages the might of Google Gemini for complex reasoning and analysis.
*   **Dynamic Data Handling:** ⚡️ Fetch data from multiple sources, and easily pipe the data around the system.
*   **Configurable & Extensible:** ⚙️ Easily create custom agents (plugins) by adding a configuration entry and building new logic.
*   **Modular Code:** 🧩 The core code is kept very modular and clean, making it a powerful base from which to expand and create more.
*   **Scalable Platform:** 📚 A powerful data-driven system that is ready for your custom requirements.

## 🎯 Core Architecture

At the heart of *SolTraider* is a robust core infrastructure designed to provide a solid foundation for all our agents to work together. The core modules are:

*   **`ConfigManager`**: Handles configuration loading and validation, from YAML files and environment variables, and makes it available for all other agents.
*   **`DataManager`**: Manages data storage and retrieval, both structured and unstructured data is stored by this manager, making it available to all other agents. It uses a local database for the structured data, and also uses a vector store for less structured data.
*   **`AgentManager`**: Manages the lifecycle of agents, creating, starting and stopping agents, and ensuring that all data is passed between them correctly.
*   **`GeminiManager`**: Provides the interface with the Google Gemini API, so that our agents can use the power of AI.

## 🤖 Core Agents

The core agents are essential to the system and provide the basic infrastructure for the rest of the agents, and they must be rock solid.

*   **🧭 Agent Endpoint (The Navigator):** The Navigator knows all of the available APIs and will direct other agents to the best endpoint for their needs, based on the type of request.
*   **🏃 Agent Gopher (The Fetcher):** The Fetcher is responsible for actually calling the different APIs, and for taking data and returning the raw results.
*  **🔒 Agent Data (The Vault Keeper):** The Vault Keeper is the single source of truth for the entire system, and it is also responsible for storing both structured, and unstructured data in our database and in the vector store.
*  **🧠 Agent Gemini (The Oracle):** The Oracle uses Gemini to provide insights based on the data in the system, and will use data from the `Data Agent` to generate actionable intelligence.
*  **🗣️ Agent Trade (The Handler):** This is the agent that action the Gemini Insights. They have rules that control how they buy or sell based on the Gemini insights and all of the historical prices that they know.
* **👂 Agent Big Ears (The Listener):** This agent has very big ears, and is listening to all data flowing through the system, so that it can then be sent to other systems via a websocket.
*  **⚖️ Agent Validator (The Verifier):** This agent is responsible for ensuring that all data and all agents adhere to all system standards.

## ✨ User Agents

The user agents are the ones that are able to be modified and changed by the users of our system, they can use the core agents, but they do not have direct access to the system.

*   **🎯 Agent Trending (The Trend Tracker):** This agent is our trend hunter, finding the next hot tokens to help you get the edge in the market.
*  **🔑 Agent Token (The Gatekeeper):** This is our entry point, making sure that all new tokens are valid, and that they are correctly added into the system so that we can start tracking them immediately.
*  **📣 Agent SMS (The Messenger):** This agent is our personal alert service, and making sure you are kept up to date, and is only sending you information when it is essential to do so.

## 🛠️ Build Your Own Agent

*   **Config-Driven:** Create custom agents without changing any of the core code, just modify the configuration.
*   **Gemini Intelligence:** With Gemini at the core, you can build an agent that is capable of incredible feats of analysis.
*   **Complete Customization:** You are able to add any python code as a new agent, to perform actions based on the data you collect.

## 🎯 Why Choose SolTraider?

*   **Real-World Results:** 📈 We're "dogfooding" the system, so we have faith in its power and potential.
*   **Tech Focused:** 💻 Built on modern tech (Pydantic, Gemini) and adheres to high coding standards and practices.
*   **Community Driven:** 🤝 With this code, you are joining a community of builders.
*   **Future Proof:** 🚀 Start with meme coins, but easily extend to other markets, and even data sources as needed.
*   **Robust:** This code has complete tests and is always ready for anything.

## 🚧 Milestones Overridden

*   We have removed the initial requirement for the system to only look at memecoins, instead focusing on general token information.
*   We have also removed the previous ideas of how the `DataFetchAgent` should work, we have instead replaced this with `Agent Price`, that only focus on fetching prices.
*  We have also moved to using `Agent Data` to store and retrieve all of our structured data.
*   The system is now using a new modular approach to configuration and agent loading, which is now using namespaces.

## 🚀 Let's build something amazing!

Ready to jump in? We are!
