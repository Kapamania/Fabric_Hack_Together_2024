Welcome to the documentation for the Legal Summarizer - RAG App – your comprehensive solution for summarizing legal documents and creating an interactive question-answering system. The RAG App is designed to streamline the process of understanding complex legal materials, enabling users to extract key insights efficiently.

Purpose:

In today's legal landscape, professionals are inundated with vast amounts of documentation, ranging from contracts and statutes to case law and regulatory texts. Extracting relevant information from these documents can be time-consuming and labor-intensive. The RAG App aims to address this challenge by offering a robust platform for summarization and question-answering, empowering users to navigate legal content with ease.

Step 1: Import and Install Necessary Libraries:

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/d9fd57eb-787b-4e55-a3dc-10ff05a6ff18)

We are using Langchain, OpenAI Embeddings and FAISS

Langchain provides a framework for text processing tasks, such as text splitting and vector storage. In the RAG App, langchain facilitates the organization and manipulation of legal text data, enabling efficient processing and analysis.

OpenAI embeddings offer powerful representations of text that capture semantic meaning. By utilizing OpenAI embeddings, the RAG App can understand the context and meaning of legal documents, enabling accurate summarization and question-answering capabilities.

FAISS is a library for efficient similarity search and clustering of dense vectors. It is commonly used in natural language processing tasks to store and retrieve embeddings efficiently.

Step 2: Initialize your API KEYS (It is recommended to use an environment variable to store and access the keys)

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/e558ac0b-b602-4fd7-9c58-48d59e74bae3)

Step 3: Set up the path for your documents.

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/64418d4a-af1a-4f7d-be41-f5821b1ae262)

If you are Using Fabric Notebooks for coding the app then you can use the Lakehouse API Path link of the document.
You can upload your docs in /lakehouse/default/Files/ folder in the lakehouse.

Step 4: Extract the texts from the PDFs in the form of raw texts

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/4daa190c-3438-4c78-9d92-198aa8943fb4)

Step 5: Split the text using Character Text Split such that it should not increase the token size

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/de4f2b0b-0bba-4115-95c2-682c16daacc8)

Step 6: Download embeddings from OpenAI

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/f9b7be9a-8e4d-428f-8143-88b8124f1791)

Step 7: Searching the documents with the OpenAI embeddings that are generated

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/85bff7aa-c765-49a6-99be-3ad9c03c5726)

Step 8: Demonstrates how to load a question-answering chain and specify the underlying language model for processing textual data.

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/a1e9ccf5-ddd9-49c5-97f1-7a487aa81ada)

Step 9: Query the app and get results

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/dc85f75c-0ba0-42a2-a3c7-0d48f1a7b505)







