# Book Recommendation System


PCSE25-72

This project implements a **hybrid book recommendation system** that intelligently combines content-based filtering and collaborative filtering to suggest books tailored to user preferences. The content-based component analyzes the textual metadata of books, including title, author, description, and genre, by creating a TF-IDF matrix and calculating cosine similarities to find books with similar content. Meanwhile, the collaborative filtering component uses user-book rating data to identify similar users through cosine similarity, building a user-item interaction matrix and recommending books highly rated by those similar users.

The hybrid model merges both approaches by assigning configurable weights (default: 0.5 each) to content and collaborative scores, generating a `hybrid_score` for each recommended item. This combined score ensures balanced and more accurate recommendations, especially in real-world scenarios where either content or user history may be limited. Additionally, the system gracefully handles cold-start problems (such as new users or books with insufficient ratings) by falling back to content-based recommendations.

The recommender is demonstrated using a small, hardcoded dataset of books and user ratings. Sample usage includes generating recommendations based on a specific book (`book_id`), a specific user (`user_id`), or both. The output is a DataFrame containing the recommended book IDs, titles, and their respective scores. This project uses Python and relies on popular libraries like `pandas`, `numpy`, and `scikit-learn`. It's ideal for educational purposes, prototypes, and understanding the mechanics behind hybrid recommendation engines.
