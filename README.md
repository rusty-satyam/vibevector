# Vibe Vector: A Vector-Based Approach to Music Genre Analysis

This project implements a music genre classification system using a unique vector-based approach. By leveraging natural language processing techniques (TF-IDF) and geometric transformations, it analyzes songs based on three key descriptors: **Instrument**, **Mood**, and **Style**.

A key feature of this project is the **implementation of Principal Component Analysis (PCA) and K-Means Clustering algorithms from scratch using NumPy**, rather than relying on pre-built libraries.

## 🎵 Project Overview

The goal of this analysis is to determine if songs can be effectively grouped into genres based solely on descriptive keywords. The project follows the following pipeline:
1.  **Data Ingestion**: Processing raw CSV data containing song descriptors.
2.  **Vectorization**: Converting text keywords into numerical vectors using TF-IDF logic.
3.  **Dimensionality Reduction**: Implementing custom PCA to reduce high-dimensional data to 2D for visualization.
4.  **Feature Engineering**: Creating a composite "song vector" using weighted averages of the descriptor vectors.
5.  **Clustering**: Implementing custom K-Means clustering to group similar songs.
6.  **Evaluation**: Analyzing the results obtained.

## 📂 Dataset

The dataset used in this project was provided by the **Kharagpur Data Analytics Group (KDAG)**.

* **Format**: CSV
* **Features**:
    * `song_id`: Unique identifier.
    * `keyword_1`: Primary Instrument (e.g., Guitar, Synth, Piano).
    * `keyword_2`: Mood (e.g., Happy, Sad, Energetic).
    * `keyword_3`: Style (e.g., Fast, Acoustic, Distorted).
    * `genre`: The labeled genre (used for verification/analysis).

## 🛠️ Technologies Used

* **Python 3**
* **NumPy**: For manual implementation of algorithms (PCA, K-Means).
* **Pandas**: For CSV handling.
* **Matplotlib**: For visualizing clusters and PCA components.
* **Jupyter Notebook**: For interactive development and analysis.

## 💻 How to Run

1.  Clone the repository:
    ```bash
    git clone https://github.com/rusty-satyam/vibevector.git
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib jupyter
    ```
3.  Open the notebook:
    ```bash
    jupyter notebook vibevector/music-genre-analysis.ipynb
    ```
4.  Run all cells to see the analysis along with visualizations.