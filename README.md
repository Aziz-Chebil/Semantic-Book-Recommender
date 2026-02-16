# 📚 Semantic Book Recommender

An intelligent book recommendation system powered by Large Language Models (LLMs) and semantic search. This project leverages natural language processing, vector embeddings, and sentiment analysis to help users discover books based on meaning and emotional tone rather than just keywords.

![Semantic Book Recommender](semantic%20book%20recommender.png)

## 🌟 Features

- **Semantic Search**: Find books using natural language queries (e.g., "a book about a person seeking revenge")
- **Vector Database**: Efficient similarity search using ChromaDB and OpenAI embeddings
- **Zero-Shot Classification**: Automatic categorization of books as Fiction or Non-Fiction without training data
- **Sentiment Analysis**: Filter books by emotional tone (suspenseful, joyful, sad, etc.)
- **Interactive Web Interface**: User-friendly Gradio dashboard for real-time recommendations
- **Smart Filtering**: Combine semantic search with category and emotional tone filters

## 🏗️ Project Architecture

The system consists of five main components:

1. **Data Exploration & Cleaning** (`data-exploration.ipynb`)
   - Load and analyze the book dataset
   - Handle missing values and data inconsistencies
   - Feature engineering and preprocessing

2. **Vector Search** (`vector-search.ipynb`)
   - Convert book descriptions into vector embeddings using OpenAI API
   - Build and manage ChromaDB vector database
   - Implement semantic similarity search

3. **Text Classification** (`text-classification.ipynb`)
   - Use zero-shot classification with Hugging Face transformers
   - Classify books as Fiction or Non-Fiction
   - Create filterable categories for recommendations

4. **Sentiment Analysis** (`sentiment-analysis.ipynb`)
   - Extract emotional tones from book descriptions using LLMs
   - Generate emotional scores (suspense, joy, sadness, etc.)
   - Enable mood-based book filtering

5. **Web Application** (`gradio-dashboard.ipynb` / `main.py`)
   - Interactive Gradio interface for user queries
   - Real-time book recommendations with cover images
   - Filter options for category and emotional tone

## 🛠️ Tech Stack

- **Language**: Python 3.11+
- **LLM & Embeddings**: OpenAI API, Hugging Face Transformers
- **Vector Database**: ChromaDB
- **Framework**: LangChain
- **Web Interface**: Gradio
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn


## 📊 Dataset
This project uses the **7K Books Dataset** from Kaggle, which includes:

- Book titles and subtitles
- Authors
- Descriptions
- ISBN-13
- Categories
- Ratings and review counts
- Cover image URLs
- Publication years

## 🔍 How It Works

1. **Text Embeddings**: Book descriptions are converted into high-dimensional vectors using OpenAI's embedding models
2. **Vector Storage**: Embeddings are stored in ChromaDB for efficient similarity search
3. **Query Processing**: User queries are embedded and compared against the database using cosine similarity
4. **Smart Filtering**: Results are filtered by category and emotional tone based on user preferences
5. **Ranking**: Books are ranked by semantic similarity and presented with metadata

## 🙏 Acknowledgments

- Based on the freeCodeCamp tutorial "Build a Semantic Book Recommender with LLMs"
- Dataset sourced from Kaggle
- Built with OpenAI, Hugging Face, and LangChain

⭐ If you find this project helpful, please consider giving it a star on GitHub!

