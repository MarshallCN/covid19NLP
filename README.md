# COVID-19 NLP Analysis

This project applies Natural Language Processing (NLP) techniques to COVID-19 related textual data, aiming to extract meaningful insights from news articles and tweets.

## Project Structure

The repository includes the following key components:

- **Data Sources**:
  - `IEEE_news/`: Contains news articles related to COVID-19.
  - `IEEE_tweets/`: Contains tweets discussing COVID-19.

- **Notebooks**:
  - `Topic_Modelling.ipynb`: Implements topic modeling to identify prevalent themes in the text data.
  - `Topic_Sentiment.ipynb`: Analyzes sentiment associated with different topics.
  - `Word_Embedding.ipynb`: Explores word embedding techniques to capture semantic relationships.

## Detailed Notebook Summaries

### 1. Topic_Modelling.ipynb

**Objective**: This notebook aims to perform topic modeling on COVID-19 related textual data to identify the main themes present in the content.

**Key Components**:

- **Data Loading and Preprocessing**: Loading data from the `IEEE_news/` and `IEEE_tweets/` directories, followed by cleaning and preprocessing steps such as removing stop words, punctuation, and performing lemmatization.

- **Topic Modeling**: Utilizing the Latent Dirichlet Allocation (LDA) model to determine the optimal number of topics and extract key terms associated with each topic.

- **Visualization**: Employing visualization tools to display relationships between topics and the weight of keywords within each topic, facilitating a better understanding of topic distribution and interconnections.

### 2. Topic_Sentiment.ipynb

**Objective**: This notebook focuses on analyzing the sentiment associated with each identified topic, evaluating public attitudes toward various themes.

**Key Components**:

- **Topic Distribution Analysis**: Building upon previous topic modeling results to assess the prevalence of each topic within the dataset.

- **Sentiment Analysis**: Classifying the sentiment of texts under each topic as positive, negative, or neutral.

- **Results Visualization**: Presenting the sentiment distribution for each topic through charts, offering a clear depiction of public sentiment toward different themes.

### 3. Word_Embedding.ipynb

**Objective**: This notebook explores the application of word embedding techniques to capture semantic relationships in COVID-19 related textual data.

**Key Components**:

- **Word Embedding Model Training**: Training a Word2Vec model on the preprocessed text data to generate vector representations of words.

- **Similar Words Analysis**: Utilizing the trained word embedding model to identify and analyze words with similar semantic meanings.

- **Visualization**: Applying dimensionality reduction techniques, such as t-SNE, to project high-dimensional word vectors into two-dimensional space, creating scatter plots that illustrate semantic distances and clustering of words.

## Getting Started

### Prerequisites

- **Python**: Ensure Python is installed. Download from [python.org](https://www.python.org/).
- **Jupyter Notebook**: Install using pip:
  ```bash
  pip install notebook
  ```

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/MarshallCN/covid19NLP.git
   cd covid19NLP
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   *Note: If `requirements.txt` is absent, manually install packages such as `numpy`, `pandas`, `scikit-learn`, `nltk`, `gensim`, and `matplotlib`.*

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   Open the desired notebook (e.g., `Topic_Modelling.ipynb`) in your browser.

## Usage

- **Data Preparation**: Load and preprocess data from the `IEEE_news/` and `IEEE_tweets/` directories.
- **Topic Modeling**: Run `Topic_Modelling.ipynb` to identify key topics in the dataset.
- **Sentiment Analysis**: Execute `Topic_Sentiment.ipynb` to assess sentiments associated with each topic.
- **Word Embeddings**: Utilize `Word_Embedding.ipynb` to visualize semantic similarities between words.

## License

This project is licensed under the MIT License.
