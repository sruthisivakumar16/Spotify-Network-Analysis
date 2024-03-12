X = smaller/bigger

### 1. interactions_X.csv

- Description: represents the interactions between songs and playlists. Indicates which songs are present in each playlist.
  
- Columns:
  - playlist_id: identifier for the playlist.
  - song_id: identifier for the song.

### 2. playlist_data_X.csv

- Description: contains information about playlists, including title and collaboration status.
  
- Columns:
  - playlist_id: identifier for the playlist.
  - playlist_name: name of the playlist.
  - playlist_collab: boolean indicating whether the playlist is a collaborative playlist 

### 3. song_data_X.csv

- Description: provides basic information about songs, such as artist or album name and Spotify URIs.
  
- Columns:
  - song_id: identifier for the song.
  - song_name: name of the song
  - artist_name: name of the artist.
  - artist_uri: Spotify URI for the artist
  - album_name: name of the album.
  - album_uri: Spotify URI for the album

### 4. X_graph.pickle

- Description: contains an undirected NetworkX graph representing a co-occurrence network of songs.
  
- Graph Properties:
  - Nodes: songs
  - Edges: co-occurrence relationships between songs in playlists
  - Edge Properties:
    - weight: the number of times two songs have appeared together in playlists.
    - common_playlists: list of playlist IDs where the two songs have co-occurred

## A note

- For Spotify-related information, consider using the Spotify API with the provided Spotify URIs.