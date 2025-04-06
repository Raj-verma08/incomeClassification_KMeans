# K-Means Clustering on Income Data

This project applies **K-Means Clustering** to segment people based on their **age** and **annual income**. It uses a simple dataset (`income_KMeans.csv`) to explore how unsupervised learning can group individuals into clusters with similar characteristics.

## 📁 Dataset

The dataset contains the following columns:

- `Name`: Person's name
- `Age`: Age of the person
- `Income($)`: Annual income in dollars

### Sample

| Name    | Age | Income($) |
|---------|-----|-----------|
| Rob     | 27  | 70000     |
| Michael | 29  | 90000     |
| Mohan   | 29  | 61000     |

---

## 📊 Objective

Use **K-Means clustering** to group individuals into **3 distinct clusters** based on their **age** and **income**.

---

## 🧪 Steps Involved

1. **Data Preprocessing**:
   - Loaded the CSV dataset using pandas
   - Explored basic stats and plotted the data using matplotlib

2. **Initial Clustering**:
   - Applied KMeans (with `n_clusters=3`) directly on raw `Age` and `Income` data
   - Visualized the results with different colors per cluster

3. **Cluster Center Visualization**:
   - Plotted cluster centers with purple star markers
   - Used `km.cluster_centers_` to get centroids

4. **Data Normalization**:
   - Used `MinMaxScaler` from `sklearn.preprocessing` to normalize both `Age` and `Income`
   - Helped improve clustering performance and scale handling

---

## 📉 Clustering Results

After clustering:

- Cluster 0: Mostly younger people with lower income
- Cluster 1: Older people with higher income
- Cluster 2: Middle-aged people with moderate income

---

## 🧰 Technologies Used

- Python
- pandas
- matplotlib
- scikit-learn

---

## 📎 How to Run

1. Clone the repository
2. Make sure you have the dependencies installed:
   ```bash
   pip install pandas matplotlib scikit-learn
