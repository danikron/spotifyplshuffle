# spotifyplshuffle
Imports the tracks of a seed playlist, shuffles them and exports them to a target playlist. The seed and target playlist can be the same.
This was based on some other script but I forget which, sorry.

## Usage
Reads a file `auth` in the script directory to find the client ID and client secret, which can be obtained by adding an approved application on the Spotify account page. The file should be formatted:
```
id:<client id>
secret:<client secret>
```
Reads a file `playlists` in the script directory to find the seed and target playlists. The file should be formatted:
```
seed:<user>/playlists/<playlist id>
target:<user>/playlists/</playlist id>
```

The script will open an authentication page in the default webbrowser in order to fetch an access token. This operation requires nc, provided by GNU Netcat or openbsd-netcat.

# spotifyplbackup
Creates a list of tracks from a seed playlist in the working directory.
