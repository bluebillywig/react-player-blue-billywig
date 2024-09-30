# react-player-blue-billywig

This GitHub-hosted NPM package provides an extension to ReactPlayer, enabling you to embed your Blue Billywig content (media clips, projects, playlists) in a React web app. 
Here’s how.

## Adding to your package.json
```
        "dependencies": {
                "react": "^18.0.0",
                "react-player": "^2.16.0",
                "react-player-blue-billywig": "https://github.com/bluebillywig/react-player-blue-billywig"
        }
```

## Importing and registering the extension
```
import React from 'react';
import ReactPlayer from 'react-player';
import ReactPlayerBlueBillywig from 'react-player-blue-billywig';
ReactPlayer.addCustomPlayer(ReactPlayerBlueBillywig);
```

## Embedding
The javascript embed codes from our platform have a ‘src’ property that ends in “.js”. Simply turn that into “.json” and use it like so:
```
<ReactPlayer url="https://bluebillywig.bbvms.com/p/demo/c/5938172.json" playing controls />
```

## Troubleshooting
If things don’t work out as expected, try first including 
```
<script type="text/javascript" src="https://cdn.bluebillywig.com/apps/player/latest/player.js"></script>
```
as a work-around.
