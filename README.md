![ArrayVerse Banner](images/banner.jpg)  
# Array

**Array** is a next-generation multi-agent application designed to revolutionize how you interact with data, queries, and systems. Powered by an intelligent swarm of AI agents, the platform efficiently processes complex tasks by distributing workloads across specialized agents.

## Features 🌟  

- **Dynamic Multi-Agent System**:  
  ArrayVerse employs a network of agents working in tandem:  
  - **Query Dispatcher**: Directs tasks to appropriate agents  
  - **Data Analyzer**: Gathers and organizes relevant data  
  - **Researcher Bot**: Performs in-depth investigations  
  - **Creative Strategist**: Generates fresh solutions  
  - **Critical Thinker**: Validates insights for accuracy  
  - **Response Builder**: Synthesizes a complete, actionable response  

- **Multi-Platform Support**:  
  - **Command-Line Interface (CLI)** for developers  
  - **Telegram Bot** for instant queries  
  - **Web App** for a modern user experience  
  - **REST API** for integration with other services  

- **Advanced Features**:  
  - Stream query responses in real-time  
  - Persistent conversation memory with auto-cleanup  
  - Support for multiple AI providers (OpenAI, Anthropic, custom models)  
  - Highly configurable agent parameters  
  - CORS-enabled API for web integrations  

---

## Installation ⚡  

1. **Clone the repository**:  
```bash  
git clone https://github.com/ArrayVerse/array-app.git  
cd array-app  
```  

2. **Install dependencies**:  
```bash  
pip install -r requirements.txt  
```  

3. **Configure settings**:  
   - Copy the `configs/settings.py.example` file to `configs/settings.py`  
   - Add your API keys and preferences  

---

## Usage 🚀  

### CLI Mode  
Run the main program directly from your terminal:  
```bash  
python main.py  
```  

### Telegram Bot  
1. Obtain a bot token from [@BotFather](https://t.me/botfather)  
2. Add the token to `configs/settings.py`  
3. Launch the bot:  
```bash  
python main.py --mode telegram  
```  

### API Server  
1. Enable the API server in `configs/settings.py`  
2. Start the server:  
```bash  
python main.py --mode api  
```  

The API will be available at `http://localhost:8000` by default.  

---

## API Endpoints 🔗  

- **`GET /health`**: Check server status  
- **`GET /agents`**: Fetch agent configurations  
- **`POST /process`**: Send a query to the agent system  

#### Example Query Payload  
```json  
{  
  "query": "Analyze the growth of ArrayVerse in the last year.",  
  "parameters": {  
    "depth": 90,  
    "technical_focus": true  
  }  
}  
```  

---

## Configuration 🔧  

Key settings can be found in `configs/settings.py`:  

- **Agent Settings**:  
  - Define agent behaviors and parameters  
  - Adjust technical depth, creativity, and more  

- **Platform Configuration**:  
  - `TELEGRAM_BOT_TOKEN`: Your bot token  
  - `ENABLE_API`: Enable or disable the API  

- **LLM Providers**:  
  - `OPENAI_API_KEY`: For OpenAI integration  
  - `ANTHROPIC_API_KEY`: For Anthropic Claude models  

---

## Contribution Guidelines 🤝  

We welcome contributions! To get involved:  
1. Fork the repository and create a new branch for your feature or fix.  
2. Make changes and submit a Pull Request.  
3. Ensure all code adheres to the [coding standards](docs/CONTRIBUTING.md).  

---

## License 📜  

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.  

**Explore the universe of possibilities with ArrayVerse!**  
