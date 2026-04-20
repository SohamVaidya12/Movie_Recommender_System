# 🎬 CineFusion AI

CineFusion AI is a **genre-based movie recommendation system** built using **Python, Scikit-learn, Pandas, and Gradio**.  
The system allows users to choose between **Hollywood** and **Bollywood** movie industries and get recommendations based on their selected **genre**.

This project uses **TF-IDF Vectorization** and **Cosine Similarity** to recommend movies with similar genre patterns.

---

## 📌 Objective

The main objective of this project is to develop an interactive **movie recommendation system** that can suggest movies to users based on their preferred **genre** and selected **industry**.

The system is designed to:

- Recommend movies based on **genre similarity**
- Support recommendations from both **Hollywood** and **Bollywood**
- Provide an easy-to-use and attractive **user interface**
- Help users quickly discover movies matching their interests
- Demonstrate the practical use of **machine learning techniques** in recommendation systems

---

## 🚀 Features

- 🎭 Genre-based movie recommendation
- 🌍 Dual industry support:
  - Hollywood
  - Bollywood
- 🤖 Recommendation using **TF-IDF + Cosine Similarity**
- 🎬 Trailer button for recommended movies
- 🎨 Interactive and user-friendly **Gradio interface**
- 🔢 User-controlled number of recommendations
- 🎲 Surprise genre option

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **Scikit-learn**
- **Gradio**
- **TF-IDF Vectorizer**
- **Cosine Similarity**

---
---

## 🧠 Techniques Used

This project is based on a **content-based recommendation approach**.  
The following techniques are used in the system:

### 1. Content-Based Filtering
Content-based filtering recommends items based on the features of the items themselves.  
In this project, movies are recommended based on their **genre information**.

**Example:**  
If a user selects **Action**, the system recommends movies whose genre patterns are similar to action-based movies.

---

### 2. TF-IDF Vectorization
**TF-IDF (Term Frequency - Inverse Document Frequency)** is used to convert text data into numerical vectors.

In this project:
- The **genres** column is treated as text
- TF-IDF converts movie genres into machine-readable numerical form
- This helps the system understand genre similarity mathematically

**Why used?**  
Because machine learning models cannot directly work with raw text values like `Action|Thriller|Drama`.

---

### 3. Cosine Similarity
Cosine Similarity is used to measure the similarity between two vectors.

In this project:
- One vector represents the selected genre
- Other vectors represent genres of all movies in the dataset
- The movies with the highest similarity score are recommended

**Why used?**  
Because it is simple, efficient, and well-suited for text-based recommendation tasks.

---

### 4. Data Preprocessing
Before recommendation:
- Missing values in the `genres` column are handled
- Titles are cleaned
- Year values are extracted from movie titles
- Genres are standardized for better matching

## 📂 Project Structure

```bash
CineFusion-AI/
│
├── app.py
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── movie.csv
│   └── bollywood_movies_only_2200.csv
│
├── notebooks/
│   └── project.ipynb
│
└── assets/
    └── demo_screenshot.png
