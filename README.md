# Moringa AI Capstone Project: Beginner's Toolkit with GenAI

## 1. Table of Contents
  - [Quick Summary](#2-quick-summary-of-the-toolkit)
  - [System Requirements](#3-system-requirements)
  - [Installation Instructions](#4-installation-instructions)
  - [Usage Examples](#5-usage-examples-tutorials)
  - [Sample Code](#6-sample-code)
  - [Common Issues & Fixes](#7-common-issues--fixes)
  - [References](#8-references)

## 2. Quick Summary of the Toolkit
  This toolkit is designed to introduce complete beginners to the world of Generative AI. It provides a simple, hands-on introduction to using Python to generate text.
  
  **Why use this?**
  - Understand the basics of Large Language Models (LLMs).
  - Run your first AI model without needing expensive hardware.
  - Learn how to integrate AI into your own Python projects.

## 3. System Requirements
  To run the code in this toolkit, you need:
  - **Operating System:** Windows, macOS, or Linux (or a browser for Google Colab).
  - **Python:** Version 3.7 or higher.
  - **Internet Connection:** Required to download the model weights.

## 4. Installation Instructions
  If you are running this locally (on your own computer), follow these steps:
  
  1. **Clone the Repository:**
     ```bash
     git clone [https://github.com/](https://github.com/)[YOUR-USERNAME]/GenAI-Beginners-Toolkit.git
  
  2. **Create a Virtual Environment (Optional but Recommended):**
     
         python -m venv venv
         source venv/bin/activate  # On Windows use: venv\Scripts\activate
  
  4. **Install Dependencies:**
     
         pip install transformers torch

## 5. Usage Examples (Tutorials)
  The primary tool in this kit is the Story Generator.
  - **Open the genai_tutorial.ipynb file in Jupyter Notebook or VS Code.
  - **Run the initialization cell to download the GPT-2 model.
  - **Change the my_prompt variable to whatever text you want.
  - **Run the final cell to see the AI continue your story.

## 6. Sample Code
  Here is the core Python snippet used to generate text:
  
    from transformers import pipeline
  
    # Load the model
    generator = pipeline('text-generation', model='gpt2')
  
    # Generate text
    result = generator("The future of AI is", max_length=50)
    print(result[0]['generated_text'])

## 7. Common Issues & Fixes
  ***Issue***, ***Cause***, ***Fix***
  - **ModuleNotFoundError  - **Libraries not installed  - **Run pip install transformers torch again.
  - **Slow Generation  - **CPU limitation  - **"If running locally on an old PC, try using Google Colab for faster speeds."
  - **Nonsense Output  - **Model Limitations  - **"GPT-2 is an older model. For better quality, try changing the model to gpt2-medium."

## 8. References
  - **Hugging Face Transformers Documentation: huggingface.co/docs/transformers
  - **Python Official Documentation: python.org
  - **Moringa School Curriculum Resources

