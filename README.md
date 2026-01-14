# Local LLM Chatbot with Conversational Memory (Ollama)

A simple Python-based chatbot that runs entirely on a local machine using
Ollama. The chatbot simulates conversational memory by maintaining and
replaying chat history to a stateless large language model.

This project was built as part of the **LLM Engineering course by Ed Donner**
to practice working with local LLMs, prompt engineering, and conversational
memory concepts.

## Overview
Large Language Models do not have memory by default. This project creates
the *illusion of memory* by storing previous user and assistant messages
and sending them back to the model with every new query.

The chatbot responds in a friendly and light-humored tone while maintaining
clear and accurate answers.

## Features
- Runs fully offline using Ollama
- Simulated conversational memory using message history
- Clear separation of system and user prompts
- Loop-based interactive CLI chatbot
- Friendly and humorous response style

## Tech Stack
- Python
- Ollama (local LLM runtime)

## How It Works
1. The system prompt defines the assistant’s personality and behavior.
2. User questions are appended to a message history list.
3. Assistant responses are also appended to the same list.
4. On each interaction, the entire message history is sent back to the
   model, creating the illusion of memory.

## Prerequisites
- Python 3.x
- Ollama installed on your system
- At least one Ollama model pulled (example below)

```bash
ollama pull llama3.2

## Acknowledgements
This project was developed while following the **LLM Engineering course by
Ed Donner**, which provided clear explanations and practical exercises on
working with large language models and local LLM setups.

Thank you to **Ed Donner** for design




