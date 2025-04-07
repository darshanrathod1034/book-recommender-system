
# 📚 Book Recommender System

This project is a **Book Recommender System** that suggests books to users using two main techniques:

1. **Popularity-Based Filtering** — recommends top-rated books based on average rating and number of ratings.
2. **Collaborative Filtering** — recommends similar books based on user reading patterns using cosine similarity.

---

## 🚀 Features

- 📖 Recommend top 50 popular books (rated by 250+ users).
- 🤝 Recommend books similar to a given book using Collaborative Filtering.
- 🧠 Uses **cosine similarity** to find similar books.
- 📊 Filters active users and popular books for better performance.

---

## 📦 Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Jupyter Notebook / Colab

---

## 📁 Dataset Used

The project uses the **Book-Crossing Dataset** which includes:

- `Books.csv`: Book details (title, author, image)
- `Ratings.csv`: Ratings by users
- `Users.csv`: User demographic information (not used in this model)

---

## 🧠 How It Works

### 🔥 Popularity-Based Recommender

- Groups books by title and calculates:
  - Average rating
  - Number of ratings
- Filters books with 250+ ratings and sorts by highest average rating.

### 🤝 Collaborative Filtering Recommender

- Filters:
  - Users who have rated more than 200 books
  - Books with at least 50 ratings
- Creates a **pivot table** (books x users)
- Calculates **cosine similarity** between books
- Returns top 4 similar books to the input book

---

## 🛠️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/darshanrathod1034/book-recommender-system.git
cd book-recommender-system
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the notebook:

```bash
jupyter notebook
```

---

## 🖼️ Output Example

Here’s an example of the recommendations for `The Da Vinci Code`:
  function call:   recommend('1984')
```
[['Animal Farm',
  'George Orwell',
  'http://images.amazon.com/images/P/0451526341.01.MZZZZZZZ.jpg'],
 ["The Handmaid's Tale",
  'Margaret Atwood',
  'http://images.amazon.com/images/P/0449212602.01.MZZZZZZZ.jpg'],
 ['Brave New World',
  'Aldous Huxley',
  'http://images.amazon.com/images/P/0060809833.01.MZZZZZZZ.jpg'],
 ['The Vampire Lestat (Vampire Chronicles, Book II)',
  'ANNE RICE',
  'http://images.amazon.com/images/P/0345313860.01.MZZZZZZZ.jpg']]

---
2 recommend('You Belong To Me')

[['Loves Music, Loves to Dance',
  'Mary Higgins Clark',
  'http://images.amazon.com/images/P/0671758896.01.MZZZZZZZ.jpg'],
 ["I'll Be Seeing You",
  'Mary Higgins Clark',
  'http://images.amazon.com/images/P/0671888587.01.MZZZZZZZ.jpg'],
 ['Before I Say Good-Bye',
  'Mary Higgins Clark',
  'http://images.amazon.com/images/P/0671004573.01.MZZZZZZZ.jpg'],
 ["Daddy's Little Girl",
  'Mary Higgins Clark',
  'http://images.amazon.com/images/P/0743206045.01.MZZZZZZZ.jpg']]

## 📌 To-Do / Improvements

- Add a web interface (using Flask or Streamlit)
- Add user-based filtering
- Add personalized login system

---

## 🧑‍💻 Author

Darshan Rathod
📍 GH Patel College of Engineering  
Backend & AI Enthusiast
 
 teammate: deep tandel 
---

## 🌟 Show Your Support

Give this repo a ⭐️ if you like it and want more updates!
