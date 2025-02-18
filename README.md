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
Embed Blue Billywig content using the JSON embed code provided by the Online Video Platform's Preview page.
```
<ReactPlayer url="https://bluebillywig.bbvms.com/p/demo/c/5938172.json" playing controls />
```

## Troubleshooting
If the player doesn't load as expected, try including the following script in your HTML as a workaround:
```
<script type="text/javascript" src="https://cdn.bluebillywig.com/apps/player/latest/player.js"></script>
```

If you're using **React Router (v7)**, you may need to add a type declaration, for instance:
```
[missingtypes.d.ts]
declare module 'react-player-blue-billywig'
```
Further, it may help to check existence of ReactPlayer.addCustomPlayer before calling it;
```
if (ReactPlayer.addCustomPlayer) ReactPlayer.addCustomPlayer(ReactPlayerBlueBillywig);
```

If you're using **Next.js (App Router)**, you may need to add 
```
'use client'
```
to the top of the file that contains your &lt;ReactPlayer&gt; tag.
