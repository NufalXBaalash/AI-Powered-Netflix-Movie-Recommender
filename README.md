🚀 README.md — AI Movie Recommender System
# 🎬 AI-Powered Netflix Movie Recommender System

This project is an intelligent movie recommendation system built using Google Gemini for semantic text embeddings and FAISS (by Meta) for fast similarity search. It analyzes Netflix movie descriptions and suggests similar content — even for custom movie inputs.

## 📌 Features

- 🔍 Semantic search over Netflix titles
- 🧠 Uses Google Gemini's `embedding-001` model
- ⚡ Fast similarity search using FAISS
- ✨ Supports custom movie queries (even if not in the dataset)
- 📊 Real Netflix dataset with detailed metadata
- 🐍 Built entirely in Python

## 📂 Dataset

The dataset used is [`netflix_titles.csv`] which includes:
- Title, Type (Movie/TV Show), Director, Cast
- Release Year, Description, Genre (`listed_in`)

## 🔧 How It Works

1. Generate a rich textual representation for each movie
2. Use Gemini API to convert each text into a 768-dimensional embedding
3. Store all embeddings in a FAISS index for fast retrieval
4. For any movie (real or described by the user), generate an embedding
5. Search for the top 5 most similar embeddings using FAISS
6. Display the most relevant movie recommendations

## 🛠 Tech Stack

- Python
- Pandas & NumPy
- Google Gemini API
- FAISS
- Google Generative AI SDK (for embedding calls)
- Requests

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/YourUsername/AI-Movie-Recommender.git
cd AI-Movie-Recommender
````

2. Install the required packages:

```bash
pip install -r requirements.txt
```

3. Add your Gemini API Key to the script:

```python
GEMINI_API_KEY = "your_key_here"
```

4. Run the notebook:

```bash
jupyter notebook main.ipynb
```

Or run the Python script version if available.

## 📹 Demo

🎥 YouTube Video: [Watch Demo](https://youtu.be/SeuIDjOlyJ4)

## 📁 Project Structure

```
AI-Movie-Recommender/
├── main.ipynb                # Full notebook with all steps
├── netflix_titles.csv        # Dataset used
├── index                     # Saved FAISS index
├── requirements.txt          # Python dependencies
└── README.md                 # You're here!
```

## 🧠 Sample Use Case

You can write a custom movie description like this:

```text
Title: IT  
Type: Movie  
Director: Andy Muschietti  
Cast: Bill Skarsgård, Jaeden Martell  
Released: 2017  
Genres: Horror  
Description: In the summer of 1989, a group of kids unite to defeat a shape-shifting monster that takes the form of a clown.
```

…and the model will recommend similar horror movies from Netflix!

## 📬 Contact

Feel free to reach out if you're interested in collaborating or have feedback.

🔗 LinkedIn: \ [Ahmed Baalash](https://www.linkedin.com/in/ahmed-baalash/)
💻 GitHub: \ [NufalXBaalash](https://github.com/NufalXBaalash)

## 🏷️ Tags

AI · Recommender Systems · Gemini · FAISS · Python · Netflix · NLP · Machine Learning · Embeddings

---

© 2025 Aseer — All rights reserved.

