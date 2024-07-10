# Spotify Network Analysis
This project aims to enhance transparency in music recommendation algorithms by exploring playlist structures through graph analysis and visualizations.

## Dataset 
The dataset is a subset of the data derived from Spotify’s The Million Playlist Dataset. The dataset contains information related to playlists, songs and the interactions between them.  From this extensive dataset, a subset of playlists was randomly selected to construct song-song co-occurrence networks. In these networks, nodes represent individual songs, and edges indicate co-occurrence relationships between songs within playlists. Each edge is weighted based on the frequency of co-occurrence between two songs in playlists. Additionally, the network includes edge properties such as the list of playlist IDs where the two songs have co-occurred.

The README.txt file contains the description of the dataset files

## Project Structure

- `data/`: Directory containing the dataset. The README.txt file contains the description of the data files 
- `notebooks/`: Jupyter notebooks with tasks performed.
- `Report.pdf`: Contains detailed report of the analysis performed.

### Notebooks
- `NetworkAnalysisSmaller.ipynb`: Contains the analysis of the structure of a small song-song co-occurrence graph including general analysis, visualization, and computation of basic metrics such as node degree and centrality measures.
-  `NetworkAnalysisBigger.ipynb`: Contains the structure of a larger song-song co-occurrence graph including general analysis, computation of metrics similar to Task 1, and a comparative analysis between the small and large graphs.
-  `EdgeWeightsBasedRecommender.ipynb`: Contains a graph recommendation algorithm based on song co-occurrence. Builds a function that takes an input song name and performs a graph-walk based on edge weights to recommend songs.
-  `SpotifyAPIBasedRecommender.ipynb`: Contains vectorized node information with attributes from the Spotify API and a recommendation algorithm based on cosine similarity.


