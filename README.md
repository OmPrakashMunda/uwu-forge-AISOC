# PythOWO 🌸

A kawaii Python interpreter and code generation service that transforms regular Python into an uwu-fied programming language! Built during [Hackathon Name] to make coding more adorable.

## What is PythOWO? ✨

PythOWO consists of two main components:

1. **PythOWO Interpreter**: A custom Python interpreter that executes code written in PythOWO syntax. It features:
   - Custom lexer and parser for uwu-style syntax
   - Variable scope management
   - Support for basic control structures (IF/EWIF/EWSE)
   - Function definitions with FWUNCTION
   - Interactive shell with kawaii prompts

2. **Code Generation Service**: An Express.js server that:
   - Uses Hugging Face's Qwen2.5-72B-Instruct model for code generation
   - Transforms regular Python into PythOWO syntax in real-time
   - Provides streaming responses for code generation
   - Executes PythOWO code and returns results

## How It Works 🔧

### Interpreter Implementation
The interpreter (`pythowo.py`) uses:
- Regular expressions for syntax parsing
- Python's eval() for expression evaluation
- Custom variable scope management
- Error handling with cute emoticons

### Code Generation Service
The service transforms code using:
```javascript
function pythOWOify(code) {
    // Transforms function definitions
    .replace(/def\s+(\w+)\s*\((.*?)\):/g, 'FWUNCTION $1($2) ->')
    // Transforms if statements
    .replace(/if\s+(.*?):/g, 'IF $1 THWEN')
    // ... more transformations
}
```

### PythOWO Syntax Examples
```python
# Regular Python
def calculate(x):
    if x > 0:
        print("Positive!")
    else:
        print("Non-positive!")

# PythOWO Version
FWUNCTION calculate(x) -> 
    IF x > 0 THWEN
        pwint("Positive!")
    EWSE
        pwint("Non-positive!")
    END
```

## Tech Stack 🛠️

- **Backend**: Express.js, Node.js
- **AI Model**: Hugging Face's Qwen2.5-72B-Instruct
- **Interpreter**: Python
- **Text Processing**: Regular Expressions
- **API**: Server-Sent Events for streaming responses

## Technical Highlights 💫

1. **Real-time Code Transformation**:
   - Regex-based syntax transformation
   - Streaming responses using Server-Sent Events
   - Error handling with kawaii messages

2. **Custom Language Features**:
   - Variable scope management
   - Control flow structures
   - Function definitions
   - Expression evaluation

3. **AI Integration**:
   - Prompt engineering for code generation
   - Stream processing of model outputs
   - Real-time syntax transformation

Built with 💝 for AISOC Chronos v1.0