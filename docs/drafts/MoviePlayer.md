A MoviePlayer manages the playback of a movie from a file or a network stream. Playback occurs in a view owned by the movie player and takes place either fullscreen or inline.

![MoviePlayer](images/movieplayer1.png)

### How to use
1. Drop a `MoviePlayer` control from the object panel to a `Window`
2. Use the `MoviePlayer Inspector` to customize its properties like `Remote File`, `Local File`, and `Scaling Mode`

![`MoviePlayer` inspector](images/movieplayer2.png)
The inspector where the `MoviePlayer` class can be configured.

### Example
1. Drop a `Button` control from the object panel to a `Window`
2. Open the `Code Editor` (cmd + 6)
3. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`
```
MoviePlayer1.contentPath = "Add your movie path here..."
```

### Most important properties
Several UI aspects can be configured in the `MoviePlayer` class but the `contentPath`, `fullscreen`, and `scalingMode` are the most commons to be configured.
- `contentPath`: The path/URL that points to the local/remote movie file.
- `fullscreen`: A Boolean that indicates whether the movie player is in full-screen mode.
- `scalingMode`: The scaling mode to use when displaying the movie.

### References
[MoviePlayer class reference](../classes/MoviePlayer.html) contains a complete list of properties and methods that can be used to customize a `MoviePlayer` object.
