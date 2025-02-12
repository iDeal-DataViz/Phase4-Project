# Phase4-Project
# Movie Recommendation System

## Overview
This project implements a **Movie Recommendation System** that suggests the top 5 movies to users based on their ratings. It combines **Collaborative Filtering** and **Content-Based Filtering** to provide personalized recommendations and solve the cold-start problem for new users.

## Features
- **Collaborative Filtering**: Uses Singular Value Decomposition (SVD) to model latent features of users and movies.
- **Content-Based Filtering**: Leverages movie genres to compute similarity using TF-IDF and Cosine Similarity.
- **Hybrid Approach**: Integrates collaborative and content-based methods for better accuracy and scalability.
- **Dynamic Recommendations**: Allows users to input ratings dynamically and receive personalized suggestions.

## Data Sources
The system uses the **MovieLens dataset**, which includes:
- `ratings.csv`: User ratings for movies.
- `movies.csv`: Titles and genres of movies.

## Technical Stack
- **Programming Language**: Python
- **Libraries**:
  - `pandas` and `numpy` for data manipulation.
  - `scikit-learn` for machine learning and evaluation metrics.
  - `scipy` for matrix factorization.
  - `TF-IDF` for feature extraction and similarity computation.
- **Presentation**: PowerPoint for business stakeholders.

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Place the dataset files (`ratings.csv`, `movies.csv`) in the `data/` folder.

## Usage
1. Run the Jupyter Notebook `Movie_Recommendation_System.ipynb` to explore the workflow and generate recommendations.
2. Modify `dynamic_user_recommendation` for custom user input.
3. Use the `optimized_content_based_recommendation` function for cold-start scenarios.

## Results
- **Collaborative Filtering Performance**:
  - RMSE: 1.998
  - MAE: 1.539
- **Hybrid Model Performance**:
  - RMSE: 1.85
  - MAE: 1.45

### Example Recommendations
- For a new user who rates:
  - `Star Wars: Episode IV - A New Hope`: 5.0
  - `Fargo`: 4.5

**Recommendations:**
1. **The Godfather**
2. **Inception**
3. **Pulp Fiction**

## Folder Structure
```
Movie_Recommendation_System/
├── data/
│   ├── ratings.csv
│   ├── movies.csv
├── notebooks/
│   ├── Movie_Recommendation_System.ipynb
├── presentation/
│   ├── Movie_Recommendation_System_Presentation.pptx
├── README.md
├── requirements.txt
```

## Future Improvements
- **Deployment**: Convert into a web application using Django or Flask.
- **Real-Time Recommendations**: Integrate with streaming platforms for live suggestions.
- **Expanded Dataset**: Incorporate additional metadata like actors, directors, and reviews for richer recommendations.

## License
This project is licensed under the MIT License.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

