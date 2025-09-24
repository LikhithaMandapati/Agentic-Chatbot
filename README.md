# 🤖 Agentic Chatbot

An intelligent, modular, and extensible chatbot framework designed to build agentic AI systems with advanced capabilities. This project leverages LangGraph, Groq, Tavily, and Streamlit to create a dynamic chatbot interface that can be customized for various use cases.

---

## 🚀 Features

- **Modular Agentic Architecture**: Utilize LangGraph's stateful graph system to define complex workflows.
- **LLM Integration**: Supports Groq's Llama 3 models for powerful language understanding.
- **Tool Integration**: Incorporate external tools like Tavily for web search capabilities.
- **Dynamic UI**: Build interactive interfaces using Streamlit, with configurable options.
- **Configurable Use Cases**: Choose from predefined use cases such as "Basic Chatbot" or "Chatbot with Web".

---

## 🛠️ Tech Stack

- **Backend**: Python 3.10+
- **Frameworks**: LangGraph, Groq, Tavily, LangChain
- **Frontend**: Streamlit
- **Deployment**: Docker (optional)
- **Environment Management**: `.env` files for API keys

---

## 📦 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/LikhithaMandapati/Agentic-Chatbot.git
   cd Agentic-Chatbot
   ```

2. Set up a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:

   Create a `.env` file in the project root and add your API keys:

   ```
   GROQ_API_KEY=your_groq_api_key
   TAVILY_API_KEY=your_tavily_api_key
   ```

---

## 🧪 Usage

1. Run the application:

   ```bash
   python app.py
   ```

2. Open your browser and navigate to `http://localhost:8501` to interact with the chatbot.

3. Use the sidebar to select the LLM, model, and use case. Enter the necessary API keys when prompted.

---

## 🧩 GraphBuilder & Use Cases

The `GraphBuilder` class allows you to define and set up different chatbot workflows:

- **Basic Chatbot**: A simple conversational agent.
- **Chatbot with Web**: An agent that can fetch real-time information using web search tools.

Each use case is defined by a specific graph structure, which can be customized to suit your needs.

---

## 📁 Project Structure

```
Agentic-Chatbot/
├── app.py                  
├── requirements.txt        
├── .env                    
├── src/
│   ├── langgraphagenticai/
│   │   ├── ui/
│   │   │   └── uiconfigfile.py  
│   │   ├── state/
│   │   │   └── state.py         
│   │   ├── nodes/
│   │   │   ├── basic_chatbot_node.py  
│   │   │   ├── chatbot_with_tool_node.py  
│   │   │   └── search_tool.py         
│   └── ...
└── ...
```

---

## 🧑‍💻 Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🔗 References

- [LangGraph Documentation](https://langgraph.com/docs)
- [Groq API Documentation](https://groq.com/docs)
- [Tavily API Documentation](https://tavily.com/docs)
