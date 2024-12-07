# Multi-Document Summarization Using a Hybrid Extractive-Abstractive Approach

Multi-Document Summarization aims to condense a set of documents into a concise summary by extracting relevant information and filtering out redundancy. This project explores a **hybrid summarization approach**, combining **extractive** and **abstractive** techniques to generate high-quality summaries. 

We leverage **TextRank** for extractive summarization and a fine-tuned **BART (Bidirectional and Auto-Regressive Transformers)** model for abstractive summarization. By using the extractive summary as input to the abstractive model, the hybrid approach combines the strengths of both methods.

## Dataset
**WikiSum**: A dataset based on English Wikipedia. It consists of a Wikipedia topic (article title), non-Wikipedia reference documents, and the target Wikipedia article text.
   - [WikiSum on Papers with Code](https://paperswithcode.com/dataset/wikisum)

## Methodology
### 1. Extractive Summarization
We use the **TextRank algorithm**, a graph-based ranking algorithm, to identify the most important sentences based on sentence similarity.

### 2. Abstractive Summarization
We fine-tune a pre-trained **BART model**, known for its ability to produce smooth and coherent summaries.

### 3. Hybrid Approach
The extractive summaries from TextRank are used as input to the fine-tuned BART model, combining their strengths for improved clarity and informativeness.

### 4. Evaluation Metrics
- **ROUGE**: Measures lexical overlap between the generated and reference summaries.
- **BERTScore**: Evaluates semantic similarity between summaries.
- **METEOR**: Assesses how well critical information from the source text is captured.


## Getting Started
### Prerequisites
- Python 3.8+
- PyTorch
- Transformers library (Hugging Face)
- scikit-learn
- nltk
- numpy
- matplotlib

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/multi-document-summarization.git

2. Run ipynb file: CS6120.ipynb

### Results and Findings
Detailed results, metrics comparisons, and visualizations are documented in the project report.


### Team Members
Palkan Motwani
Savan Parmar
