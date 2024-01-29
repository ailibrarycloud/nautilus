# Nautilus by AI Library
Enterprise data intelligence platform

## Introduction
Nautilus is a Data Intelligence AI Assistant that uses multiple AI technologies enabling monitoring and managing of data groups by  
- creating a unified single source of truth derived from multiple data sources
- automating answers to frequently asked questions
- enabling research on unstructured data
- automating report generation
- enriching data in exisitng plaforms using APIs

#### Underlying AI Technologies and Concepts
- Generative AI (Text-to-text)
- Vector embeddings 
- Neural search
- Retrieval Augmented Generation (RAG)

## Product Architecture

Nautilus connects to relevant data sources and stores them flexibly, creating a single source of truth, ‘Unified Knowledge Base’. 

Data is sourced from 
- Public sites like Google News, YouTube (board meetings), Twitter
- Domain-specific Sites like Crunchbase, SEC etc
- Proprietary Information like Zum’s RFP Responses
- Responses received from FOIA requests

Knowledge is stored in a vector database in the form of vector embeddings. When queried, Nautilus retrieves relevant information from the database. This search is semantic in nature that understands context rather than keyword search. Once relevant information is retrieved, it is passed to an LLM to generate response in natural language.

![Nautilus Product Architecture](https://github.com/ailibrarycloud/nautilus/blob/main/nautilus-product-architecture.png?raw=true)

## Security 
- Nautilus can be deployed on a cloud server owned by the client
- Nautilus is LLM agnostic and can be used with privately hosted LLMs or enterprise LLMs
- Data can be air-gapped and poses no incremental cybersecurity risks
- Responses are traceable to Ground Truth
- Nautilus has entrprise access controls
- IP Liability exposure and data leaks can be prevented and/or limited
- Nautilus' architecture limits hallucinations
