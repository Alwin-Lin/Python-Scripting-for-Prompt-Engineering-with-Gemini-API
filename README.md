# Week 1: Python Scripting for Prompt Engineering

This repository contains the Python script `prompt_experiments.py` for Week 1 of the course.

## Description

The script `prompt_experiments.py` demonstrates various prompt engineering techniques by interacting with the Gemini API. It showcases how different prompting strategies (zero-shot, few-shot, and chain-of-thought) affect the LLM's output for a defined task, such as sentiment classification of user-provided text.

## How to Run

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url> # Replace <your-repository-url> with the actual URL
    cd <your-repository-name> # Replace <your-repository-name> with the actual directory name
    ```
2.  **Install dependencies:**
    ```bash
    pip install google-generativeai python-dotenv
    ```
3.  **Set up your API Key:**
    * Create a `.env` file in the root directory of the project.
    * Add your Gemini API key to the `.env` file:
        ```
        GEMINI_API_KEY=YOUR_ACTUAL_GEMINI_API_KEY
        ```
    * **Important:** Ensure `.env` is listed in your `.gitignore` file to prevent committing your API key.

4.  **Run the script:**
    ```bash
    python prompt_experiments.py
    ```
    The script will prompt you to enter text (e.g., a movie review) and then display the outputs from the different prompting techniques.

## Prompting Techniques Implemented

The script demonstrates and compares the following prompting techniques:

* **Zero-Shot Prompting:** Directly asks the LLM to perform a task on the input text without any prior examples within the current prompt.
    * *Example in script:* "Classify the sentiment of this movie review: '[user_text]'"
* **Few-Shot Prompting:** Provides the LLM with 2-3 examples of the desired input/output format or task execution before presenting the actual query. This helps guide the model towards the expected response style and accuracy.
    * *Example in script:* Programmatically adds examples like "Review: '...' Sentiment: Positive" before the user's review.
* **Chain-of-Thought (CoT) Prompting:** Appends a phrase like "Let's think step-by-step." to the query. This encourages the model to break down the problem into intermediate reasoning steps, which can lead to more accurate and well-explained results, especially for complex tasks.
    * *Example in script:* "Classify the sentiment of this movie review and explain your reasoning: '[user_text}'. Let's think step-by-step."

## Expected Outcomes from Running the Script

* The script will print the exact prompt used for each technique.
* The script will print the LLM's response for each technique.
* Users can observe and compare how the LLM's output changes based on the prompting strategy. This allows for a practical understanding of:
    * How zero-shot performs as a baseline.
    * How providing examples in few-shot can improve specificity or accuracy.
    * How encouraging step-by-step reasoning with CoT can enhance the explanatory power or problem-solving capability of the model.

## Files

* `prompt_experiments.py`: The main Python script.
* `.env` (user-created, and should be in `.gitignore`): Stores the Gemini API key.
* `README.md`: This file.
* `.gitignore` (user-created or generated): Specifies intentionally untracked files that Git should ignore (e.g., `.env`, `__pycache__/`).
