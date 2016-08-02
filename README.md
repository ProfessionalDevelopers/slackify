# slackify
Automatically add music from slack channels to a spotify playlist.

To set up:

- Clone this repo
- Create a new integration in Slack, note the token
- Create a Spotify app at developer.spotify.com with a callback location you'll be using, note the ID Secret and Redirect URI
- Create a Spotify playlist, note your username and the id of the playlist if you copy the URI
- Create a file called "env_variables" in the root of the project with the following format:

```SLACK_TOKEN=XXXXXXX
SPOTIFY_ID=XXXXXXX
SPOTIFY_SECRET=XXXXXXX
SPOTIFY_REDIRECT_URI=http://where-is-this-running:8888/callback
SPOTIFY_USERNAME=theusername
SPOTIFY_PLAYLIST_ID=XXXXXXX
```
run ```node slackify.js```

