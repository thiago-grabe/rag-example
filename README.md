
# Retrieval-Augmented Generation (RAG) System for Cars Dataset

This project demonstrates the creation of a **Retrieval-Augmented Generation (RAG)** system. It combines generative AI and vector similarity search to build a robust retrieval mechanism for car data.

## Project Overview

The system uses the following components:
1. **Generated Data**: Simulates a dataset of car details using OpenAI's GPT-3.5 Turbo model.
2. **Vectorization**: Converts car descriptions into vector representations using OpenAI's Embedding model.
3. **Vector Storage**: Stores and retrieves vectors efficiently with **Chroma**, an in-memory vector database.

The generated dataset includes the following attributes:
- **Name**: Car name
- **Price**: Car price
- **Engine**: Engine type
- **Description**: Detailed car description

## Installation

### Prerequisites
1. Install Python 3.8 or later.
2. Ensure you have `pip` installed.

### Install Requirements
Run the following command to install all necessary dependencies:

```bash
pip install -r requirements.txt
```

### Required Environment Variables
Create a `.env` file in the project directory with the following content:
```
OPENAI_API_KEY=<your-openai-api-key>
```

Replace `<your-openai-api-key>` with your actual OpenAI API key.

## How to Run the Notebook

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/thiago-grabe/rag-example.git
   cd rag-example
   ```

2. **Set Up the Environment**:
   Install the required packages by running:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**:
   Launch the notebook with:
   ```bash
   jupyter notebook
   ```

4. Open the notebook file and follow the instructions within.

## Key Features

- **Data Augmentation**: Generates a car dataset programmatically using OpenAI's GPT model.
- **Vectorization**: Embeds car descriptions into vector space for similarity search.
- **Retrieval**: Uses Chroma as the backend to fetch relevant vectors efficiently.

## Dependencies

The following dependencies are used in the project (also listed in `requirements.txt`):

- **langchain**: For handling LLM-based workflows.
- **chromadb**: Vector database for efficient retrieval.
- **transformers**: Hugging Face library for models and tokenizers.
- **sentence-transformers**: For embedding generation.
- **openai**: For GPT-based generation and embedding creation.
- **numpy**: Numerical computations.
- **ipywidgets** and **ipykernel**: For interactive notebook features.

## Example Outputs

An example entry in the dataset:
```
Name: Toyota Camry
Price: $25,000
Engine: Hybrid
Description: A reliable and fuel-efficient sedan with advanced features.
```

## Future Work

- Enhance the dataset generation pipeline.
- Implement advanced ranking algorithms for retrieved results.
- Integrate with external APIs for real-world datasets.

---

Feel free to modify this as per your project repository structure! Let me know if you need further enhancements.