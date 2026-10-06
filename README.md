# Local AI Chatbot

https://baljithk2004-hash.github.io/local-ai-chatbot/
 
A lightweight browser-based chatbot interface for locally running AI models using Ollama.
 
## Features
 
- Simple web interface
- Runs completely on your computer
- No API keys required
- Supports multiple Ollama models
- Privacy-friendly
- Works offline
 
---
 
## Installation
 
### 1. Install Ollama
 
Download and install Ollama from:
 
https://ollama.com
 
Verify installation:
 
```cmd
ollama --version
```
 
---
 
### 2. Download Qwen2.5 Coder 1.5B
 
Open Command Prompt and run:
 
```cmd
ollama pull qwen2.5-coder:1.5b
```
 
Wait for the model download to complete.
 
---
 
### 3. Start Ollama
 
Start the Ollama server:
 
```cmd
ollama serve
```
 
You should see Ollama listening on:
 
```text
http://localhost:11434
```
 
---
 
### 4. Test the Model
 
Run a quick prompt:
 
```cmd
ollama run qwen2.5-coder:1.5b
```
 
Example:
 
```text
>>> Write a simple HTML page
```
 
---
 
### 5. API Request Example
 
Generate a response using the Ollama API:
 
```cmd
curl http://localhost:11434/api/generate -d "{\"model\":\"qwen2.5-coder:1.5b\",\"prompt\":\"Create a login form\",\"stream\":false}"
```
 
Example response:
 
```json
{
"response": "<html>...</html>"
}
```
 
---
 
## Using with This Chatbot
 
1. Start Ollama:
 
```cmd
ollama serve
```
 
2. Open the chatbot website.
 
3. Ensure the chatbot is configured to connect to:
 
```text
http://localhost:11434/api/generate
```
 
4. Start chatting.
 
---
 
## Supported Models
 
Examples:
 
```cmd
ollama pull qwen2.5-coder:1.5b
```
 
```cmd
ollama pull qwen2.5:1.5b
```
 
```cmd
ollama pull phi3:mini
```
 
```cmd
ollama pull llama3.2:1b
```
 
---
