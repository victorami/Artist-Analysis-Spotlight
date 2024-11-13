# Artist Analysis Spotlight

This project aims to conduct an in-depth analysis of Tyler, the Creator's discography by exploring various audio and track-level features obtained from the Spotify API. The goal is to uncover meaningful patterns and insights about Tyler, the Creator's music, including trends in audio characteristics across albums, popularity dynamics, and collaborative aspects. The analysis serves both to highlight Tyler’s creative evolution and to showcase methods of musical data analysis.

The data was obtained directly from the Spotify API, which provides a variety of track-level and artist-level features, including in-depth audio analysis for each track. For this project, data on Tyler, the Creator's tracks, albums, and audio features were extracted and then processed for analysis.

The dataset comprises a rich set of features for each track in Tyler, the Creator's discography, covering a range of audio, temporal, and metadata characteristics.

### Feature Columns
- **Basic Information**: Track, album, and artist names, album art, release date, and genres.
- **Popularity & Explicit Content**: Track popularity scores on Spotify, and flags for explicit content.
- **Audio Features**: Key musical attributes such as danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence, and tempo.
- **Additional Metadata**: Duration (in ms and seconds), release details (year, month, day of the week), and the presence of featured artists.

This dataset provides a comprehensive basis for analyzing musical structure, emotional tone, and artistic collaborations.

| Column               | Description |
|----------------------|-------------|
| artist_name          | The name of the main artist for the track, in this case, always "Tyler, the Creator." |
| artist_image_url     | URL link to an image of the artist, usually provided by Spotify. |
| track_name           | The title of the track as listed on Spotify. |
| track_id             | Spotify's unique identifier for the track. |
| album_name           | The name of the album on which the track appears. |
| album_id             | Spotify's unique identifier for the album. |
| album_artwork_url    | URL link to the album cover art image. |
| genres               | List of musical genres associated with the artist. |
| release_date         | The date the track or album was released, usually in YYYY-MM-DD format. |
| popularity           | A score between 0 and 100 representing the track's popularity. |
| explicit             | Boolean indicator of explicit content (True = explicit, False = not explicit). |
| danceability         | A measure from 0.0 to 1.0 for danceability based on tempo, rhythm, and beat strength. |
| energy               | A measure from 0.0 to 1.0 for track intensity; higher values mean higher energy. |
| key                  | The key of the track as an integer (0 = C, 1 = C♯/D♭, ..., 11 = B). |
| loudness             | The average loudness of the track in decibels (dB). |
| mode                 | Indicates the modality of the track (1 = major, 0 = minor). |
| speechiness          | A measure from 0.0 to 1.0 estimating the presence of spoken words. |
| acousticness         | A measure from 0.0 to 1.0 indicating the likelihood the track is acoustic. |
| instrumentalness     | A measure from 0.0 to 1.0 representing the probability of no vocals. |
| liveness             | A measure from 0.0 to 1.0 indicating likelihood the track was performed live. |
| valence              | A measure from 0.0 to 1.0 describing musical positiveness; higher values are happier. |
| tempo                | The track's tempo in beats per minute (BPM). |
| time_signature       | Estimated time signature (e.g., 4 = 4/4 time, 3 = 3/4 time). |
| featured_artists     | List of other artists featured on the track, if any. |
| type                 | The type of Spotify object; in this dataset, always "track." |
| duration_ms          | Duration of the track in milliseconds. |
| year                 | The year the track was released, extracted from the release date. |
| month                | The month the track was released, extracted from the release date. |
| day_of_the_week      | The day of the week the track was released, extracted from the release date. |

### Files

- **Artist Discography Dataset**: A CSV file containing detailed Spotify data on the artist's discography, retrieved through Spotify's API.
- **Data Collection Notebook**: A Jupyter Notebook used to request and compile data from Spotify's API.
- **Analysis Notebook**: A Jupyter Notebook dedicated to the analysis and visualization of the Spotify data for insights into the artist's discography.

### Requirements

- **Jupyter Notebook**: [https://jupyter.org/](https://jupyter.org/)

### Libraries

- **Pandas**: [https://pandas.pydata.org/](https://pandas.pydata.org/) 
- **NumPy**: [https://numpy.org/](https://numpy.org/)
- **Matplotlib (Pyplot)**: [https://matplotlib.org/stable/api/pyplot_api.html](https://matplotlib.org/stable/api/pyplot_api.html) 
- **Seaborn**: [https://seaborn.pydata.org/](https://seaborn.pydata.org/) 
- **Warnings**: [https://docs.python.org/3/library/warnings.html](https://docs.python.org/3/library/warnings.html)
- **IPython**: [https://ipython.readthedocs.io/](https://ipython.readthedocs.io/)
- **Requests**: [https://requests.readthedocs.io/](https://requests.readthedocs.io/)
- **Ast**: [https://docs.python.org/3/library/ast.html](https://docs.python.org/3/library/ast.html)
- **Base64**: [https://docs.python.org/3/library/base64.html](https://docs.python.org/3/library/base64.html)
- **Json**: [https://docs.python.org/3/library/json.html](https://docs.python.org/3/library/json.html)
- **Spotipy**: [https://spotipy.readthedocs.io/](https://spotipy.readthedocs.io/)
