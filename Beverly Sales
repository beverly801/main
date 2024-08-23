// Class representing a Song
class Song {
  String title;  // Title of the song
  String artist; // Artist of the song
  double duration; // Duration of the song in minutes

  // Constructor to initialize a song with its title, artist, and duration
  Song(this.title, this.artist, this.duration);

  // Method to play the song
  void play() {
    print('Now playing: "$title" by $artist');
  }
}

// Class representing a Playlist (Stage)
class Playlist {
  String name;  // Name of the playlist (or stage)
  List<Song> songs;  // List to hold the songs in the playlist

  // Constructor to initialize a playlist with a name
  Playlist(this.name) : songs = [];

  // Method to add a song to the playlist
  void addSong(Song song) {
    songs.add(song);
  }

  // Method to remove a song from the playlist
  void removeSong(Song song) {
    songs.remove(song);
  }

  // Method to play all songs in the playlist
  void playAll() {
    print('Playing all songs in the playlist: $name');
    for (Song song in songs) {
      song.play();
    }
  }

  // Method to calculate the total duration of the playlist
  double totalDuration() {
    return songs.fold(0, (sum, song) => sum + song.duration);
  }
}

// Class representing a Music Festival
class MusicFestival {
  String name;  // Name of the festival
  List<Playlist> stages;  // List to hold the playlists (stages)

  // Constructor to initialize the festival with a name
  MusicFestival(this.name) : stages = [];

  // Method to add a playlist (stage) to the festival
  void addStage(Playlist playlist) {
    stages.add(playlist);
  }

  // Method to start the festival and play all songs on all stages
  void startFestival() {
    print('Welcome to the $name Music Festival!');
    for (Playlist stage in stages) {
      stage.playAll();
    }
  }
}

void main() {
  // Creating songs for Stage 1
  Song song1 = Song('Bohemian Rhapsody', 'Queen', 5.55);
  Song song2 = Song('Stairway to Heaven', 'Led Zeppelin', 8.02);
  Song song3 = Song('Hotel California', 'Eagles', 6.30);
  Song song4 = Song('Imagine', 'John Lennon', 3.03);
  Song song5 = Song('Like a Rolling Stone', 'Bob Dylan', 6.13);

  // Creating songs for Stage 2
  Song song6 = Song('Smells Like Teen Spirit', 'Nirvana', 5.01);
  Song song7 = Song('Billie Jean', 'Michael Jackson', 4.54);
  Song song8 = Song('Hey Jude', 'The Beatles', 7.11);
  Song song9 = Song('Sweet Child o\' Mine', 'Guns N\' Roses', 5.56);
  Song song10 = Song('Thriller', 'Michael Jackson', 5.57);

  // Creating songs for Stage 3
  Song song11 = Song('Lose Yourself', 'Eminem', 5.26);
  Song song12 = Song('Shape of You', 'Ed Sheeran', 3.53);
  Song song13 = Song('Uptown Funk', 'Mark Ronson ft. Bruno Mars', 4.30);
  Song song14 = Song('Rolling in the Deep', 'Adele', 3.48);
  Song song15 = Song('Blinding Lights', 'The Weeknd', 3.22);

  // Creating playlists (stages) and adding songs
  Playlist stage1 = Playlist('Rock Legends');
  stage1.addSong(song1);
  stage1.addSong(song2);
  stage1.addSong(song3);
  stage1.addSong(song4);
  stage1.addSong(song5);

  Playlist stage2 = Playlist('Pop Icons');
  stage2.addSong(song6);
  stage2.addSong(song7);
  stage2.addSong(song8);
  stage2.addSong(song9);
  stage2.addSong(song10);

  Playlist stage3 = Playlist('Modern Hits');
  stage3.addSong(song11);
  stage3.addSong(song12);
  stage3.addSong(song13);
  stage3.addSong(song14);
  stage3.addSong(song15);

  // Creating a music festival
  MusicFestival festival = MusicFestival('Global Music Fest');
  festival.addStage(stage1);
  festival.addStage(stage2);
  festival.addStage(stage3);

  // Starting the festival
  festival.startFestival();
}
