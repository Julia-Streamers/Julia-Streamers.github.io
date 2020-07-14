# Documentation

## New streamer

If you want to add yourself to the list of streams all you need to do is add another `\streamer` command to the index.md.

The `\streamer` command takes four arguments:
1. Your Twitch username
2. How you want to call yourself (can be the same as 1.)
3. Link to your profile picture (which needs to be in `_assets/streamers`)
4. A description which where you might want to describe what you are working on at the moment

As an example command:
```
\streamer{opensourcesblog}{OpenSourcES}{opensourcesblog.png}{I mostly stream about project Euler.}
```

This needs to be added between 
`~~~<div class="streamers">~~~` and `~~~</div>` in the `index.md`