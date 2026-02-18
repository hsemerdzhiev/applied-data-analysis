# 📊 Advanced Data Analysis & Machine Learning Case Studies

This repository presents **three end-to-end data science projects** addressing real-world problems in **sensor analytics, graph-based classification, and recommender systems**. Each notebook focuses on **comparing multiple techniques**, evaluating their trade-offs, and extracting **actionable insights**.

The projects emphasize not only *how* algorithms work, but *when* and *why* they should be used.

---

## 🚀 Why This Repository Matters

This repository demonstrates:
- Practical problem formulation
- Algorithm selection and comparison
- Interpretation of results
- Applicability to real-world systems (IoT, content platforms, dating apps)

All analyses are reproducible and clearly documented.

---

## 🛠 Technologies & Tools

- **Programming:** Python 3.11  
- **Data Analysis:** NumPy, pandas, SciPy  
- **Visualization:** Matplotlib, Seaborn, NetworkX  
- **Machine Learning & Models:** scikit-learn, gensim  
- **Specialized Methods:**  
  - **Dynamic Time Warping (DTW)**  
  - **Principal Component Analysis (PCA)**  
  - **Random Walks & Spectral Embeddings**  
  - **MinHashing & Non-negative Matrix Factorization (NMF)**  
- **Environment Management:** `venv`, `requirements.txt`  
- **Version Control:** Git & GitHub

---

## 📁 Project Structure

| Folder/File | Description |
|-------------|-------------|
| 📂 data-analysis-notebooks/ | Root repository |
| ├── 📂 Anomalies-Detection/ | Sensor analysis notebook project |
| │ ├── 📂 Resources/ | Folder where data is stored |
| │ └── 📄 sensor-signals-analysis.ipynb | Jupyter notebook for sensor data analysis |
| ├── 📂 network_analysis/ | Network exploration notebook project |
| │ ├── 📂 Resources/ | Folder where data is stored |
| │ └── 📄 network_analysis.ipynb | Jupyter notebook for network analysis |
| ├── 📂 recommender_systems/ | Recommender systems notebook project |
| │ ├── 📂 Resources/ | Folder where data is stored |
| │ └── 📄 recommender_systems.ipynb | Jupyter notebook for recommendation analysis |
| ├── .gitignore | Ignore venv, __pycache__, and notebook checkpoints |
| ├── 📄 README.md | Main repo README |
| └── 📄 requirements.txt | Python dependencies with exact versions |
 
- Each folder contains a single notebook, its resources and predictions made from the given algorightms.  
- Notebooks are **self-contained** and can be executed independently.

---

## 📈 Project 1: Sensor Signal Analysis & Anomaly Detection  
**Notebook:** `sensor-signals-analysis.ipynb`

### 🎯 Problem
Sensor-based systems must detect abnormal behavior early to prevent failures. These anomalies can appear as:
- **Point anomalies** (single outliers),
- **Contextual anomalies** (abnormal in a specific context),
- **Collective anomalies** (abnormal sequences).

### 🧠 Methods Used
- **Dynamic Time Warping (DTW):**  
  Captures similarity between time series under temporal distortions.
- **Principal Component Analysis (PCA):**  
  Reduces dimensionality and highlights dominant signal patterns.
- **Anomaly Detection Techniques:**  
  Applied to detect point, contextual, and collective anomalies in sensor signals.

### 🔍 Final Findings
- DTW is highly effective for detecting **collective anomalies** where temporal alignment matters.
- PCA-based approaches efficiently expose **global deviations** and point anomalies.
- Combining DTW and PCA provides a more complete anomaly detection strategy than using either alone.

### 💡 Skills Demonstrated
Time-series analysis, anomaly detection, dimensionality reduction, signal interpretation.

---

## 🌐 Project 2: Article Classification via Network Representations  
**Notebook:** `node-classifying.ipynb`

### 🎯 Problem
Articles form implicit networks based on references, similarity, or shared metadata. The goal is to **classify articles into three distinct categories** using graph-based representations.

### 🧠 Methods Compared
- **Random Walk-based Node Representations:**  
  Capture local structural and semantic relationships.
- **Spectral Embeddings:**  
  Encode global graph structure via Laplacian eigenvectors.

### 🔍 Final Findings
- Random walk representations perform better when article categories are **locally clustered**.
- Spectral embeddings excel when **global graph structure** separates classes.
- Classification performance depends strongly on how category information is distributed across the graph.

### 💡 Skills Demonstrated
Graph learning, node embeddings, multi-class classification, experimental evaluation.

---

## 🤝 Project 3: Dating App Recommender System  
**Notebook:** `recommender-systems.ipynb`

### 🎯 Problem
Dating apps require recommendations that are:
- Accurate
- Scalable
- Sensitive to user preferences and sparsity

The objective is to generate meaningful match recommendations from user interaction data.

### 🧠 Methods Compared
- **MinHashing (Locality Sensitive Hashing):**  
  Efficient similarity approximation for large user bases.
- **Non-negative Matrix Factorization (NMF):**  
  Learns latent user–user and user–item preferences.

### 🔍 Final Findings
- MinHashing scales efficiently and is well-suited for **large, rapidly growing platforms**.
- NMF captures deeper latent compatibility signals, producing **higher-quality recommendations**.
- A hybrid approach balances scalability and recommendation accuracy in real-world dating apps.

### 💡 Skills Demonstrated
Recommender systems, matrix factorization, similarity search, applied ML for consumer products.

---

## 🚀 How to Run

1. Clone the repo
2. Create a virtual environment using **bash**:
   ```bash
   python -m venv venv
   source venv/Scripts/activate  # or venv\Scripts\activate in cmd
3. Install dependencies:
    ```bash
    pip install --upgrade pip
    pip install -r requirements.txt
