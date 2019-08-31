**super**: **[Object](../gravity/object.md)**

Provides playback of audio data from a file, an url or memory. A Sound object is usually a representation of an audio asset.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Completed**()
Handle this event if you want to perform some operations when audio resource finished playing.

* **OnError**()
Handle this event if you want to take any action in case of error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **isPlaying**: **[Bool](../gravity/bool.md)**
A Bool value that indicates whether the audio player is playing. \(read-only\)

* **var** **channels**: **[Int](../gravity/int.md)**
The number of audio channels in the sound associated with the audio player. \(read-only\)

* **var** **duration**: **[Float](../gravity/float.md)**
Returns the total duration, in seconds, of the sound associated with the audio player. \(read-only\)

* **var** **pan**: **[Float](../gravity/float.md)**
The audio player’s stereo pan position. By setting this property you can position a sound in the stereo field. A value of –1.0 is full left, 0.0 is center, and 1.0 is full right.

* **var** **volume**: **[Float](../gravity/float.md)**
The playback volume for the audio player, ranging from 0.0 through 1.0 on a linear scale.

* **var** **time**: **[Float](../gravity/float.md)**
The playback point, in seconds, within the timeline of the sound associated with the audio player. If the sound is playing, currentTime is the offset of the current playback position, measured in seconds from the start of the sound. If the sound is not playing, currentTime is the offset of where playing starts upon calling the play method, measured in seconds from the start of the sound.

By setting this property you can seek to a specific point in a sound file or implement audio fast-forward and rewind functions.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **open**(**srcfile**: **[Object](../gravity/object.md)**)<strong>: [Object](../gravity/object.md)</strong> 
Initializes and returns the Sound object with the content of the source file. The source file can be an URL or a <a href="File.html">File</a> object.



### Constructors

* **func** **Sound**(**nameOrURL**: **[Object](../gravity/object.md)**)
Creates and initializes a new sound resource.

* **func** **Sound**(**nameOrURL**: **[Object](../gravity/object.md)**, **globalInstance**: **[Bool](../gravity/bool.md)**)
Creates and initializes a new sound resource.



### Methods

* **func** **play**()<strong>: [Bool](../gravity/bool.md)</strong> 
Plays a sound asynchronously.

* **func** **pause**()
Pause a sound.

* **func** **resume**()
Resume a sound.

* **func** **stop**()
Stop a sound.





