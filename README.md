## 🗒️ Authors


Name | Sciper |
--- | --- | 
Bacuet Aymeric | 297168 |
Tetard Kenji | 301569 |


| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#objects) | :movie_camera: | `:movie_camera:` | :film_strip: | `:film_strip:` | [top](#table-of-contents) |
| [top](#objects) | :film_projector: | `:film_projector:` | :clapper: | `:clapper:` | [top](#table-of-contents) |
| [top](#objects) | :tv: | `:tv:` | :camera: | `:camera:` | [top](#table-of-contents) |
| [top](#objects) | :camera_flash: | `:camera_flash:` | :video_camera: | `:video_camera:` | [top](#table-of-contents) |
| [top](#objects) | :vhs: | `:vhs:` | :mag: | `:mag:` | [top](#table-of-contents) |
| [top](#objects) | :mag_right: | `:mag_right:` | :candle: | `:candle:` | [top](#table-of-contents) |
| [top](#objects) | :bulb: | `:bulb:` | :flashlight: | `:flashlight:` | [top](#table-of-contents) |
| [top](#objects) | :izakaya_lantern: | `:izakaya_lantern:` <br /> `:lantern:` | :diya_lamp: | `:diya_lamp:` | [top](#table-of-contents) |


The goal of this data visualization project is to create an interactive graph that showcases the relationships between actors and directors based on the movies they worked on together. The graph allows users to explore the connections between individuals and gain insights into the movies they collaborated on.

The interactive graph provides an intuitive and engaging way for users to explore the relationships and collaborations between actors and directors. By clicking on the edges, users can see the posters and descriptions of the movies and gain a deeper understanding of the collaborations.

The visualization includes multiple interactive buttons, such as a date cursor that enables users to filter the graph based on the movies made in a specific year or earlier. Similarly, the genre button allows users to see the connections between actors and directors for a particular genre, such as comedy.

This project uses data visualization techniques to present complex information in a clear and concise manner, allowing users to explore and analyze the data in an interactive and engaging way.

# Problematic

The need to understand the relationships and collaborations between actors and directors in the film industry is the problem that this project seeks to address. There is a wealth of information available about movies and their creators, but effectively analyzing and comprehending this information can be difficult. This project explores and visualizes the relationships and collaborations between actors and directors in an interactive and intuitive manner.

The primary goal of the project is to assist users in understanding the relationships and collaborations between actors and directors, as well as the films they worked on together. The interactive graph allows users to explore the data in a dynamic and engaging manner, with the option to filter by date and genre, making it easier to analyze and comprehend the information presented.

This project can facilitate new discoveries and insights in the field of film studies by providing a clear and concise representation of the data.

# Dataset
[Actor and Movie Dataset](https://github.com/KenjiTet/MA2-Kenji-Aymeric-Data-Viz/tree/main/Dataset/actorfilms.csv)

This dataset contains information about movies and the actors who starred in them. The columns of the dataset are:

  - Actor: the name of the actor who starred in the movie.
  - ActorID: a unique identifier for the actor.
  - Film: the title of the movie.
  - Year: the year the movie was released.
  - Votes: the number of votes the movie received on the website where the data was collected.
  - Rating: the average rating of the movie on the website where the data was collected.
  - FilmID: a unique identifier for the movie.
 
The dataset contains multiple rows for each actor, each row corresponding to a different movie that the actor starred in. The dataset includes movies released over     a span of several decades. The number of votes and the rating of the movies are also included, which can be used to analyze the popularity and quality of the movies. The dataset can be used to explore the careers of different actors, as well as to analyze trends in the movie industry over time.

[Poster Dataset](https://github.com/KenjiTet/MA2-Kenji-Aymeric-Data-Viz/tree/main/Dataset/duplicate_free_41K.csv)

This dataset contains information about movies and their posters. The columns of the dataset are:

  - Id: a unique identifier for the movie.
  - Poster: the URL of the poster image for the movie.
  - Title: the title of the movie.
  - Year: the year the movie was released.
  - Rating: the average rating of the movie on the website where the data was collected.
  - Genre: the genre(s) of the movie.
  - Action, adventure, animation, comedy, crime, drama, fantasy, horror, mystery, romance, sci-fi, short, thriller: binary flags indicating whether the movie belongs       to the corresponding genre(s).

The dataset includes thousands of movie posters released from 1932 to 2020. The genre(s) of each movie are also included, as well as binary flags indicating whether the movie belongs to specific genres, such as action, comedy, drama, etc. The dataset can be used to analyze trends in movie genres and to identify the most popular movies based on ratings. The poster URLs can also be used to download and analyze the images themselves.

# Data Preprocessing

Based on the information provided, it's difficult to fully assess the quality of the data in the poster movie dataset. However, there are a few things that can be noted:

  - The poster column contains URLs of images, but it was unclear if all the URLs are valid and still available. It's possible that some of the images have been    
    removed or that the URLs are incorrect.
  - The genre column contains multiple genres separated by commas. It could be difficult to work with this column in its current format, especially if we want to 
    analyze the data by genre.

Given the task of linking actors to movies, it's clear that some preprocessing and data cleaning will be necessary. The current dataset shows which actors were in each movie, but the task requires knowing which movies each actor appeared in. As mentioned, one way to accomplish this would be to create a dictionary with the movies as keys and lists of actors as values, and then convert that to a dataframe.

Once the actor/movie dataframe is created, it will be necessary to merge it with the poster movie dataset to obtain the necessary information for visualization. This will likely require additional data cleaning and processing to ensure that the data is consistent and that the merge can be performed accurately.

Overall, it's likely that several preprocessing and data cleaning steps will be necessary to obtain a useful dataset for visualization. However, with careful attention to detail and a systematic approach, it should be possible to achieve the desired outcome.

# Target Audience

The target audience for this visualization could be movie enthusiasts, students, researchers, or anyone interested in exploring the relationships between actors and directors in the film industry. It could also be used by filmmakers and producers to identify potential collaborators based on previous collaborations, allowing for more efficient and effective filmmaking.
