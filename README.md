# PCOS-Chatbot

<a>
  <img src="https://media.licdn.com/dms/image/v2/D562DAQFz5jG-BXhKlg/profile-treasury-image-shrink_160_160/profile-treasury-image-shrink_160_160/0/1727089737864?e=1727697600&v=beta&t=QUEIVoILEhTJ6S1lSXSjldIYEZ_1NQU3_4DDAZMsZuI">
</a>

# Medical Chatbot using RAG

• Data: PCOS.pdf

    • https://www.mdpi.com/2077-0383/12/4/1454
    
    • https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9440853/
    
    • https://academic.oup.com/jes/article/3/8/1545/5518341

• Frameworks:

    o Langchain - Pipeline
    
    o Llama - LLM Model
    
    o Sentence-Transformers - Embedding Model
    
    o Chroma - Vector Store

# Models

• LLM Model:

    o BioMistral-7B
    
• Embeddings Model:

    o PubMedBert-Base-embedding


# Process

Indexing

• Load the document and parse the text

• Divide text into chun - chunking

• Create embedding vectors for each chunk

• Store chunks and embeddings in the Vector Store

Querying

• Load LLM model

• Build application chain end-to-end model

• Query the chatbot

    o Pass query to Retriever
   
    o Retrieves relevant docs from Vector Store (KNN)
   
    o Pass both query and docs to LLM
   
    o Generate the response
