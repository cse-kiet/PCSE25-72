# Title of Project: Book Recommendation System

## Team Members:
1. Tripti Singh (2100290100175  sec-C)
2. Urvi Gupta (2100290100177  sec-C)
3. Vidyush Singh (2100290100185  sec-C)

## Steps for Execution:
1. Import required libraries for data handling, text processing, and similarity computation.

2. Define the BookRecommender class with methods for preprocessing, vectorization, and recommendation.

3. Instantiate the class with book data (dict or DataFrame).

4. Convert input data to a DataFrame if it's a dictionary.

5. Fill in missing values in description, author, and optionally genre.

6. Combine title, author, description, and genre into a single combined_features text field.

7. Initialize a TF-IDF vectorizer and fit-transform combined_features into a sparse matrix.

8. Compute cosine similarity between all book vectors using linear_kernel.

9. Call recommend_books() with a book title and number n.

10. Find the index of the input book title in the dataset (case-insensitive match).

11. Retrieve similarity scores of the selected book with all others.

12. Sort similarity scores in descending order, excluding the book itself.

13. Return top n most similar books as recommendations.

## Checklist:
1. Final Project Report
2. Certificate VII Semester (Dated: December 2024).
3. Certificate VIII Semester (Dated: May 2025).
4. Synopsis
5. Final Presentation
6. Source Code
7. Database dump (.sql file)
8. If a web project, then a Docker file for deployment
9. README (This file)
