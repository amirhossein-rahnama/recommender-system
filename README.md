
# Recommender Extender

## Overview

Welcome to the Recommender Extender project! This project aims to enhance the music discovery experience for 1980s radio enthusiasts by developing a sophisticated content-based recommender system (CBRS). By leveraging natural language processing (NLP) and machine learning techniques, we strive to balance the nostalgia of familiar 1980s hits with the excitement of discovering lesser-known tracks from the same era.

## Project Structure

The project is organized into the following main sections:

1. **Feature Acquisition**: Gathering various features from different sources like charts, Last.fm, lyrics, and Spotify audio analysis to enrich our dataset.
2. **Feature Engineering**: Processing and refining the acquired features, including dataset reduction and the application of NLP techniques.
3. **Content-Based Recommender System (CBRS)**: Developing the backend and frontend of the recommender system, with detailed methodologies for similarity metrics and feature weighting.
4. **Results**: Conducting surveys to evaluate the CBRS, analyzing user feedback, and refining the system based on the findings.
5. **Conclusion and Future Work**: Summarizing the project achievements and outlining potential future improvements.

## Feature Acquisition

We gathered features from various sources to create a comprehensive dataset for our CBRS:

- **Charts**: Data from German charts in the 1980s.
- **Last.fm**: User-generated data including playcount, listeners, and tags.
- **Lyrics**: Lyrics scraped from Musixmatch and Genius.
- **Spotify Audio Analysis**: Low-level audio features from Spotify's API.

## Feature Engineering

Our feature engineering efforts included:

- **Dataset Reduction**: Reducing the dataset size for efficiency while maintaining relevance.
- **Lyrical Features**: Using NLP to extract features like sentiment and word embeddings.
- **Genre and Tag Processing**: Utilizing one-hot encoding and embeddings to capture genre and tag information.

## Content-Based Recommender System

The CBRS was developed through multiple iterations:

- **Baseline Model**: Initial model using basic features.
- **Additional Features**: Enhanced model with NLP-generated features.
- **Final Model**: Comprehensive model with all features, encapsulated within a class for modularity and extensibility.

### Backend

Implemented using Python, the backend calculates similarities between songs based on features and provides recommendations.

### Frontend

A web-based frontend built with Flask and Jinja to interact with the CBRS, allowing users to input song preferences and receive recommendations.

## Results

We conducted surveys to gather user feedback and iteratively improved the CBRS based on this data. Key findings included:

- User preferences for 1980s music.
- Satisfaction with the recommendations.
- Areas for improvement in the CBRS.

## Conclusion and Future Work

We plan to integrate the OpenAI API for deeper lyrical analysis, expand multilingual support, and continuously refine the system based on user feedback.

## Installation

To set up the project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/amirhossein-rahnama/recommender-system.git
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Flask app:
   ```bash
   flask run
   ```

## Usage

1. Open your web browser and navigate to `http://127.0.0.1:5000/`.
2. Enter a song title and artist to receive recommendations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

- Amir Hossein Rahnama
- Martin Wild
- Thore Ole Dahl

## Advisors

- Prof. Dr. Tillmann Schwörer
- Prof. Dr. rer. nat. Stephan Doerfel
