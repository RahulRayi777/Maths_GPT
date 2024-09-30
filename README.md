# Text To Math Problem Solver and Data Search Assistant

This Streamlit app allows users to input questions related to math or general knowledge and get responses using **Groq's Gemma 2 model** and tools like a math solver and Wikipedia search. The app is built on **LangChain**, integrating tools and agents to handle mathematical reasoning and data searches.

## Features

- **Mathematical Problem Solver**: Users can input complex math problems, and the app will compute and explain the solution step by step using the **LLMMathChain**.
- **Reasoning Tool**: Logic-based and reasoning questions are answered with a detailed explanation.
- **Wikipedia Search**: Users can get general information on topics by leveraging Wikipedia's API.
- **Interactive Chat**: The app allows for real-time interaction with the user, providing responses based on input questions.

App Components

1. Groq LLM (Gemma-2):
The app uses Groq's Gemma-2-9b-It model to perform language-based tasks, such as answering math problems, reasoning, and searching Wikipedia...

2. Tools:
Math Solver (LLMMathChain): A tool that handles mathematical expressions and generates detailed explanations of the solution.
Wikipedia Search: The app can search for information on general topics via the WikipediaAPIWrapper.
Reasoning Tool: A logical reasoning tool that explains answers to non-mathematical questions.

3. Prompt Templates:
The app uses a customized prompt to ensure the model logically solves math questions and provides clear, step-by-step explanations.

5. Agent Initialization:
Zero-Shot React Description Agent: The app uses the AgentType.ZERO_SHOT_REACT_DESCRIPTION, allowing the model to figure out the task from a simple description without requiring task-specific training.
Interaction Flow

## Requirements

To run the app, you will need the following Python libraries:

```bash
streamlit
langchain
langchain_groq
langchain_community
