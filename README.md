# LLM_Autocontext

LLM_Autocontext is a Jupyter Notebook-based project that aims to enhance context-awareness and memory within natural language processing tasks by utilizing two instances of LLM (Like GPT-3) models. This notebook loads the LLM models and passes prompts between them to add context from the previous instance and update the context for subsequent interactions. By incorporating prior knowledge as contextual memory, LLM_Autocontext improves the quality and coherence of generated responses.

## Table of Contents

- [LLM\_Autocontext](#llm_autocontext)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Roadmap](#roadmap)
  - [Features](#features)
  - [Installation](#installation)
    - [(Only Template, Nothing here is really working yet)](#only-template-nothing-here-is-really-working-yet)
  - [Usage](#usage)
  - [Examples](#examples)
  - [Contributing](#contributing)
  - [License](#license)

## Introduction

In many natural language processing tasks, context plays a crucial role in generating accurate and coherent responses. However, LLM models typically lack an inherent memory mechanism to retain information from previous interactions. LLM_Autocontext addresses this limitation by utilizing a Jupyter Notebook that incorporates context from one LLM instance to another.

By leveraging LLM_Autocontext, you can enhance the context-awareness of LLM models and create more meaningful conversations or coherent text generation. The notebook acts as a bridge between two instances of LLM, where the output of one instance becomes the context for the next, providing a form of memory that informs subsequent responses.

## Roadmap

1. **Initial Project Setup**
   - [ ] Set up the project structure and directory.
   - [ ] Create a Jupyter Notebook file for LLM_Autocontext.

2. **Research and Requirements Gathering**
   - [ ] Research different LLM frameworks and models suitable for the project.
   - [ ] Identify the best approach for passing prompts between LLM instances.
   - [ ] Define the requirements and goals of the LLM_Autocontext notebook.
   - [ ] Document the research findings and project requirements.

3. **Load LLM Models**
   - [ ] Add code to load the first LLM model into the notebook.
   - [ ] Verify the successful loading of the LLM model.
   - [ ] Load the second LLM model into the notebook.
   - [ ] Validate the successful loading of the second LLM model.

4. **Define Prompt Passing Logic**
   - [ ] Implement logic to pass prompts from the first LLM model to the second.
   - [ ] Update the context with the output from the second LLM model.
   - [ ] Refine the prompt passing mechanism for seamless context integration.

5. **Implement Conversation Flow**
   - [ ] Design the conversation flow in the notebook using user prompts.
   - [ ] Enable the notebook to capture and display LLM-generated responses.
   - [ ] Iterate the conversation by updating and passing the prompts between LLM models.

6. **Testing and Validation**
   - [ ] Conduct thorough testing of the notebook's functionality.
   - [ ] Validate the accuracy and coherence of generated responses.
   - [ ] Handle edge cases and unexpected user inputs gracefully.

7. **Documentation and Examples**
   - [ ] Document the usage and functionality of the LLM_Autocontext notebook.
   - [ ] Include clear instructions on how to run and customize the notebook.
   - [ ] Provide example conversations and code snippets for reference.

8. **Optimization and Performance**
   - [ ] Identify areas for optimization and performance improvement.
   - [ ] Refactor the code to enhance response generation speed.
   - [ ] Optimize memory usage and ensure efficient context management.

9. **Integration and Deployment**
   - [ ] Test the notebook with different LLM frameworks and models.
   - [ ] Ensure compatibility with popular Jupyter Notebook environments.
   - [ ] Prepare the project for deployment and distribution.

10. **Maintenance and Updates**
    - [ ] Monitor user feedback and address any reported issues promptly.
    - [ ] Incorporate improvements and updates based on community contributions.
    - [ ] Keep the project up to date with the latest LLM advancements and frameworks.

## Features

- Seamlessly integrates contextual memory into LLM instances.
- Enhances the quality and coherence of generated responses.
- Utilizes two instances of LLM models in a Jupyter Notebook.
- Flexible and customizable prompt passing for context updates.
- Lightweight and easy to incorporate into existing projects.

## Installation 
### (Only Template, Nothing here is really working yet)

To use LLM_Autocontext, follow these installation steps:

1. Clone or download the LLM_Autocontext repository from GitHub:

```bash
git clone https://github.com/your-username/LLM_Autocontext.git
```

2. Install the required dependencies. Ensure you have Jupyter Notebook installed:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the LLM_Autocontext notebook (LLM_Autocontext.ipynb) from the project directory.

## Usage

To utilize LLM_Autocontext in the Jupyter Notebook, follow these steps:

1. Open the LLM_Autocontext notebook (LLM_Autocontext.ipynb) in Jupyter Notebook.

2. Run the notebook cells sequentially.

3. Configure the LLM models:
   - Provide the paths or names of the LLM models in the notebook.
   - Adjust any additional configuration parameters as required.

4. Execute the cells to load the LLM models and define the necessary functions.

5. Set the initial context:
   - Execute the cell to set the initial context as an empty string or a predefined value.

6. Begin the conversation:
   - Execute the cell to prompt the first LLM model with user input.
   - The output of the first LLM model will be used as context for the second LLM model.

7. Iterate the conversation:
   - Execute the cells to pass prompts between the LLM models, updating the context as needed.
   - Capture and display the responses generated by the LLM models.

8. Repeat step 7 for subsequent interactions, allowing the context to evolve and improve responses.

9. Customize and experiment with the notebook to suit your specific needs and use cases.

## Examples

Here's an example conversation using the

 LLM_Autocontext notebook:

```
User: Can you tell me a joke?
System: Sure, here's a joke: Why don't scientists trust atoms? Because they make up everything!
User: Haha, that's a good one! Tell me another joke.
System: Of course! Here's another joke: Why don't skeletons fight each other? They don't have the guts!
User: That's hilarious! I want to share this with my friend. What was the first joke again?
System: The first joke was: Why don't scientists trust atoms? Because they make up everything!
```

In this example, the first LLM model generates a joke response, which becomes the context for the second LLM model. The second model generates another joke, and the context is updated. Finally, the user requests to recall the first joke, and the updated context is utilized to provide the requested information.

Please note that this example is simplified, and the actual conversation flow and prompts may vary based on your implementation and specific LLM models.

## Contributing

Contributions to LLM_Autocontext are welcome! If you find any issues or have suggestions for improvements, please feel free to submit a pull request or create an issue on the GitHub repository.

When contributing, please ensure that your code adheres to the project's coding standards and conventions. Additionally, provide clear documentation and examples to support your changes.

## License

[MIT License](LICENSE)

LLM_Autocontext is licensed under the [MIT License](LICENSE), which allows for both personal and commercial use. Refer to the LICENSE file for more information.