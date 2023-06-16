# LLM_Autocontext

LLM_Autocontext is a project aimed at creating a program that leverages the power of LLM (Like GPT-3) models to enhance context-awareness and memory within natural language processing tasks. This program takes the input and output of one LLM instance and incorporates it as contextual memory into the prompt of another instance. By enabling models to retain and utilize prior knowledge, LLM_Autocontext aims to improve the quality and coherence of generated responses.

## Table of Contents

- [LLM\_Autocontext](#llm_autocontext)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Examples](#examples)
- [Set up the context manager](#set-up-the-context-manager)
- [Set the initial context](#set-the-initial-context)
- [Set up the generator](#set-up-the-generator)
- [Start a conversation](#start-a-conversation)

## Introduction

In many natural language processing tasks, context plays a crucial role in generating accurate and coherent responses. However, most LLM models lack an inherent memory mechanism to retain information from previous interactions. LLM_Autocontext addresses this limitation by introducing a program that facilitates the integration of context as memory.

By utilizing LLM_Autocontext, you can enhance the context-awareness of LLM models and create more meaningful conversations or coherent text generation. The program acts as a bridge between two instances of LLM, where the output of one instance becomes the context for the next, providing a form of memory that informs subsequent responses.

## Features

- Seamlessly integrates contextual memory into LLM instances.
- Enhances the quality and coherence of generated responses.
- Supports various LLM frameworks and models.
- Flexible and customizable configuration options.
- Lightweight and easy to integrate into existing projects.

## Installation

Follow these steps to install and set up LLM_Autocontext:

1. Clone the LLM_Autocontext repository from GitHub:

```bash
git clone https://github.com/your-username/LLM_Autocontext.git
```

2. Navigate to the project directory:

```bash
cd LLM_Autocontext
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Configure the LLM framework and models:

   - Open `config.py` file.
   - Specify the paths or names of the LLM models you want to use.
   - Adjust any additional configuration parameters according to your requirements.

5. LLM_Autocontext is now ready to be used in your project.

## Usage

To utilize LLM_Autocontext in your project, follow these steps:

1. Import the necessary modules:

```python
from LLM_Autocontext import LLMContextManager, LLMGenerator
```

2. Create an instance of the LLMContextManager:

```python
context_manager = LLMContextManager()
```

3. Set the context for the LLMGenerator:

```python
context_manager.set_context("previous LLM output")
```

4. Create an instance of the LLMGenerator:

```python
generator = LLMGenerator()
```

5. Generate responses using the contextual memory:

```python
response = generator.generate_response(context_manager.get_context(), "prompt")
```

6. Repeat steps 3-5 for subsequent interactions, updating the context each time.

## Examples

Here are a few examples to demonstrate how LLM_Autocontext can be used:

```python
from LLM_Autocontext import LLMContextManager, LLMGenerator

# Set up the context manager
context_manager = LLMContextManager()

# Set the initial context
context_manager.set_context("")

# Set up the generator
generator = LLMGenerator()

# Start a conversation
user_input = input("User: ")
context_manager.set_context(generator.generate_response(context_manager.get_context(), user_input))

while True:
    user_input