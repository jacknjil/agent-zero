# Aider Usage with Different LLMs

This document provides detailed information about how to use aider with various Language Models (LLMs).

## Supported LLMs

Aider supports the following LLMs:

1. OpenAI GPT models
2. Anthropic Claude models
3. Local models via Ollama

## Configuration

To use aider with different LLMs, you need to set up the appropriate API keys and configurations. Here's how to do it for each supported LLM:

### OpenAI GPT Models

1. Obtain an API key from OpenAI.
2. Set the `OPENAI_API_KEY` environment variable:
   ```
   export OPENAI_API_KEY="your-api-key-here"
   ```
3. When running aider, specify the OpenAI model you want to use:
   ```
   aider --model gpt-4
   ```

### Anthropic Claude Models

1. Get an API key from Anthropic.
2. Set the `ANTHROPIC_API_KEY` environment variable:
   ```
   export ANTHROPIC_API_KEY="your-api-key-here"
   ```
3. Run aider with a Claude model:
   ```
   aider --model claude-2
   ```

### Local Models via Ollama

1. Install Ollama on your system.
2. Pull the desired model:
   ```
   ollama pull codellama
   ```
3. Run aider with the local model:
   ```
   aider --model ollama/codellama
   ```

## Best Practices

- Choose the appropriate model based on your task complexity and required context length.
- For code-related tasks, models fine-tuned on code (like GPT-4 or CodeLlama) often perform better.
- Local models via Ollama can be faster and more private, but may have lower capabilities compared to cloud-based models.

## Troubleshooting

If you encounter issues:

1. Ensure your API keys are correctly set and have the necessary permissions.
2. Check your internet connection for cloud-based models.
3. For local models, ensure Ollama is running and the model is correctly installed.

For more detailed information and advanced usage, please refer to the official aider documentation.
