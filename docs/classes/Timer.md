**super**: **[Object](../gravity/object.md)**

A Timer object fires after certain time interval has elapsed.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called each time the timer fires.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **interval**: **[Float](../gravity/float.md)**
The number of seconds between firings of the timer. If interval is less than or equal to 0.0, this method chooses the nonnegative value of 0.1 milliseconds instead.

* **var** **repeat**: **[Bool](../gravity/bool.md)**
If true, the timer will repeatedly reschedule itself. If false, the timer will be stopped after it fires.

* **var** **isRunning**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the timer is currently started and running.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Initializers

* **func** **Timer**(): <strong>[instance](#)</strong> 
Initializes a timer object with a time interval equals to 0.0.

* **func** **Timer**(**interval**: **[Float](../gravity/float.md)**): <strong>[instance](#)</strong> 
Initializes a timer object with the specified time interval. The timer will be invalidated after it fires.

* **func** **Timer**(**interval**: **[Float](../gravity/float.md)**, **repeat**: **[Bool](../gravity/bool.md)**): <strong>[instance](#)</strong> 
Initializes a timer object with the specified time interval and repeat option. If the repeat option is true, the timer will repeatedly reschedule itself until invalidated, otherwise the timer will be invalidated after it fires.



### Methods

* **func** **start**()
Start timer.

* **func** **stop**()
Stop timer.





