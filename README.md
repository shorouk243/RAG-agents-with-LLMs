# Interactive Retrieval-Augmented Generation (RAG) Agent

An **Interactive Retrieval-Augmented Generation (RAG) Agent** designed to answer user queries by combining information retrieval and natural language generation. The system retrieves relevant information from a predefined dataset (text chunks) and generates contextually accurate responses using a language model.

## Project Overview

This project builds a system that:
1. Retrieves relevant information from a dataset based on user queries.
2. Uses a powerful language model to generate informative, coherent answers.
3. Provides an interactive query-response interface for real-time engagement.

The system is suitable for applications like chatbots, virtual assistants, and customer support systems.

---

## Features

- **Real-Time Query Response**: Processes user queries and generates answers in real-time.
- **Retrieval + Generation**: Combines information retrieval for relevance and text generation for fluent responses.
- **Domain Adaptability**: Easily adaptable to different datasets and domains.
- **Interactive and Scalable**: Designed for interactive use with potential scalability for large datasets.

---

## Workflow

1. **Data Source**:
   - Predefined dataset containing chunks of text related to the domain (e.g., descriptions of depression, symptoms, and types).

2. **Retrieval Process**:
   - Searches through the dataset to retrieve the most relevant chunks based on the user's query.
   - Uses similarity algorithms (e.g., cosine similarity, embeddings) for matching queries to text chunks.

3. **Text Generation**:
   - Uses a **language model** (e.g., GPT-2 or BART) to generate answers based on the retrieved text.
   - Models are fine-tuned or prompted to produce fluent, contextually accurate responses.

4. **Interactive Query System**:
   - Users interactively ask questions, and the system retrieves relevant information and generates tailored responses.

---

## Models Used

### Text Retrieval
- Retrieves the most relevant chunks from the dataset using similarity-based matching techniques.

### Language Model (Text Generation)
- **[GPT-2](https://huggingface.co/gpt2)**:
  - Excels at generating coherent and human-like responses.
- **[BART](https://huggingface.co/facebook/bart-large-cnn)**:
  - Ideal for summarization and concise answer generation.

---

## Example Interaction

**User Query**:  
*What are the different types of depression?*

**Retrieved Chunks**:  
1. Descriptions of major depression and persistent depressive disorder.  
2. Seasonal affective disorder and other less common types.  

**Generated Response**:  
*"There are two common types of depression: Major depression, which involves severe mood symptoms for at least 2 weeks, and Persistent depressive disorder, which includes milder symptoms lasting for 2 years or more. Additionally, seasonal affective disorder is related to seasonal changes."*

---

## Use Cases

- **Mental Health Assistants**: Provide information about mental health conditions like depression, symptoms, and treatments.
- **Customer Support**: Respond to user queries by retrieving and generating answers from a knowledge base.
- **Chatbots**: Build conversational agents with knowledge about specific domains.
- **Healthcare Applications**: Share information about medical conditions, treatments, and general well-being.

---

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/interactive-rag-agent.git
   cd interactive-rag-agent
