# Neolen

This code provides a utility for generating answers to questions based on the content of uploaded files. Here is a summary of what the code does:

The code imports necessary libraries including openai, docx, and PdfReader from the PyPDF2 package.

It sets up the OpenAI API credentials using the provided API key.

The code defines a function called generate_default_answer that returns a random default answer from a predefined list when the model cannot provide a specific answer to a question.

There are two functions, extract_text_from_docx and extract_text_from_pdf, for extracting text content from Word documents (.docx) and PDF files (.pdf) respectively.

The code defines the main function, generate_answer, which takes in a list of file paths and a question. It extracts the text content from the uploaded files based on their formats, combines the text content, and prepares an input prompt for the GPT-3.5 model. It then uses the model to generate an answer to the question and returns the generated answer. If the answer is empty, it falls back to using the generate_default_answer function.

Lastly, an example usage is provided where the user is prompted to enter a question and the paths of the files. The generate_answer function is called with the provided inputs, and the resulting answer is printed.

