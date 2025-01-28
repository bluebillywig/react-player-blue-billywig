# react-player-blue-billywig

This GitHub-hosted NPM package extends ReactPlayer, enabling you to embed Blue Billywig content (media clips, projects, playlists) in a React web application.

## Add to package.json
```
        "dependencies": {
                "react": "^18.0.0",
                "react-player": "^2.16.0",
                "react-player-blue-billywig": "^8.17.0"
        }
```

## Import and Register the Extension
```
import React from 'react';
import ReactPlayer from 'react-player';
import ReactPlayerBlueBillywig from 'react-player-blue-billywig';
ReactPlayer.addCustomPlayer(ReactPlayerBlueBillywig);
```

## Embedding
Embed Blue Billywig content using the URL provided in the JavaScript embed codes from the Online Video Platform. Simply change the .js file extension to .json and use it like this:
```
<ReactPlayer url="https://bluebillywig.bbvms.com/p/demo/c/5938172.json" playing controls />
```

## Troubleshooting
If the player doesn't load as expected, try including the following script in your HTML as a workaround:
```
<script type="text/javascript" src="https://cdn.bluebillywig.com/apps/player/latest/player.js"></script>
```
