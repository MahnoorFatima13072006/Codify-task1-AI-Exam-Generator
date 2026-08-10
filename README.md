# AI Exam Generator – Task 1

## Overview

This project is an AI-based Exam Generator developed in Python.

The system takes a curriculum/syllabus text file as input, extracts the topics from it, and uses an AI model to generate exam questions based on those topics.

The generated questions are then cleaned, formatted, and saved as a text-based exam paper.

## Features

- Load a curriculum from a `.txt` file
- Read and process the syllabus content
- Split the syllabus into individual topics
- Generate AI-based descriptive exam questions
- Generate questions based on individual curriculum topics
- Clean unnecessary text from generated questions
- Save the generated exam paper as a `.txt` file

## Technologies Used

- Python
- Ollama
- DeepSeek-R1 8B
- Requests
- Jupyter Notebook

## AI Model

The project uses the **DeepSeek-R1 8B** model through Ollama.

The Python program sends the topic and question-generation prompt to the locally running Ollama service. The generated response is then returned to Python for further processing.

## How It Works

The system follows these steps:

1. The curriculum `.txt` file is loaded.
2. The syllabus content is read by the Python program.
3. The syllabus is split into individual topics.
4. A prompt is created for each topic.
5. The prompt is sent to the DeepSeek-R1 8B model through Ollama.
6. The AI generates an exam question.
7. The generated response is cleaned and formatted.
8. The questions are saved as an exam paper in a `.txt` file.

## Project Workflow

```text
Curriculum (.txt)
       ↓
Load Syllabus
       ↓
Split into Topics
       ↓
Create AI Prompt
       ↓
DeepSeek-R1 8B via Ollama
       ↓
Generate Questions
       ↓
Clean Questions
       ↓
Save Exam Paper (.txt)
