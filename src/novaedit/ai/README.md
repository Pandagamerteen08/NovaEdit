# AI Module

## Overview

The AI module provides artificial intelligence capabilities to NovaEdit, enabling features like code completion, generation, and intelligent assistance.

## Components

### nova_ai.py
Main AI controller:
- AI feature orchestration
- Request handling and routing
- Response processing
- Feature management

### memory.py
AI memory and context management:
- Conversation history
- Code context preservation
- User preference learning
- Session management

### providers.py
External AI provider integrations:
- Support for multiple AI services
- Provider abstraction layer
- API client management
- Response normalization

## Supported AI Providers

### Planned Integrations
- OpenAI GPT models
- Anthropic Claude
- Google PaLM
- Local LLM support
- Custom provider framework

## AI Features

### 1. Code Completion
Intelligent suggestions as you type:
- Function completions
- Variable completions
- Keyword suggestions
- Module/library suggestions

### 2. Code Generation
Generate code from natural language:
- Function generation
- Class generation
- Boilerplate code
- Comment-to-code

### 3. Error Analysis
AI-powered error explanations:
- Error interpretation
- Suggested fixes
- Related documentation
- Learning resources

### 4. Code Explanation
Understand code with AI help:
- Function explanation
- Algorithm explanation
- Complex logic breakdown
- Language-specific patterns

## Usage Examples

### Basic AI Request

```python
from novaedit.ai.nova_ai import NovaAI

ai = NovaAI()
response = ai.generate_code("Create a Python function to calculate factorial")
print(response)
```

### With Context

```python
context = {
    "language": "python",
    "file_content": open("main.py").read(),
    "cursor_line": 42
}
response = ai.complete_code(context)
```

### Memory Management

```python
from novaedit.ai.memory import Memory

memory = Memory()
memory.add_interaction("user_message", "assistant_response")
history = memory.get_history(limit=10)
```

## Configuration

Settings for AI module in `settings/defaults.json`:

```json
{
  "ai": {
    "enabled": true,
    "provider": "openai",
    "model": "gpt-4",
    "api_key": "your-key-here",
    "temperature": 0.7,
    "max_tokens": 2000,
    "context_window": 4000
  }
}
```

## API Reference

### NovaAI Class

```python
class NovaAI:
    def generate_code(prompt: str, context: dict = None) -> str
    def complete_code(context: dict) -> str
    def explain_code(code: str, language: str) -> str
    def analyze_error(error: str, context: dict) -> str
    def set_provider(provider: str, config: dict) -> bool
```

### Memory Class

```python
class Memory:
    def add_interaction(role: str, content: str) -> None
    def get_history(limit: int = None) -> List[dict]
    def clear_history() -> None
    def set_context(context: dict) -> None
    def get_context() -> dict
```

## Provider Implementation

### Creating Custom Provider

```python
from novaedit.ai.providers import BaseProvider

class CustomProvider(BaseProvider):
    def __init__(self, api_key: str):
        self.api_key = api_key
    
    def generate(self, prompt: str, **kwargs) -> str:
        # Implement your provider logic
        pass
    
    def complete(self, context: dict) -> str:
        # Implement completion logic
        pass
```

## Privacy and Security

### Data Handling
- User code is sent to AI provider (configurable)
- Local processing option available
- Option to disable AI features entirely
- Clear data disclosure in settings

### API Keys
- Never hardcode API keys
- Use environment variables
- Encrypted storage in settings
- Clear instructions for setup

## Performance Considerations

- Requests made asynchronously to avoid blocking UI
- Results cached for identical prompts
- Memory pruned automatically (configurable)
- Rate limiting respects provider limits

## Error Handling

```python
from novaedit.ai.nova_ai import AIError

try:
    response = ai.generate_code(prompt)
except AIError as e:
    print(f"AI Error: {e}")
    # Fallback behavior
```

## Future Enhancements

- [ ] Local model support (Ollama, LM Studio)
- [ ] Real-time code review
- [ ] Intelligent refactoring suggestions
- [ ] Documentation generation
- [ ] Unit test generation
- [ ] Bug detection and fixes
- [ ] Performance optimization suggestions
- [ ] Architecture recommendations

## Directory Structure

```
ai/
├── README.md            # This file
├── nova_ai.py          # Main AI controller
├── memory.py           # Context and history
├── providers.py        # Provider implementations
└── examples/           # Usage examples
```

## Troubleshooting

### API Key Issues
- Verify API key is correct
- Check provider account is active
- Ensure API key has necessary permissions

### Rate Limiting
- Check rate limit status
- Implement exponential backoff
- Contact provider about limits

### Poor Suggestions
- Provide more context
- Check language detection
- Review provider model selection
- Consider prompt engineering

---

For settings configuration, see `../settings/settings.py`.
For integration with editor, see `../editor/editor.py`.
