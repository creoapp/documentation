**super**: [Object](Object.md)

It is a graphics rendering and animation infrastructure that you use to animate the views and other visual elements of your app. On iOS it is a Core Animation. An animation object is implicity created by the runtime system and it represents an instance of an animation created within the Animation Editor inside CREO IDE.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillStart**()
Animation will start.

* **DidStart**()
Animation is started.

* **Completed**()
Animation is completed

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **isRunning**: **[Bool](../gravity/types.md)**
Check if animation is running. \(read-only\)

* **var** **speed**: **[Float](../gravity/types.md)**
The speed of the animation.



### Methods

* **func** **play**()
Start animation (asynchronously).

* **func** **pause**()
Pause animation.

* **func** **resume**()
Resume animation.

* **func** **stop**()
Stop animation.

* **func** **reverse**()
Start animation in reverse mode.





