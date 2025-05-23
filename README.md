# Chatbot with MCP Client

## Usage

```bash
# python server
uv run client.py path/to/server.py

# node server
uv run client.py path/to/build/index.js
```

## How It Works
**When you submit a query:**

- The client gets the list of available tools from the server
- Your query is sent to Claude along with tool descriptions
- Claude decides which tools (if any) to use
- The client executes any requested tool calls through the server
- Results are sent back to Claude
- Claude provides a natural language response
- The response is displayed to you