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

* **var** **contentPath**: **[String](../gravity/string.md)**
The path/URL that points to the local/remote movie file.

* **var** **movie**: **[Movie](Movie.md)**
Use this property to set the content from a Movie object from the Assets library.

* **var** **movieSourceType**: **<a href="#_enum_MovieSourceType">MovieSourceType</a>**
The types of media available in the movie.

* **var** **movieMediaTypes**: **<a href="#_enum_MovieMediaTypeMask">MovieMediaTypeMask</a>**
The playback type of the movie. \(read-only\)

* **var** **isPreparedToPlay**: **[Bool](../gravity/bool.md)**
Returns true if prepared for playback, otherwise false. \(read-only\)

* **var** **currentPlaybackTime**: **[Float](../gravity/float.md)**
The current playback time of the now playing item in seconds.

* **var** **currentPlaybackRate**: **[Float](../gravity/float.md)**
The current playback rate of the now playing item. Default is 1.0 (normal speed). Pausing will set the rate to 0.0. Setting the rate to non-zero implies playing.

* **var** **allowsAirPlay**: **[Bool](../gravity/bool.md)**
Specifies whetever the movie player allows AirPlay movie playback.

* **var** **airPlayVideoActive**: **[Bool](../gravity/bool.md)**
Indicates whetever the movie player is currently playing video via AirPlay. \(read-only\)

* **var** **naturalSize**: **[Size](Size.md)**
The width and height of the movie frame. \(read-only\)

* **var** **fullscreen**: **[Bool](../gravity/bool.md)**
A Boolean that indicates whetever the movie player is in full-screen mode.

* **var** **scalingMode**: **<a href="#_enum_MovieScalingMode">MovieScalingMode</a>**
The scaling mode to use when displaying the movie.

* **var** **controlStyle**: **<a href="#_enum_MovieControlStyle">MovieControlStyle</a>**
The style of the playback controls.

* **var** **duration**: **[Float](../gravity/float.md)**
The duration of the movie, measured in seconds. \(read-only\)

* **var** **playableDuration**: **[Float](../gravity/float.md)**
The amount of currently playable content. \(read-only\)

* **var** **loadState**: **<a href="#_enum_MovieLoadState">MovieLoadState</a>**
The network load state of the movie player. \(read-only\)

* **var** **playbackState**: **<a href="#_enum_MoviePlaybackState">MoviePlaybackState</a>**
The current playback state of the movie player. \(read-only\)

* **var** **initialPlaybackTime**: **[Float](../gravity/float.md)**
The time, specified in seconds within the video timeline, when playback should start.

* **var** **endPlaybackTime**: **[Float](../gravity/float.md)**
The end time (measured in seconds) for playback of the movie.

* **var** **shouldAutoplay**: **[Bool](../gravity/bool.md)**
A Boolean that indicates whetever a movie should begin playback automatically.

* **var** **readyForDisplay**: **[Bool](../gravity/bool.md)**
A Boolean that indicates whetever the first video frame of the movie is ready to be displayed. \(read-only\)

* **var** **repeatMode**: **<a href="#_enum_MovieRepeatMode">MovieRepeatMode</a>**
Obtains the most recent time-based metadata provided by the streamed movie.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **setFullscreenAnimated**(**fullscreen**: **[Bool](../gravity/bool.md)**, **animated**: **[Bool](../gravity/bool.md)**)
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

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_MovieSourceType"></div>

#### MovieSourceType
 * .File
 * .Streaming
 * .Unknown

<div id="_enum_MovieMediaTypeMask"></div>

#### MovieMediaTypeMask
 * .Audio
 * .None
 * .Video

<div id="_enum_MovieScalingMode"></div>

#### MovieScalingMode
 * .AspectFill
 * .AspectFit
 * .Fill
 * .None

<div id="_enum_MovieControlStyle"></div>

#### MovieControlStyle
 * .Default
 * .Embedded
 * .Fullscreen
 * .None

<div id="_enum_MovieLoadState"></div>

#### MovieLoadState
 * .Playable
 * .PlaythroughOK
 * .Stalled
 * .Unknown

<div id="_enum_MoviePlaybackState"></div>

#### MoviePlaybackState
 * .Interrupted
 * .Paused
 * .Playing
 * .SeekingBackward
 * .SeekingForward
 * .Stopped

<div id="_enum_MovieRepeatMode"></div>

#### MovieRepeatMode
 * .None
 * .One

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



