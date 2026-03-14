This project tells how to use Model Context Protocol (MCP) in a real project. In this project, we are building a simple Weather Agent MCP server and connecting it to Claude Desktop.

After the writing the python code, we need to add this connector in claude Desktop by editing it's config file. Then content in 
claude_desktop_config.json file is as follows

{
  "mcpServers": {
    "weather": {
      "command": "uv",
      "args": [
        "--directory",
        "C:\\Users\\Lokesh\\Documents\\lokesh project\\MCP project",
        "run",
        "weather_agent.py"
      ]
    }
  }
