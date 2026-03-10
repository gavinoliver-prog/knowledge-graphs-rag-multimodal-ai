# Knowledge Graphs, Multimodal AI and RAG

I created this repository containing a collection of practical notebooks exploring modern data science and artificial intelligence techniques relevant to computational biology and biomedical research.

The material progresses from graph-based data modeling and semantic knowledge graphs to multimodal foundation models and retrieval-augmented generation (RAG). The goal is to provide hands-on examples that illustrate how these technologies can be applied to scientific data, literature, and translational research workflows.

Topics covered include:

- knowledge graph construction and analysis  
- semantic graphs using RDF and SPARQL  
- foundation model embeddings  
- multimodal machine learning workflows  
- retrieval-augmented generation (RAG) systems  
- vector databases for embedding search  

The notebooks are designed as guided learning exercises and lightweight prototypes rather than production systems. Each notebook focuses on illustrating core ideas with minimal infrastructure so the underlying concepts remain clear.

Together they form a practical introduction to several modern AI approaches increasingly used in biomedical data science, computational biology, and translational research.

---

## Python Environment Setup

The Python notebooks use a virtual environment managed with **uv** and dependencies listed in `python/requirements.txt`.

```bash
cd python
uv venv
source .venv/bin/activate
uv pip install -r requirements.txt
jupyter notebook


---

# Knowledge Graphs

### 06_graph_thinking_in_python.ipynb
Introduces the core concepts of graph-based data structures. Covers nodes, edges, graph traversal, and basic graph analysis using Python examples to build intuition for relationship-driven data.

### 07_building_knowledge_graphs_networkx.ipynb
Demonstrates how to construct practical knowledge graphs using the NetworkX library. Shows how entities and relationships can be represented programmatically and explored using graph operations.

### 08_querying_bio_knowledge_graphs.ipynb
Explores common graph queries including neighbors, shortest paths, and subgraph extraction. Uses biological examples such as gene–pathway and drug–target relationships.

### 09_building_knowledge_graphs_from_biological_tables.ipynb
Shows how real-world knowledge graphs are constructed from tabular data sources. Covers entity normalization, typed nodes, relationship edges, and exporting graph relationships as triples.

---

# Semantic Graphs (RDF and SPARQL)

### 10_rdf_and_triples_in_python.ipynb
Introduces RDF (Resource Description Framework) graphs and triple-based data representation using the `rdflib` library. Demonstrates namespaces, URIs, literals, and serialization formats.

### 11_sparql_querying.ipynb
Teaches the fundamentals of SPARQL queries for retrieving information from RDF graphs. Includes pattern matching, filtering, aggregation, and multi-hop semantic queries.

### 12_biomedical_ontologies_semantic_kgs.ipynb
Introduces biomedical ontologies and how semantic knowledge graphs integrate standardized identifiers for genes, diseases, pathways, and drugs. Demonstrates ontology-driven relationships in RDF graphs.

---

# Foundation Models and Multimodal AI

### 13_foundation_model_embeddings_in_python.ipynb
Introduces embedding generation using pretrained transformer models. Demonstrates how text inputs are converted into vector representations that can be compared, visualized, and analyzed.

### 14_image_foundation_models_embeddings.ipynb
Uses a pretrained vision transformer to convert images into embedding vectors. Demonstrates similarity analysis and visualization of image embedding spaces.

### 15_multimodal_integration_embeddings.ipynb
Combines embeddings from multiple data modalities such as image features and molecular variables. Demonstrates how multimodal feature spaces can be used for predictive modeling.

### 16_translational_multimodal_pipeline.ipynb
Simulates a translational biomedical AI workflow integrating image embeddings, molecular features, and clinical variables to predict outcomes such as drug response.

### 17_tiny_self_supervised_model_demo.ipynb
Illustrates the core training idea behind foundation models using a small self-supervised learning example. Demonstrates how encoders learn embeddings through contrastive-style objectives.

---

# Retrieval-Augmented Generation (RAG)

### 18_rag_fundamentals.ipynb
Introduces the architecture of retrieval-augmented generation systems. Covers document chunking, embedding generation, vector similarity retrieval, and prompt construction.

### 19_building_a_simple_retriever.ipynb
Builds a reusable document retrieval pipeline. Demonstrates chunking strategies, embedding generation, similarity search, and inspection of retrieval rankings.

### 20_full_rag_pipeline_prompt_design.ipynb
Extends retrieval pipelines to include language model generation. Demonstrates prompt construction, prompt engineering experiments, and inspection of hallucinations versus grounded responses.

### 21_scientific_pdf_rag.ipynb
Implements a RAG system for scientific papers. Demonstrates PDF ingestion, text extraction, chunking, embedding, and answering domain-specific questions from research documents.

---

# Vector Databases

### 22_vector_databases.ipynb
Introduces vector databases used for scalable embedding storage and retrieval. Demonstrates how embeddings are indexed, searched, and retrieved efficiently in modern AI systems such as RAG pipelines and semantic search applications.

---

# Summary

Together, these notebooks introduce a range of modern computational techniques used in biomedical AI and data science, including:

- knowledge graph construction and analysis  
- semantic data integration with RDF and SPARQL  
- multimodal foundation model workflows  
- retrieval-augmented generation for scientific literature  
- vector databases for large-scale embedding search
