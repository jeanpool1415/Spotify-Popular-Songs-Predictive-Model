# Spotify-Popular-Songs-Predictive-Model
Basic approach to predict popular songs in spotify based on audio and lyrics features

## Project purpose and goals
Most existing models analyze the popularity of songs primarily through audio features, offering useful insights but neglecting the significant impact of lyrical content. This gap creates a business necessity to explore the combined influence of audio and lyrical features on a song's popularity, addressing a more holistic understanding of success factors in the music industry.

This project aims to provide actionable insights by analyzing both audio and lyrical features, addressing key challenges like aligning creativity with listener preferences and supporting emerging artists. It equips stakeholders, including artists, record labels, and platforms like Spotify, with predictive tools to enhance decision-making and foster collaborations. By bridging gaps in creativity, market demands, and innovation, the project seeks to revolutionize music discovery and production through data-driven strategies.

## Dataset
The dataset used for the model contains the processed audio features (loudness, energy, dancebility,..) and the raw lyrics from each song to be process.

## Methodologies used
In this basic approach for preprocessing the lyrics have been used techniques to extract emotion, sentiments, lexical diversity and topics. For dealing with the imbalance data from the popular category, undersampling technique has been used. In the modelling, logistic regression has been used as baseline to compare with a Random Forest model.

## Key findings
- General Trends: Simpler lyrics (lower lexical diversity), loudness, and danceability are key predictors of popularity across genres, with newer songs generally being more popular except in rock.
- Genre-Specific Insights: Popularity drivers vary by genre; for example, "Hip-Hop" subgenres dominate in rap, while older tracks are favored in rock, and reggaeton elements are critical in Latin music.
- Model Performance: Random Forest models excel in capturing complex relationships, but imbalanced datasets pose challenges in achieving precision-recall balance. The model excels predicting not popular songs, but struggle with popular songs. However, capture around 72% of the popular songs.
- Feature Divergence: Subgenres and specific attributes (e.g., "Neo Soul" in R&B or "Indie Poptimism" in pop) have unique impacts, while thematic diversity has minimal importance.

## Limitations and improvements
- Temporal Trends: Year-related features dominate predictions but might fail to generalize to older or timeless tracks.
- Dataset Imbalance: The results are influenced by the dataset's composition, particularly its balance across genres and popularity classes.

- Recommendations:
    - Incorporate additional data like streaming metrics ( play counts or playlist placements) to refine predictions.
    - Experiment with neural networks or hybrid models to capture deeper relationships between features.
    - Explore more advanced NLP techniques to extract richer semantic meaning from lyrics.








