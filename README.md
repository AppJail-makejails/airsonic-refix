# Airsonic (refix) UI

Modern responsive web frontend for [airsonic-advanced](https://github.com/airsonic-advanced/airsonic-advanced), [navidrome](https://github.com/navidrome/navidrome), [gonic](https://github.com/sentriz/gonic) and other [subsonic](https://github.com/topics/subsonic) compatible music servers.

github.com/tamland/airsonic-refix

<img src="https://i.imgur.com/BX1C3c9.png" width="80%" height="auto">

## Features

* Responsive UI for desktop and mobile
* Browse library for albums, artist, generes
* Playback with persistent queue, repeat & shuffle
* MediaSession integration
* View, create, and edit playlists with drag and drop
* Built-in 'random' playlist
* Search
* Favourites
* Internet radio
* Podcasts

## How to use this Makejail

```sh
appjail makejail \
    -j airsonic-refix \
    -f gh+AppJail-makejails/airsonic-refix \
    -o virtualnet=":<random> default" \
    -o nat \
    -o expose=80
```

### Arguments

* `airsonic_refix_tag`: See [#tags](#tags).
* `airsonic_refix_server_url` (optional): The backend server URL. When set the server input on the login page will not be displayed.

### Tags

| Tag    | Arch     | Version        | Type   |
| ------ | -------- | -------------- | ------ |
| `13.3` | `amd64`  | `13.3-RELEASE` | `thin` |
| `14.0` | `amd64`  | `14.0-RELEASE` | `thin` |
