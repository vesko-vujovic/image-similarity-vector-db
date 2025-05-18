# Image similarity search using Vector Database

This repository provides a Jupyter notebook that demonstrates how to perform image similarity search using vector embeddings and a vector database.


### Overview

The notebook [`image-similarity-vector-db.ipynb`][^1] walks through the process of:

- Extracting feature vectors (embeddings) from images using a pre-trained neural network.
- Storing these embeddings in a vector database.
- Performing a similarity search to find images most similar to a given query image.

This approach is useful for duplicate detection, content-based image retrieval, and organizing large image datasets etc...

---

### Features

- Uses deep learning models to generate robust image embeddings.
- Demonstrates integration with a vector database for efficient similarity search.
- Provides end-to-end workflow: from image loading to querying similar images.

---

### Requirements

- Python 3.13
- Jupyter Notebook
- Deep learning libraries (e.g., PyTorch, depending on the feature extractor used)
- Vector database client library (`qdrant`)

---

### Getting Started

1. **Clone the repository:**

```bash
git clone https://github.com/vesko-vujovic/image-similarity-vector-db.git
cd image-similarity-vector-db
```

2. **Install dependencies:**
   
```Install the required Python packages (run the first cell of the notebook)```


4. **Launch the notebook:**

```bash
jupyter notebook image-similarity-vector-db.ipynb
```

---

### How It Works

- **Feature Extraction:**
Images are passed through a pre-trained neural network (such as ResNet) to obtain high-dimensional feature vectors that represent their content.
- **Embedding Storage:**
These vectors are stored in a vector database, which enables fast similarity search.
- **Similarity Search:**
Given a query image, its embedding is computed and compared to the stored vectors using a similarity metric (e.g., cosine similarity or L2 distance).
The most similar images are retrieved from the database.

---
![streamlit-ui](/posts/image-similarity-vector-db/image-similarity-ui.gif)

