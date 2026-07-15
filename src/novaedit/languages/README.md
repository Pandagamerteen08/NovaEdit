# Languages Module

## Overview

The Languages module provides syntax highlighting and language support for multiple programming languages in NovaEdit.

## Components

### language_manager.py
Central manager for all language operations:
- Language detection from file extensions
- Language definition loading
- Syntax highlighting rule application
- Language preference management

### Language Definitions
JSON files defining syntax rules for each language:

#### Current Languages
- **python.json** - Python syntax highlighting
- **javascript.json** - JavaScript syntax highlighting
- **html.json** - HTML markup syntax
- **css.json** - CSS stylesheet syntax
- **json.json** - JSON data format
- **markdown.json** - Markdown documentation format

#### Future Languages
- **java.json** - Java programming language (planned)
- **csharp.json** - C# programming language (planned)

## Language Definition Format

Each language definition is a JSON file with the following structure:

```json
{
  "name": "Language Name",
  "fileExtensions": [".ext1", ".ext2"],
  "mimeTypes": ["text/plain"],
  "keywords": {
    "control": ["if", "else", "for", "while"],
    "declaration": ["def", "class", "function"],
    "constant": ["True", "False", "None"]
  },
  "patterns": {
    "string": {
      "single": "'([^'\\\\]|\\\\.)*'",
      "double": "\"([^\"\\\\]|\\\\.)*\"",
      "triple": "'''[\\s\\S]*?'''"
    },
    "comment": {
      "line": "#.*$",
      "block": "/\\*[\\s\\S]*?\\*/"
    },
    "number": "-?\\d+(\\.\\d+)?",
    "operator": "[+\\-*/%=<>!&|^~]",
    "brackets": {"round": "()", "square": "[]", "curly": "{}"}
  },
  "symbols": {
    "function": "def\\s+([a-zA-Z_]\\w*)\\s*\\(",
    "class": "class\\s+([a-zA-Z_]\\w*)"
  }
}
```

## Usage Examples

### Detecting Language from File

```python
from novaedit.languages.language_manager import LanguageManager

manager = LanguageManager()
language = manager.get_language_by_extension(".py")
# Returns: Language object for Python
```

### Getting Syntax Patterns

```python
patterns = manager.get_patterns(language)
# Returns: Dictionary of regex patterns for highlighting
```

### Listing Supported Languages

```python
languages = manager.get_all_languages()
# Returns: List of all supported language objects
```

## Adding a New Language

### Step 1: Create Language Definition

Create `definitions/new_language.json`:

```json
{
  "name": "New Language",
  "fileExtensions": [".nl"],
  "keywords": {
    "control": ["if", "else"],
    "declaration": ["var", "func"]
  },
  "patterns": {
    "string": "\"([^\"\\\\]|\\\\.)*\"",
    "comment": "//.*$"
  }
}
```

### Step 2: Register in Language Manager

Update `language_manager.py` to load the new definition:

```python
def _load_languages(self):
    # Add your language to the loading list
    self.languages['new_language'] = self._load_definition('new_language.json')
```

### Step 3: Test the Implementation

Create test file and verify highlighting works correctly.

## Color Scheme Integration

Languages work with the Theme system for colors:

- Keywords → Color from theme
- Strings → Color from theme
- Comments → Color from theme
- Operators → Color from theme
- Functions → Color from theme

See `themes/theme_manager.py` for color configuration.

## Performance Considerations

- Language definitions are cached after first load
- Regex patterns are compiled for efficiency
- Large files use incremental highlighting
- Syntax highlighting runs in separate thread

## Directory Structure

```
languages/
├── README.md                 # This file
├── language_manager.py       # Main manager
├── definitions/              # Language definitions
│   ├── python.json
│   ├── javascript.json
│   ├── html.json
│   ├── css.json
│   ├── json.json
│   └── markdown.json
└── future/                   # Planned languages
    ├── java.json
    └── csharp.json
```

## Future Enhancements

- [ ] Language server protocol (LSP) support
- [ ] Tree-sitter for better parsing
- [ ] Custom language creation UI
- [ ] Language pack downloads
- [ ] IntelliSense/AutoComplete integration

---

For more information on themes, see `../themes/theme_manager.py`.
For settings integration, see `../settings/settings.py`.
