# Data Augmentation Using TVAE (Tabular Variational AutoEncoder)

This project demonstrates how to use **Tabular Variational AutoEncoder (TVAE)** to **augment tabular datasets**, especially in scenarios involving **imbalanced or limited data**. By generating realistic synthetic data, TVAE helps enhance the performance of machine learning models.

---

## 🧬 What is TVAE?

TVAE (Tabular VAE) is a **deep generative model** that learns the joint distribution of tabular data using a variational autoencoder. It is particularly useful for:

* Generating high-quality synthetic tabular data
* Addressing data imbalance
* Preserving privacy while sharing data

We use the **SDV (Synthetic Data Vault)** library to implement TVAE.

---

## 📁 Dataset

The project supports any **structured tabular dataset** with numerical and categorical columns. In our case, the dataset used was:

* Custom CSV file (structure: customer churn, or other classification-type data)
* Dataset is preprocessed to handle missing values and encode categorical variables

---

## 🧠 Workflow

1. **Data Preprocessing**

   * Missing value handling
   * Label encoding or one-hot encoding
   * Feature scaling

2. **TVAE Model Training**

   * Using SDV’s `TVAE()` model to learn distribution
   * Fitting on real data

3. **Data Generation & Augmentation**

   * Generating synthetic rows
   * Appending to real data or using for separate evaluation

4. **Model Evaluation**

   * Training a classifier on real + synthetic vs real-only
   * Performance comparison using metrics

---

## ⚙️ Technologies Used

* Python
* Pandas / NumPy
* SDV (for TVAE)
* Scikit-learn
* Jupyter Notebook
* Matplotlib / Seaborn

## 📈 Evaluation Metrics

* Classifier Accuracy / F1 Score
* Quality of Synthetic Data (e.g., visual inspection, feature distributions)

---

## 💡 Use Cases

* Small datasets for machine learning
* Handling class imbalance in classification tasks
* Privacy-preserving synthetic data sharing

---

## 🤝 Contributions

Contributions are welcome. Please fork this repo and submit a pull request if you'd like to improve the code or add enhancements.

---

## 📜 License

MIT License

---

## 👤 Author

**Ibrahim Lodhi**
