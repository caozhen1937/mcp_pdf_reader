# MCP Enabled PDF Reader
Model Context Protocol (MCP) server exposes a tool called read_pdf to read a single pdf document. Although there is no maximum size to the pdf file that can be read, the number of tokens passed to the model will be the limiting factor.

## Installation

### Prerequisites

#### Windows
1.Install Python 3.10 or higher:
   - Download the latest Python installer from [python.org](https://python.org)
   - Run the installer, checking "Add Python to PATH"
   - Open Command Prompt and verify installation with `python --version`

2.Install uv:
   - Open Command Prompt as Administrator
   - Run `pip install --user uv`
   - Verify installation with `uv --version`

#### macOS

1.Install Python 3.10 or higher:
   - Using Homebrew: `brew install python`
   - Verify installation with `python3 --version`

2.Install uv:
   - Using Homebrew: `brew install uv`
   - Alternatively: `pip3 install --user uv`
   - Verify installation with `uv --version`

## Configuration

Add the following to your IDE mcp config.

```json
{
    "mcpServers": {
        "mcp-pdf-reader": {
            "command": "uvx",
            "args": [
                "--from",
                "git+https://github.com/caozhen1937/mcp_pdf_reader@main",
                "mcp_pdf_reader"
            ]
        }
    }
}
```


## Contributing

We welcome contributions to improve these tools. Please submit issues and pull requests through our repository.

## Support

For questions and support:
1. Check our documentation
2. Submit an issue in our repository
