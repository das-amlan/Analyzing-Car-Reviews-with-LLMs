# Analyzing Car Reviews with LLMs

This project prototypes a chatbot application for "Car-ing is sharing," an auto dealership. The chatbot utilizes various pre-trained Hugging Face Large Language Models (LLMs) to perform several tasks related to car reviews, aiming to assist both customers and human agents.

## Project Goals

The primary goals of this project are to:

*   Develop a prototype chatbot capable of processing and responding to textual prompts related to car reviews.
*   Implement functionalities for sentiment analysis, translation, question answering, and text summarization using pre-trained LLMs.
*   Provide a foundation for building a more comprehensive AI-powered assistant for the auto dealership.

## Functionalities

The chatbot prototype demonstrates the following core functionalities:

### Sentiment Analysis

Analyzes car reviews to determine the overall sentiment (positive or negative) using the \`distilbert-base-uncased-finetuned-sst-2-english\` model. This can be used to quickly gauge customer satisfaction and identify areas for improvement.

### Translation

Translates car reviews from English to Spanish using the \`Helsinki-NLP/opus-mt-en-es\` model, enabling the dealership to handle reviews and communicate with a wider range of customers. The translation quality is evaluated using the BLEU score.

### Question Answering

Extracts relevant information from car reviews by answering specific questions posed by users or agents using the \`deepset/minilm-uncased-squad2\` model. This can help quickly find details about a car's performance, features, or issues.

### Summarization

Generates concise summaries of lengthy car reviews using the \`cnicu/t5-small-booksum\` model, allowing users and agents to quickly grasp the main points without reading the entire text.

## Technical Details

The project utilizes the following key technologies and libraries:

*   **Python:** The primary programming language.
*   **pandas:** For data manipulation and analysis.
*   **torch:** A deep learning framework (used by Hugging Face Transformers).
*   **evaluate:** For evaluating model performance (e.g., BLEU score).
*   **transformers:** The Hugging Face library for accessing pre-trained LLMs and pipelines.

The notebook demonstrates how to load and use different pre-trained models from the Hugging Face Hub for each task.

## Project Structure

The notebook is organized into the following sections:

1.  **Import necessary packages:** Imports required libraries such as pandas, torch, evaluate, and transformers.
2.  **Load Dataset:** Loads the car reviews dataset from a CSV file.
3.  **Classify car reviews:** Demonstrates sentiment analysis using a pre-trained sentiment analysis model and evaluates its performance.
4.  **Translate a car review:** Shows how to translate a car review using a pre-trained translation model and evaluates the translation using the BLEU score.
5.  **Q&A:** Presents an example of question answering on a car review using a pre-trained question answering model.
6.  **Summarize and analyze:** Illustrates text summarization of a car review using a pre-trained summarization model.

## Getting Started

To run this notebook, you will need to have the required libraries installed. You can install them using `pip`.
