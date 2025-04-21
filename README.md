# Medical Diagnosis Knowledge Graph with Retrieval Augmented Generation (RAG)

This project designs and implements a Retrieval Augmented Generation (RAG) system for answering clinical queries and generating informative summaries using the MIMIC-IV-Ext Direct dataset. The system leverages a retrieval component to find relevant documents and a generative model to produce context-aware responses. 
## Overview

This assignment involves the following key tasks:

1. **Data Loading:** Loads the MIMIC-IV-Ext Direct dataset (provided separately) for use in the RAG system.
2. **Document Splitting:** Divides the dataset into smaller chunks for efficient processing.
3. **Embeddings & Vector Store:** Creates embeddings for the text chunks using a pre-trained sentence transformer model (all-MiniLM-L6-v2) and stores them in a FAISS vector database for fast retrieval.
4. **Retrieval & Question Answering:** Uses a large language model (Flan-T5) to answer clinical queries based on the most relevant information retrieved from the vector database.
5. **Summarization:** Summarizes the retrieved information and the generated answer using a text summarization model (BART-large-cnn) to provide concise explanations.

## How to Use

1. **Install dependencies:** Ensure you have the required libraries installed by running the first cell in the notebook.
2. **Load Data:** Place the MIMIC-IV-Ext Direct dataset in the same directory as the notebook. The notebook automatically loads the data.
3. **Run the Cells:** Execute the notebook cells sequentially to initialize the RAG pipeline.

## Technologies

* **MIMIC-IV-Ext Direct:** Dataset containing medical information for clinical queries.
* **LangChain:** Framework for building applications with LLMs.
* **FAISS:** Library for efficient similarity search.
* **Sentence Transformers:** Pre-trained models for generating text embeddings.
* **Flan-T5:** Large language model for text generation.
* **BART-large-cnn:** Text summarization model.
* **Python:** Programming language.

## Potential Improvements

* **Fine-tuning:** Fine-tune the language models on a medical dataset to improve answer accuracy and relevance.
* **Knowledge Graph Expansion:** Extend the knowledge graph with more detailed information and relationships.
* **Enhanced User Interface:** Further develop the Streamlit frontend for improved user experience.

## Disclaimer

This project is for demonstration and educational purposes only. It should not be used for actual medical diagnosis or treatment. Consult with a qualified healthcare professional for any medical concerns.


## License

This project is licensed under the MIT License.
