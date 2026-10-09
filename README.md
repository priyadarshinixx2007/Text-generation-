# Text-generation-
# Text Generation Using AI

A simple **AI-powered Text Generation application** built using **Python, Streamlit, Hugging Face Transformers, and the Qwen language model**.

The application allows users to enter a prompt and generate AI-based text. Users can also control the maximum length and temperature of the generated text.

---

## Project Overview

Text generation is an Artificial Intelligence and Natural Language Processing (NLP) task where an AI model generates human-like text based on a given input prompt.

For example, if the user enters:

```text
Artificial Intelligence is
```

The AI model can continue the sentence and generate relevant text.

This project provides a simple web interface where users can enter prompts and generate text without directly interacting with the Python code.

---

## Objectives

* Understand the basics of AI-based text generation.
* Learn how to use Hugging Face Transformers.
* Integrate a pre-trained language model into a Python application.
* Build an interactive AI application using Streamlit.
* Understand text-generation parameters such as `max_length` and `temperature`.
* Generate text based on user-provided prompts.

---

## Technologies Used

| Technology                | Purpose                          |
| ------------------------- | -------------------------------- |
| Python                    | Programming language             |
| Streamlit                 | Web application interface        |
| Hugging Face Transformers | Loading and running the AI model |
| Qwen                      | Pre-trained language model       |
| VS Code                   | Development environment          |

---

## Model Used

The project uses a Qwen language model from Hugging Face.

```text
Qwen/Qwen3.8-2.4T-A95B
```

The model is loaded using the Hugging Face `pipeline()` function with the `text-generation` task.

The model receives the user's prompt and generates a continuation based on that prompt.

**Note:** Verify that the model ID is correct and accessible on Hugging Face before running the application.

---

## How the Project Works

The application follows this workflow:

```text
User enters a prompt
        |
        v
Streamlit receives the input
        |
        v
Prompt is sent to the Qwen model
        |
        v
Model generates text
        |
        v
Generated text is displayed
```

---

## Features

* AI-powered text generation
* Custom user prompts
* Adjustable maximum generation length
* Adjustable temperature
* One-click text generation
* Simple Streamlit interface
* Hugging Face Transformers integration
* Pre-trained language model
* Model caching using Streamlit

---

## Project Structure

```text
text-generation/
|
|-- app.py
|-- requirements.txt
|-- README.md
|-- .gitignore
```

### File Description

| File               | Description                |
| ------------------ | -------------------------- |
| `app.py`           | Main Streamlit application |
| `requirements.txt` | Required Python libraries  |
| `README.md`        | Project documentation      |
| `.gitignore`       | Files excluded from Git    |

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/text-generation.git
```

### 2. Open the Project Directory

```bash
cd text-generation
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Requirements

Create a `requirements.txt` file containing:

```text
streamlit
transformers
torch
```

---

## Run the Application

Start the Streamlit application using:

```bash
streamlit run app.py
```

The application will open in your browser.

---

## Example

### Input

```text
Artificial Intelligence is
```

### Settings

* Maximum length: 100
* Temperature: 0.7

### Output

The AI model generates a continuation based on the given prompt.

Example:

```text
Artificial Intelligence is transforming the way people
work, learn, communicate, and solve complex problems.
```

The exact output may vary because text generation uses sampling.

---

## Concepts Learned

### 1. Natural Language Processing

NLP enables computers to process and generate human language.

### 2. Large Language Models

Large language models generate text based on patterns learned from training data.

### 3. Text Generation

Text generation is the process of producing new text based on an input prompt.

### 4. Hugging Face Transformers

The Transformers library provides access to pre-trained AI models.

### 5. Streamlit

Streamlit makes it possible to create interactive Python-based web applications.

### 6. Prompt-Based Generation

The user's input acts as a prompt that guides the model's generated output.

---

## Limitations

The generated text may:

* Contain incorrect information.
* Repeat certain phrases.
* Produce unexpected results.
* Depend heavily on the input prompt.
* Change when generation settings are modified.
* Require significant computing resources depending on the model.

AI-generated content should be reviewed before being used for important or factual purposes.

---

## Future Improvements

The project can be extended with the following features:

* Copy generated text button
* Clear prompt button
* Download generated text
* Word and token counter
* Chat-style interface
* Multiple text-generation modes
* Generate multiple responses
* Save previous generations
* Improved Streamlit interface
* Deployment using Streamlit Community Cloud
* Additional generation parameters such as `top_k`, `top_p`, and `repetition_penalty`

These improvements can make the application more interactive, flexible, and user-friendly.

---

## Author

**## Author

**Priyadarshini D**

---

## License

This project is intended for educational and learning purposes.
