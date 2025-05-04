# 🛍️ Product Recommendation System

This project is a content-based recommendation system built using fashion product data.  
Given a product ID, the model suggests similar products based on category, type, color, and usage.

## 📁 Dataset
- Source: Provided CSV (`styles.csv`)
- Size: ~44,000 rows
- Features: `gender`, `masterCategory`, `subCategory`, `articleType`, `baseColour`, etc.

## 🧠 How It Works
1. Combines product features into a single string.
2. Applies **TF-IDF vectorization** to convert text to numeric form.
3. Uses **Nearest Neighbors (cosine similarity)** to find the most similar products.

## 📌 Libraries Used
- `pandas`
- `scikit-learn`
- `numpy`

## 🚀 How to Use
1. Load the notebook in Google Colab.
2. Upload `styles.csv`
3. Run all cells.
4. Use `get_recommendations(product_id)` to find similar products.

Example:

```python
get_recommendations(15970)
