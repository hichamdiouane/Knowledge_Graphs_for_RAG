# Knowledge Graphs for RAG

This project demonstrates how to build and use Knowledge Graphs for Retrieval-Augmented Generation (RAG) using LangChain, Neo4j, and Groq LLM.

## Features

- Text processing and chunking using LangChain
- Knowledge graph extraction using LLM
- Neo4j graph database integration
- RAG implementation with knowledge graph retrieval
- Query processing using Groq LLM

## Prerequisites

- Python 3.8+
- Neo4j database (local or cloud)
- Groq API key

## Installation

1. Clone the repository:
```bash
git clone https://github.com/hichamdiouane/Knowledge_Graphs_for_RAG.git
cd Knowledge_Graphs_for_RAG
```

2. Install required packages:
```bash
pip install langchain langchain-community langchain-groq transformers
pip install llama-index
pip install langchain-experimental
pip install neo4j
pip install python-dotenv
```

3. Set up environment variables:
Create a `.env` file in the project root with the following variables:
```
NEO4J_URI=your_neo4j_uri
NEO4J_USERNAME=your_neo4j_username
NEO4J_PASSWORD=your_neo4j_password
GROQ_API_KEY=your_groq_api_key
```

## Project Structure

```
Knowledge_Graphs_for_RAG/
├── .env                    # Environment variables
├── .gitignore             # Git ignore file
├── README.md              # Project documentation
└── notebook.ipynb         # Main implementation notebook
```

## Usage

1. Open and run the Jupyter notebook:
```bash
jupyter notebook notebook.ipynb
```

2. The notebook contains the following main steps:
   - Text loading and preprocessing
   - Knowledge graph extraction
   - Neo4j database integration
   - RAG implementation
   - Query processing

## Example Queries

The system can answer questions like:
- "Where does Sarah work?"
- "Who works for prismaticAI?"
- "Does Michael work for the same company as Sarah?"

## Security

- Sensitive credentials are stored in the `.env` file
- The `.env` file is excluded from Git tracking
- API keys and database credentials should be kept secure

## Dependencies

- langchain
- langchain-community
- langchain-groq
- transformers
- llama-index
- langchain-experimental
- neo4j
- python-dotenv

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
