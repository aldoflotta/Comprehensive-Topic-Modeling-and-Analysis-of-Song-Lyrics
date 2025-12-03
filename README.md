# 🎵 Comprehensive Topic Modeling and Analysis of Song Lyrics

A large-scale computational analysis of 500,000 song lyrics using Natural Language Processing and unsupervised machine learning to uncover hidden thematic patterns and cultural trends from 1950 to 2024.

## 📊 Project Overview

This project explores the semantic structure and temporal evolution of song lyrics through advanced topic modeling techniques. By analyzing half a million songs spanning over seven decades, we reveal fascinating shifts in musical storytelling—from romantic idealism to materialistic realism.

### Key Findings

- **LDA outperforms** LSA and NMF with a coherence score of 0.4756
- **Traditional romance themes** have declined over time
- **Money, success, and explicit content** have surged since the 1990s
- **10 distinct thematic clusters** identified through unsupervised learning
- **Sentiment analysis** confirms topics carry predictable emotional signatures

## 🎯 Objectives

1. **Implementation** of three topic modeling algorithms (LDA, LSA, NMF)
2. **Quantitative evaluation** using coherence metrics
3. **Qualitative interpretation** of discovered themes
4. **Temporal trend analysis** across 74 years (1950-2024)
5. **Sentiment correlation** with thematic content

## 🛠️ Methodology

### Data Preprocessing Pipeline

- **Filtering**: English-language songs with valid metadata (1950-2024)
- **Tokenization**: Lowercase conversion, stopword removal, custom filler word filtering
- **Bigram Formation**: Detection of common phrases (e.g., "broken heart")
- **Lemmatization**: POS filtering (Nouns, Proper Nouns, Adjectives only)

### Topic Modeling Approaches

#### Unsupervised Learning
- **LDA** (Latent Dirichlet Allocation) - Probabilistic generative model
- **LSA** (Latent Semantic Analysis) - SVD-based dimensionality reduction
- **NMF** (Non-Negative Matrix Factorization) - Parts-based representation

#### Guided Topic Analysis
- Dictionary-based keyword matching
- Chunk processing for big data scalability
- Full dataset analysis (millions of songs)

### Evaluation Metrics

- **Cv Coherence Score** for topic quality assessment
- **VADER Sentiment Analysis** for emotional polarity
- **Temporal Aggregation** by decade

## 📈 Results

### Model Performance

| Model | Coherence Score (Cv) |
|-------|---------------------|
| **LDA** | **0.4756** |
| NMF | 0.4667 |
| LSA | 0.3764 |

### Discovered Topics

The LDA model identified 10 distinct themes:

- Party/Dance
- General/Time
- Religion/Elements
- Explicit/Aggressive
- Physical/Descriptive
- **Romantic Love** ❤️
- Existential/Life
- Music Genre/Style
- Hip-Hop/Slang
- Relationships

### Cultural Shifts (1950-2024)

- 📉 **Decline**: Traditional romantic imagery
- 📈 **Rise**: Explicit content, urban themes, materialism
- 🎯 **Peak**: Money/Success themes surge post-1990s

### Sentiment Distribution

- **Most Positive**: Party, Celebration, Love themes
- **Most Negative**: War, Violence, Heartbreak themes

## 💻 Technologies

- **Python 3.x**
- **NLTK** - Text preprocessing and stopword removal
- **Gensim** - Topic modeling (LDA) and phrase detection
- **Scikit-learn** - LSA and NMF implementations
- **Spacy** - Advanced NLP and lemmatization
- **VADER** - Sentiment analysis
- **pyLDAvis** - Interactive topic visualization
- **Pandas** - Data manipulation
- **Matplotlib/Seaborn** - Data visualization

## 📊 Dataset

**Source**: [Genius Song Lyrics with Language Information](https://www.kaggle.com/datasets/carlosgdcj/genius-song-lyrics-with-language-information)

- **Size**: ~9GB (500,000 songs analyzed)
- **Timespan**: 1950-2024
- **Language**: English
- **Features**: Lyrics, Artist, Year, Genre metadata

## 📝 Future Work

- Expand to **multilingual analysis** (non-English languages)
- Increase topic granularity (K > 10)
- Implement **dynamic topic modeling** for finer temporal resolution
- Genre-specific topic analysis
- Artist influence network analysis
- Deep learning approaches (BERT, transformers)

## 🎓 Academic Context

This project was developed as part of the Big Data and Text Analytics course at the University of Modena and Reggio Emilia.

**Author**: Aldo Flotta  
**Institution**: University of Modena and Reggio Emilia  

## 📚 References

1. Blei, D. M., Ng, A. Y., & Jordan, M. I. (2003). Latent dirichlet allocation. *Journal of Machine Learning Research*, 3, 993-1022.
2. Deerwester, S., et al. (1990). Indexing by latent semantic analysis. *Journal of the American Society for Information Science*, 41(6), 391-407.
3. Lee, D. D., & Seung, H. S. (1999). Learning the parts of objects by non-negative matrix factorization. *Nature*, 401(6755), 788-791.
