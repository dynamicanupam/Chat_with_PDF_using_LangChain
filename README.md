
# Chat with PDF files using LangChain and Google Gemini-Pro
---
> An AI-powered system for extracting, summarizing, and providing real-time Q&A from PDF documents, capable of understanding and responding to user queries.
---
## Objectives
The objective of this project is to enable interactive Q&A with multiple PDF files using the Google Gemini Generative AI model. Users can upload PDFs, ask questions related to their content, and receive accurate responses based on the document information.

## Demo
https://github.com/user-attachments/assets/02a035d8-6efa-468f-bf61-656660e68c80

## Features
- **AI-Powered Extraction**: Automatically extracts text from multiple PDFs.
- **Summarization**: Uses large language models (LLMs) to generate concise document summaries.
- **Question Answering**: Enables users to query PDF content and receive accurate, context-aware responses.
- **Real-Time Interaction**: Offers a seamless chat interface for engaging with document content.

## Tools and Libraries Used

- **Streamlit**: Used for building the web application interface, making it easy to create interactive elements and display information to the user.
- **PyPDF2**: Used for reading text from PDF files, allowing the app to extract information from uploaded PDFs.
- **Langchain**: Used for natural language processing tasks, including text splitting, vector embeddings, and question answering.
- **Google Generative AI**: Specifically, the Gemini model, used for generating answers to questions based on the content of the PDF files.
- **FAISS**: Used for similarity search, creating a vector store of text chunks from the PDF files to enable efficient retrieval of relevant information.
- **dotenv**: Used for loading environment variables, allowing the app to securely access the Google Generative AI API key.

## Installation
To run the application, first install the required dependencies.
Clone the repository first and then intall the requirements.txt file 

    pip install -r requirements.txt

## Usage
Set up your environment variables: 
Ensure you have access to Google Gemini Pro API and update your .env file with the appropriate API keys.
Run the application:

     streamlit run app.py

Upload your PDF documents through the interface, and start querying them using the provided chat interface.

## How It Works
- **Document Upload**: Allows users to upload multiple PDF files via the web interface.
- **Text Extraction**: Utilizes PyPDF2 to extract text from each PDF.
- **Query Processing**: Employs LangChain and Google Gemini Pro to interpret and handle user queries.
- **Answer Generation**: Delivers accurate responses and summaries based on the content of the uploaded PDFs.
