# Timer

**super**: [Object](Object.md)

A Timer object fires after certain time interval has elapsed.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called each time the timer fires.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Properties

* **var** **interval**: **[Float](../gravity/types.md)**
The number of seconds between firings of the timer. If interval is less than or equal to 0.0, this method chooses the nonnegative value of 0.1 milliseconds instead.

* **var** **repeat**: **[Bool](../gravity/types.md)**
If true, the timer will repeatedly reschedule itself. If false, the timer will be stopped after it fires.

* **var** **isRunning**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether the timer is currently started and running.

</ul>

### Initializers

* **func** **Timer**(): <strong>[instance](#)</strong> 
Initializes a timer object with a time interval equals to 0.0.

* **func** **Timer**(**interval**: <strong>[Float](../gravity/types.md)</strong>): <strong>[instance](#)</strong> 
Initializes a timer object with the specified time interval. The timer will be invalidated after it fires.

* **func** **Timer**(**interval**: <strong>[Float](../gravity/types.md)</strong>, **repeat**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[instance](#)</strong> 
Initializes a timer object with the specified time interval and repeat option. If the repeat option is true, the timer will repeatedly reschedule itself until invalidated, otherwise the timer will be invalidated after it fires.

</ul>

### Methods

* **func** **start**()
Start timer.

* **func** **stop**()
Stop timer.

</ul>

</ul>

