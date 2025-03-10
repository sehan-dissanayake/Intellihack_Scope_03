# 🤖 Intellihack Scope 03 - AI Research Question Answering System

[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/downloads/)
[![HuggingFace](https://img.shields.io/badge/🤗-HuggingFace-yellow)](https://huggingface.co/)
[![Qwen](https://img.shields.io/badge/Model-Qwen%202.5--3B-green)](https://huggingface.co/Qwen/Qwen2.5-3B-Instruct)
[![License](https://img.shields.io/badge/License-MIT-purple)](LICENSE)

A specialized AI question-answering system for cutting-edge AI research topics. This project fine-tunes the Qwen 2.5-3B model and implements a Retrieval-Augmented Generation (RAG) system to provide accurate answers to technical questions about advanced AI research concepts.

![AI Research QA System](https://i.imgur.com/GPmqCdU.png)

## 📚 Covered Technical Topics

- **DualPipe**: Bidirectional pipeline parallelism for efficient LLM training
- **DeepSeek-V3**: Advanced 671B parameter Mixture-of-Experts architecture
- **Fire-Flyer File System (3FS)**: High-performance distributed storage for AI workloads
- **Expert Parallelism Load Balancing (EPLB)**: Dynamic workload distribution for MoE models

## 🧠 Project Components

The project implements a full AI research question-answering pipeline:

1. **Data Processing**: Chunking and cleaning technical documentation
2. **QA Pair Generation**: Creating high-quality training data
3. **Model Fine-tuning**: QLoRA fine-tuning of Qwen 2.5-3B
4. **RAG Implementation**: Vector database + fine-tuned model
5. **Comprehensive Evaluation**: Testing model performance and accuracy

## 📂 Project Structure
📁 Intellihack_Scope_03/
├── 📁 data/
│   ├── 📁 raw/                 # Store original documents here
│   ├── 📁 processed/           # Processed chunks
│   └── 📁 qa_pairs/            # Generated QA pairs
├── 📁 models/                  # For saving fine-tuned models
├── 📁 notebooks/
│   ├── 01_setup_and_exploration.ipynb
│   ├── 02_data_processing.ipynb
│   ├── 03_qa_pair_generation.ipynb
│   ├── 04_model_fine_tuning.ipynb
│   ├── 05_rag_implementation.ipynb
│   └── 06_evaluation.ipynb
├── 📁 src/                     # Source code modules
└── requirements.txt


## ⚙️ Setup and Installation

### System Requirements

- Python 3.9+ (tested with 3.13.1)
- CUDA-enabled GPU with 12GB+ VRAM (for fine-tuning)
- 16GB+ RAM
- 20GB+ free disk space

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Intellihack_Scope_03.git
   cd Intellihack_Scope_03

Create and activate a virtual environment:

bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
Install dependencies:

bash
pip install -r requirements.txt
Add technical documentation to data/raw/ directory:

bash
mkdir -p data/raw
# Add your .md and .txt files to this directory
🚀 Usage
Running the Notebooks
Execute the notebooks in sequence to process data, generate QA pairs, fine-tune the model, and implement the RAG system:

Data Exploration: Understand the technical documentation dataset

bash
jupyter notebook notebooks/01_setup_and_exploration.ipynb
Data Processing: Chunk and clean the documentation

bash
jupyter notebook notebooks/02_data_processing.ipynb
QA Pair Generation: Create training data

bash
jupyter notebook notebooks/03_qa_pair_generation.ipynb
Model Fine-tuning: Fine-tune Qwen 2.5-3B with QLoRA

bash
jupyter notebook notebooks/04_model_fine_tuning.ipynb
RAG Implementation: Set up and test the RAG system

bash
jupyter notebook notebooks/05_rag_implementation.ipynb
Evaluation: Test and compare model performance

bash
jupyter notebook notebooks/06_evaluation.ipynb
📊 Evaluation Results
The evaluation compares three approaches:

Base Qwen 2.5-3B-Instruct model
Fine-tuned model (QLoRA)
RAG system (fine-tuned model + retrieval)
Metrics include:

ROUGE and BLEU scores against reference answers
Error analysis and hallucination detection
Response length and content analysis
Topic-specific performance evaluation
🛠️ Technologies Used
LLM: Qwen 2.5-3B-Instruct
Fine-tuning: QLoRA (Quantized Low-Rank Adaptation)
Embeddings: sentence-transformers/all-MiniLM-L6-v2
Vector Store: FAISS
Frameworks: PyTorch, Transformers, LangChain, PEFT
Evaluation: ROUGE, BLEU, custom error analysis
👥 Contributors
Sehan Dissanayake (@sehan-dissanayake)
📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Qwen Team for the Qwen 2.5-3B model
Hugging Face for the Transformers library
LangChain for the RAG implementation framework
Code

This README provides a comprehensive overview of the Intellihack Scope 03 project with clear instructions for setup and usage. The formatting includes badges, emojis, and organized sections to make it more visually appealing and professional.
