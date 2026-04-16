🚗 Automotive AI Assistant (RAG-Based)
Project Overview

This project is a Mini AI-Powered Automotive Knowledge Assistant that answers vehicle-related queries such as vehicle models, specifications, service schedules, warning indicators, and recommendations. It uses Embeddings, FAISS, and RAG (Retrieval-Augmented Generation) to provide accurate answers.

Objective

To build an intelligent assistant that can understand user queries, retrieve relevant automotive data, generate accurate responses, and recommend vehicles based on user needs.

Technologies Used

Python
Sentence Transformers (Embeddings)
FAISS (Vector Database)
NumPy

System Architecture

User Query
↓
Embedding (convert text → vector)
↓
FAISS (semantic search)
↓
Retrieve relevant data
↓
Generate Answer (RAG)

Dataset

Synthetic dataset including vehicle models (Ford Explorer, Ford Ranger, Ford Escape, Ford F-150), service details (oil change, maintenance schedules), and warning messages (engine light, battery alert).

Semantic Search
What are Embeddings?

Embeddings convert text into numerical vectors so that machines can understand semantic meaning. For example, "7 seater SUV" is converted into a vector representation.

Similarity Metric (Cosine Similarity)

Cosine similarity measures how similar two vectors are. A value close to 1 means highly similar, while a value close to 0 means not similar. It is used to find the most relevant data for a query.

What is RAG?

RAG (Retrieval-Augmented Generation) combines retrieval (finding relevant data using FAISS) and generation (producing answers using that data).

Why Grounding is Important

In automotive systems, incorrect answers can lead to safety risks. Grounded responses ensure reliability and accuracy.

What Causes Hallucination

Lack of relevant data, weak prompts, and model guessing.

Hallucination Mitigation

Use retrieved context only, restrict answer generation, and return fallback responses like "Information not available".

Features

Semantic search using FAISS
RAG-based question answering
Vehicle recommendation system
Simple and efficient design

Sample Queries

Search: search("7 seater SUV")
Ask: ask("What does engine warning light mean?")
Recommend: recommend("I need a family car")

Sample Output

SEARCH:
['Ford Explorer is a 7-seater SUV suitable for families']

ASK:
Answer: Engine warning light means engine malfunction

RECOMMEND:
['Ford Explorer', 'Ford Escape']

How to Run
Open Google Colab or Jupyter Notebook
Install dependencies: pip install sentence-transformers faiss-cpu
Run the code
Test using sample queries
Design Decisions

Used FAISS for fast similarity search
Used Sentence Transformers for lightweight embeddings
Used rule-based logic for recommendations for simplicity and explainability

Conclusion

This project demonstrates how AI techniques like semantic search and RAG can be used to build an intelligent automotive assistant that provides accurate and useful information.

Author

B. Jothika
B.Tech Artificial Intelligence and Data Science
