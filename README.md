# Intelligent-Assistant-for-Customer-Reviews
This project is designed to create an intelligent assistant that retrieves and summarizes information from customer reviews in the Amazon Customer Reviews Dataset, specifically focusing on Digital Software. The project was developed as part of the final project for the Natural Language Processing course organized by Prof. Giorgio Satta at the University of Padova in the Department of Informatica DEI.

## Contributors
- **Aysima Merve Akkurt** - ICT for Internet and Multimedia

## Dataset
The dataset used in this project is the [Amazon Customer Reviews Dataset](https://www.kaggle.com/datasets/cynthiarempel/amazon-us-customer-reviews-dataset?select=amazon_reviews_us_Digital_Software_v1_00.tsv). It contains:

- A collection of reviews from the Amazon.com marketplace (1995-2015).
- 102,084 unique reviews on Digital Software Products.
- Metadata including customer ID, review ID, product ID, product title, star rating, helpful votes, and more.

## Project Overview
This project implements an intelligent assistant capable of:
1. Retrieving relevant reviews based on user queries.
2. Summarizing the retrieved information using a large language model (LLM).

### Key Components
- **Data Cleaning and Preprocessing**: The dataset was cleaned to handle missing values, text normalization, and splitting lengthy reviews into smaller chunks.
- **Document Embedding and Vector Store Setup**: Utilized the `sentence-transformers` library to generate embeddings for each review chunk and stored them using FAISS for efficient similarity searches.
- **Prompt Engineering**: Designed prompts to structure user queries and retrieve relevant documents.
- **LLM Inference**: Implemented the GPT-2 model to generate coherent responses based on the constructed prompts.

## Installation
To run the project, ensure you have the required libraries installed. You can install them using:
pip install -q sentence-transformers faiss-cpu transformers torch pandas matplotlib

