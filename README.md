# mcp-cline
mcp - clineserver

make sqlite table and copy to folder :C:/Users/people.db

make folder : "C:\Users\cline\mcp\sqlite\server"s and clone code into it : git clone https://github.com/modelcontextprotocol/servers.git

add Cline to visual studio code
in cline add mcp server and in market search for sqlite and install it.

in the client_mcp__setting.json add below config:


{
  "mcpServers": {

    "sqlite": {
      "command": "uv",
      "args": [
        "--directory",
        "C:/Users/cline/mcp/sqlite/servers/src/sqlite",
        "run",
        "mcp-server-sqlite",
        "--db-path",
        "C:/Users/people.db"
      ]
    }

  }
}



