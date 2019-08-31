**super**: **[Object](../gravity/object.md)**

A class that provides audio recording capability in your application.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidFinishRecording**(**succesfully**: **[Bool](../gravity/bool.md)**)
This event is called when a recording is stopped or has finished due to reaching its time limit.

* **OnError**(**error**: **[String](../gravity/string.md)**)
This event is called when an audio recorder encounters an error during recording.

* **DeniedAuthorization**()
This event is called when user denied your app permission to record.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **isRecording**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the audio recorder is recording. \(read-only\)

* **var** **deviceCurrentTime**: **[Float](../gravity/float.md)**
The time, in seconds, of the host device where the audio recorder is located. \(read-only\)

* **var** **currentTime**: **[Float](../gravity/float.md)**
The time, in seconds, since the beginning of the recording. \(read-only\)

* **var** **seconds**: **[Float](../gravity/float.md)**
Total duration, in seconds, of the recorded audio file. \(read-only\)

* **var** **data**: **[Data](Data.md)**
A Data value serialization representing the file recorder (recording must be stopped). \(read-only\)

* **var** **filePath**: **[String](../gravity/string.md)**
Full path to the recorded file (if any). \(read-only\)

* **var** **inputChannels**: **[Int](../gravity/int.md)**
The number of audio input channels for the current route. \(read-only\)

* **var** **maximumInputChannels**: **[Int](../gravity/int.md)**
The maximum number of input channels available for the current audio route. \(read-only\)

* **var** **preferredInputChannels**: **[Int](../gravity/int.md)**
The preferred number of input channels for the current route. \(read-only\)

* **var** **outputChannels**: **[Int](../gravity/int.md)**
The number of audio output channels. \(read-only\)

* **var** **maximumOutputChannels**: **[Int](../gravity/int.md)**
The maximum number of output channels available for the current audio route. \(read-only\)

* **var** **preferredOutputChannels**: **[Int](../gravity/int.md)**
The preferred number of output channels for the current route. \(read-only\)

* **var** **inputGain**: **[Float](../gravity/float.md)**
The gain applied to inputs associated with the session. \(read-only\)

* **var** **outputVolume**: **[Float](../gravity/float.md)**
The system wide output volume set by the user. \(read-only\)

* **var** **inputLatency**: **[Float](../gravity/float.md)**
The latency for audio input, measured in seconds. \(read-only\)

* **var** **outputLatency**: **[Float](../gravity/float.md)**
The latency for audio output, measured in seconds. \(read-only\)

* **var** **currentSampleRate**: **[Float](../gravity/float.md)**
The current audio sample rate, in hertz. \(read-only\)

* **var** **preferredSampleRate**: **[Float](../gravity/float.md)**
The preferred sample rate, in hertz. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **start**(**time**: **[Float](../gravity/float.md) = 0**, **duration**: **[Float](../gravity/float.md) = 0**)
Starts or resumes recording.

* **func** **stop**()
Stops recording and closes the audio file.

* **func** **pause**()
Pauses a recording.

* **func** **reset**()
Reset recording and cleanup temp files.

* **func** **copyToFile**(**filePath**: **[String](../gravity/string.md)**)
Copy temporary audio file used during recording to a specified location.

* **func** **updateMeters**()
Refreshes the average and peak power values for all channels of an audio recorder.

* **func** **peakPower**(**channel**: **[Int](../gravity/int.md)**): <strong>[Float](../gravity/float.md)</strong> 
Returns the peak power for a given channel, in decibels, for the sound being recorded. The current peak power, in decibels, for the sound being recorded. A return value of 0 dB indicates full scale, or maximum power; a return value of -160 dB indicates minimum power (that is, near silence). If the signal provided to the audio recorder exceeds ±full scale, then the return value may exceed 0 (that is, it may enter the positive range).

* **func** **averagePower**(**channel**: **[Int](../gravity/int.md)**): <strong>[Float](../gravity/float.md)</strong> 
Returns the average power for a given channel, in decibels, for the sound being recorded. The current average power, in decibels, for the sound being recorded. A return value of 0 dB indicates full scale, or maximum power; a return value of -160 dB indicates minimum power (that is, near silence). If the signal provided to the audio recorder exceeds ±full scale, then the return value may exceed 0 (that is, it may enter the positive range).





