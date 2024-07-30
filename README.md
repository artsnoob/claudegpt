# AI Chat CLI

AI Chat CLI is a command-line interface tool that allows users to interact with GPT-4 and Claude AI models directly from their terminal. It supports various features like file input, image analysis, conversation history, and code block saving.

## Features

- Chat with GPT-4 or Claude AI models
- Support for both interactive and non-interactive modes
- File input support for including text content in conversations
- Image analysis capability
- Conversation history tracking and reuse
- Code block saving in coding mode
- Colorized output for better readability

## Prerequisites

- Python 3.6+
- OpenAI API key
- Anthropic API key

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/artsnoob/claudegpt.git
   cd claudegpt
   ```

2. Install the required packages:
   ```
   pip install openai anthropic pygments colorama
   ```

3. Set up your API keys:
   - Open the script and replace `gpt_api_key` and `claude_api_key` with your actual API keys.

## Usage

### Interactive Mode

Run the script without any arguments to enter interactive mode:

```
python claudegpt.py
```

In interactive mode, you can:
- Choose between GPT and Claude APIs
- Enable/disable coding mode
- Use special commands like `file:`, `image:`, `save:`, `history`, and `coding`
- Type `exit` to end the chat

### Non-interactive Mode

You can also use the script in non-interactive mode:

```
python claudegpt.py "Your message here"
```

Additional options:
- `-f` or `--file`: Include a text file in the conversation
- `-i` or `--image`: Analyze an image file

Example:
```
python claudegpt.py "Analyze this image" -i /path/to/image.jpg
```

## Special Commands

- `file: /path/to/file`: Include a text file in the conversation
- `image: /path/to/image`: Analyze an image file
- `save: /path/to/file`: Save the last AI response to a file
- `history`: View and reuse previous questions
- `coding`: Toggle coding mode (enables/disables code block saving)
- `exit`: End the chat session
