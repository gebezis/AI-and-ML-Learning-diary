# A very rough outline of a suggested plan by ChatGPT

### 1. Python & Data Handling
- Fluency in NumPy, Pandas, and Python I/O
- Clean code in Jupyter or script format
- Ability to process and structure datasets (JSON, CSV, HTML, etc.)
### 2. ML Foundations
 - Linear/logistic regression, decision trees, basic model training using scikit-learn
 - Understanding of overfitting, train/test split, cross-validation, loss functions
 - Implement one mini-project: e.g., predicting housing prices or classifying movie reviews
### 3. PyTorch
 - Manual implementation of small feedforward and LSTM models
 - Use of torch.nn, optim, and DataLoader correctly
 - One notebook that trains a small model on a dataset (MNIST or similar)
### 4. Transformers with Hugging Face
 - Load and use pre-trained models: bert-base-uncased, distilbert-base, gpt2
 - Fine-tune on a classification task (e.g., sentiment, spam) using your own dataset
 - Understand tokenizers, positional encodings, attention weights
### 5. Lexical and Dense Retrieval
 - Implement TF-IDF and BM25 search using small document sets
 - Use Sentence-BERT to embed and retrieve text from a corpus
 - Setup FAISS index and return top-k relevant results for a query
### 6. Portfolio Output
 - A GitHub repo showing:
    - a notebook that fine-tunes BERT
    - a working retrieval system over a custom document set (e.g., Docker docs or Python docs)
    - basic API or CLI to query your system
 - Clear documentation with readme and structured code
Part 2: Advanced Stack (Learn On the Job or While Applying)
These are the competencies you can reasonably signal as “in progress” during application, while actively studying or prototyping.
### 7. Retrieval-Augmented Generation (RAG) Systems
 - Understand the RAG architecture: retriever + generator loop
 - Study the RAG paper (Lewis et al., 2020) and optionally ColBERT for comparison
 - Begin experimenting with Hugging Face’s RAGSequenceForGeneration or assemble a modular system with Sentence-BERT + GPT2
 - Integrate your retriever with a language model to answer questions grounded in documents
### 8. Evaluation Frameworks for LLMs
 - Learn standard metrics (BLEU, ROUGE, METEOR) and their limitations
 - Explore recent eval approaches: OpenAI Evals, TruLens, RAGAS
 - Begin building a pipeline to compare answer quality under different retrievers or prompts
 - Read about LLM-as-judge setups and try implementing one
### 9. Vector Databases & Scaling
 - Replace FAISS with a hosted vector DB (Weaviate, Pinecone, Qdrant)
 - Learn indexing, filtering, metadata search, hybrid scoring
 - Benchmark query latency and retrieval accuracy under load or dataset scale
### 10. Experimental Rigor
 - Design ablation studies: change retriever, chunking strategy, top-k, model size
 - Log metrics systematically
 - Begin using tools like Weights & Biases or MLflow for experiment tracking
### 11. Deployment Infrastructure
 - Dockerize your RAG system
 - Serve via FastAPI or Flask
 - Deploy locally or to cloud (GCP, AWS)
 - Optional: Add frontend via Streamlit or static HTML for demo purposes