# An Analysis of Spotify's _Top Tracks of 2022 - Nigeria_  Playlist
## By Neto Anyama.

## Table of Contents
<ul>
<li><a href="#description">Description</a></li>
<li><a href="#conclusions">Conclusions</a></li>
<li><a href="#visualization">Visualization</a></li>
</ul>

<a id='description'></a>
### Description
Hi! I'm Neto Anyama. In this project, I performed exploratory data analysis on the Top Tracks of 2022 Nigeria playlist, curated by Spotify, on Spotify. It contained the 50 songs that were most listened to in Nigeria, where I'm from. Data wrangling was done using Python (specifically the Spotipy library), while visualization was done using PowerBI.

#### Dataset Features.
1. Name: The name of the track.                  
2. Album: The album on which the track appears.           
3. Artist: The name of the performing artist.               
4. Release Date: The date the song/album was released.    
5. Duration: The duration of the track in minutes, originally in milliseconds.            
6. Popularity: The score assigned to each track based on the number of streams, likes etc.             
7. Danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
8. Energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.          
9. Key: The key the track is in. If no key was detected, the value is -1. Key ranges from -1 to 11.
10. Loudness: The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.
11. Mode: Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
12. Speechiness: Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. 
13. Acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
14. Instrumentalness: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.
15. Liveness: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.            
16. Valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
17. Tempo: The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.                
18. ID: The Spotify ID for the track.
19. Time Signature: An estimated time signature. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure). The time signature ranges from 3 to 7 indicating time signatures of "3/4", to "7/4".

> Descriptions of most of the columns were obtained from [here](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features).
  
#### Questions.
1. What are the most popular songs overall?
2. In what month were most of these songs released?
3. How did certain audio features influence popularity?

Listen to the playlist [here](https://open.spotify.com/playlist/37i9dQZF1DX1W96TRrqJX4). 

<a id='conclusions'></a>
### Conclusions.

After performing exploratory data analysis on the dataset, the following inferences were made:

- 90% of the songs in the playlist had time signatures of 4.

- 8 of the songs that made the list were released in September 2022, the highest of all the release months.

- Shorter songs were more popular than longer songs.

- Songs with a higher tempo are more danceable that songs with lower tempo.

- Nigerians preferred songs with particularly low acousticness (0 - 0.10) to songs on the other end of the scale.

- Songs with a speechiness of 0.15 (low speechiness) were the most preferred. This means that songs made up primarily of beats and instrumentals were greatly preferred.

- Nigerians enjoyed songs with a midrange energy (0.65), i.e., moderately fast, loud and intense.

- Nigerians greatly enjoyed particularly danceable rhythms, with the most love coming at the 0.8 danceability point.

- Songs with a mid-upper range (0.6-0.75) valence were most preferred. Therefore, Nigerians enjoyed songs with some level of positivity to them.

<a id='visualization'></a>
### Visualization
The interactive report for this project was done using PowerBI can be found [here](https://app.powerbi.com/view?r=eyJrIjoiNWJhOGY5OTYtNGYzYy00ODBmLTk3NWItMDg0NGYxMTQ3ZmY1IiwidCI6ImEzMjNmYmMzLTM3NzUtNDNhMi05MWYxLTA4YWY1ZTA1MTVhZSJ9).
