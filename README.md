# 🤖 Multi-Server AI Agent with Model Context Protocol (MCP)

![Python](https://img.shields.io/badge/python-3.10+-blue.svg) 
![MCP](https://img.shields.io/badge/Protocol-MCP-green.svg)
![LangGraph](https://img.shields.io/badge/Agent-LangGraph-orange.svg)
![License](https://img.shields.io/badge/license-MIT-red.svg)

## 🌟 Project Overview
[cite_start]This project demonstrates a cutting-edge **Agentic AI** system built using the **Model Context Protocol (MCP)**[cite: 2, 43]. [cite_start]By leveraging MCP, this agent can seamlessly interact with multiple data sources and tools without requiring bespoke, hard-coded integrations for every API[cite: 4, 34].

[cite_start]The agent functions as a "Universal Interface," acting like a **USB-C for AI**[cite: 5]. [cite_start]It can intelligently decide whether to fetch art history from a museum or technical documentation for a software library based on your natural language queries[cite: 63, 64, 65].

---

## 🏗️ Architecture
[cite_start]The system follows the standard MCP Client-Server architecture, optimized for scalability and reliability[cite: 9, 10].



### 🔌 Transport Layers Used:
* [cite_start]**STDIO Transport**: Used for the **MetMuseum-MCP** server to handle local process communication[cite: 52, 68].
* [cite_start]**HTTP Transport**: Used for the **Context 7** server to manage remote, cloud-based documentation retrieval[cite: 52, 67].

### 🧠 Core Components:
* [cite_start]**Multi-Server MCP Client**: A unified client that manages simultaneous sessions with both local and remote servers[cite: 53, 54, 93].
* [cite_start]**LangGraph ReAct Agent**: A logic engine powered by LLMs (like GPT-5) that follows a "Reasoning and Acting" pattern[cite: 43, 69].
* [cite_start]**Persistent Memory**: Uses `InMemorySaver` to maintain a `thread_id`, allowing the agent to remember context across multiple chat turns[cite: 70, 78, 96].
* [cite_start]**Asynchronous Execution**: Powered by `asyncio` for non-blocking communication with MCP servers[cite: 71, 97].

---

## 🛠️ Integrated MCP Servers
| Server | Functionality | Transport |
| :--- | :--- | :--- |
| **MetMuseum-MCP** | [cite_start]Access to 400,000+ artworks, metadata, and images from the Metropolitan Museum of Art[cite: 60]. | [cite_start]STDIO [cite: 68] |
| **Context 7** | [cite_start]LLM-optimized documentation search across major software frameworks and libraries[cite: 61]. | [cite_start]HTTP [cite: 67] |

---

## 🚀 Getting Started

### Prerequisites
* Python 3.10+
* Basic understanding of CLI and environment variables.

### Installation
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Leelaissakattaota/mcp-ai-agent.git](https://github.com/Leelaissakattaota/mcp-ai-agent.git)
   cd mcp-ai-agent
