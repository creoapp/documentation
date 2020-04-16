**super**: **[UIView](UIView.md)** (on iOS)

A MoviePlayer manages the playback of a movie from a file or a network stream. Playback occurs in a view owned by the movie player and takes place either fullscreen or inline.



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidEnterFullscreen**()
Posted when the movie player has entered full-screen mode.

* **DidExitFromFullscreen**()
Posted when the movie player has exited full-screen mode.

* **DurationAvailable**()
Posted when the duration of the movie has been determined.

* **NowPlayingMovieDidChange**()
Posted when the currently playing movie has changed.

* **PlaybackDidFinish**()
Posted when the movie has finished playing.

* **PlaybackStateDidChange**()
Posted when the movie player's playback state has changed.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **contentPath**: **[String](../gravity/string.md)**
The path/URL that points to the local/remote movie file.

* **var** **movie**: **[Movie](Movie.md)**
Use this property to set the content from a Movie object from the Assets library.

* **var** **isPreparedToPlay**: **[Bool](../gravity/bool.md)**
Returns true if prepared for playback, otherwise false. \(read-only\)

* **var** **currentPlaybackTime**: **[Float](../gravity/float.md)**
The current playback time of the now playing item in seconds.

* **var** **currentPlaybackRate**: **[Float](../gravity/float.md)**
The current playback rate of the now playing item. Default is 1.0 (normal speed). Pausing will set the rate to 0.0. Setting the rate to non-zero implies playing.

* **var** **scalingMode**: **<a href="#_enum_MovieScalingMode">MovieScalingMode</a>**
The scaling mode to use when displaying the movie.

* **var** **showsPlaybackControls**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the player view controller shows playback controls.

* **var** **duration**: **[Float](../gravity/float.md)**
The duration of the movie, measured in seconds. \(read-only\)

* **var** **playableDuration**: **[Float](../gravity/float.md)**
The amount of currently playable content. \(read-only\)

* **var** **playbackState**: **<a href="#_enum_MoviePlaybackState">MoviePlaybackState</a>**
The current playback state of the movie player. \(read-only\)

* **var** **endPlaybackTime**: **[Float](../gravity/float.md)**
The end time (measured in seconds) for playback of the movie.

* **var** **shouldAutoplay**: **[Bool](../gravity/bool.md)**
A Boolean that indicates whetever a movie should begin playback automatically.

* **var** **readyForDisplay**: **[Bool](../gravity/bool.md)**
A Boolean that indicates whetever the first video frame of the movie is ready to be displayed. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **play**()
Plays items from the current queue, resuming paused playback if possible.

* **func** **pause**()
Pauses playback if playing.

* **func** **stop**()
Ends playback. Calling -play again will start from the beginnning of the queue.

* **func** **beginSeekingForward**()
.

* **func** **beginSeekingBackward**()
.

* **func** **endSeeking**()
.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **animations**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="animations ()" data-content="The animations closure, if set, contains the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.">Closure</a>**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (finished: Bool)" data-content="The completion closure, if set, is executed when the animation sequence ends. This block has no return value and takes a single Bool argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle.">Closure</a>**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_MovieScalingMode"></div>

#### MovieScalingMode
 * .AspectFill
 * .AspectFit
 * .Fill

<div id="_enum_MoviePlaybackState"></div>

#### MoviePlaybackState
 * .Paused
 * .Playing
 * .SeekingBackward
 * .SeekingForward
 * .Stopped

<div id="_enum_AnimationOption"></div>

#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone



