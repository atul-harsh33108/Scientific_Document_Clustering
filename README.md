# Scientific_Document_Clustering

# ArXiv Paper Clustering with NLP, Dask, SciSpacy, and K-Means

## 📌 Project Overview
This project processes and clusters scientific research papers from the **ArXiv dataset** using **Dask**, **SciSpacy**, **TF-IDF**, and **K-Means clustering**. It includes interactive visualizations using **t-SNE, UMAP, and Plotly**.

## 🚀 Features
- **Efficient Dataset Handling**: Uses Dask to process large ArXiv JSON files.
- **Text Preprocessing**: Stopword removal, lemmatization, and tokenization with SciSpacy.
- **Feature Engineering**: Word count calculation and duplicate removal.
- **Dimensionality Reduction**: PCA for optimizing TF-IDF features.
- **Clustering & Visualization**:
  - K-Means clustering with optimal `k` selection.
  - Interactive t-SNE and UMAP plots with Plotly.

## 🛠️ Installation
To set up the environment, install the required dependencies:

```bash
pip install dask pandas numpy scikit-learn spacy scispacy click umap-learn plotly
pip install https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/releases/v0.5.4/en_core_sci_lg-0.5.4.tar.gz
```

## 📂 Dataset
- Source: **ArXiv** research paper dataset (JSON format).
- Filters papers published in **2024 and later**.
- Extracts abstracts for NLP processing.

## 📝 Processing Pipeline
1. **Data Loading**: Uses Dask for parallel processing.
2. **Preprocessing**: Tokenization, lemmatization, and stopword removal.
3. **Vectorization**: TF-IDF transformation.
4. **Dimensionality Reduction**: PCA to retain 95% variance.
5. **Clustering**: K-Means to group papers into meaningful topics.
6. **Visualization**: Generates interactive t-SNE & UMAP plots.

## 📊 Results
- **Clustered Papers** into meaningful research topics.
- **Visualized clusters** using interactive **Plotly** graphs.

## 📜 Usage
Run the main script to process and cluster the dataset:

```bash
python main.py
```

## 📈 Visualization Example
![t-SNE Visualization](assets/tsne_plot.png)

## 💡 Future Improvements
- Implement **BERT embeddings** for better clustering.
- Optimize **hyperparameters** for K-Means.
- Extend to **multi-year datasets** for trend analysis.

## 🤝 Contributing
Contributions are welcome! Feel free to submit **issues** or **pull requests**.

## 📄 License
This project is licensed under the **MIT License**.

---
🚀 **Created with passion for NLP and AI research!**

