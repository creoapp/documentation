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

* **MediaTypesAvailable**()
Posted when the available media types in the movie has been determined.

* **LoadStateDidChange**()
Posted when the movie player's network buffering state has changed.

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

* **var** **contentPath**: **[String](../gravity/types.md)**
The path/URL that points to the local/remote movie file.

* **var** **movieSourceType**: **MovieSourceType**
The types of media available in the movie.

* **var** **movieMediaTypes**: **MovieMediaTypeMask**
The playback type of the movie. \(read-only\)

* **var** **isPreparedToPlay**: **[Bool](../gravity/types.md)**
Returns true if prepared for playback, otherwise false. \(read-only\)

* **var** **currentPlaybackTime**: **[Float](../gravity/types.md)**
The current playback time of the now playing item in seconds.

* **var** **currentPlaybackRate**: **[Float](../gravity/types.md)**
The current playback rate of the now playing item. Default is 1.0 (normal speed). Pausing will set the rate to 0.0. Setting the rate to non-zero implies playing.

* **var** **allowsAirPlay**: **[Bool](../gravity/types.md)**
Specifies whetever the movie player allows AirPlay movie playback.

* **var** **airPlayVideoActive**: **[Bool](../gravity/types.md)**
Indicates whetever the movie player is currently playing video via AirPlay. \(read-only\)

* **var** **naturalSize**: **[Size](Size.md)**
The width and height of the movie frame. \(read-only\)

* **var** **fullscreen**: **[Bool](../gravity/types.md)**
A Boolean that indicates whetever the movie player is in full-screen mode.

* **var** **scalingMode**: **MovieScalingMode**
The scaling mode to use when displaying the movie.

* **var** **controlStyle**: **MovieControlStyle**
The style of the playback controls.

* **var** **duration**: **[Float](../gravity/types.md)**
The duration of the movie, measured in seconds. \(read-only\)

* **var** **playableDuration**: **[Float](../gravity/types.md)**
The amount of currently playable content. \(read-only\)

* **var** **loadState**: **MovieLoadState**
The network load state of the movie player. \(read-only\)

* **var** **playbackState**: **MoviePlaybackState**
The current playback state of the movie player. \(read-only\)

* **var** **initialPlaybackTime**: **[Float](../gravity/types.md)**
The time, specified in seconds within the video timeline, when playback should start.

* **var** **endPlaybackTime**: **[Float](../gravity/types.md)**
The end time (measured in seconds) for playback of the movie.

* **var** **shouldAutoplay**: **[Bool](../gravity/types.md)**
A Boolean that indicates whetever a movie should begin playback automatically.

* **var** **readyForDisplay**: **[Bool](../gravity/types.md)**
A Boolean that indicates whetever the first video frame of the movie is ready to be displayed. \(read-only\)

* **var** **repeatMode**: **MovieRepeatMode**
Obtains the most recent time-based metadata provided by the streamed movie.



### Methods

* **func** **setFullscreenAnimated**(**fullscreen**: **[Bool](../gravity/types.md)**, **animated**: **[Bool](../gravity/types.md)**)
Causes the movie player to enter or exit full-screen mode.

* **func** **play**()
Plays items from the current queue, resuming paused playback if possible.

* **func** **pause**()
Pauses playback if playing.

* **func** **stop**()
Ends playback. Calling -play again will start from the beginnning of the queue.

* **func** **prepareToPlay**()
Prepares the current queue for playback, interrupting any active (non-mixible) audio sessions. Automatically invoked when play is called if the player is not already prepared.

* **func** **beginSeekingForward**()
.

* **func** **beginSeekingBackward**()
.

* **func** **endSeeking**()
.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### MovieSourceType
 * .File
 * .Streaming
 * .Unknown

#### MovieMediaTypeMask
 * .Audio
 * .None
 * .Video

#### MovieScalingMode
 * .AspectFill
 * .AspectFit
 * .Fill
 * .None

#### MovieControlStyle
 * .Default
 * .Embedded
 * .Fullscreen
 * .None

#### MovieLoadState
 * .Playable
 * .PlaythroughOK
 * .Stalled
 * .Unknown

#### MoviePlaybackState
 * .Interrupted
 * .Paused
 * .Playing
 * .SeekingBackward
 * .SeekingForward
 * .Stopped

#### MovieRepeatMode
 * .None
 * .One

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



