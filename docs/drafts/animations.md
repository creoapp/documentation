User experience in modern mobile apps is boosted by animations, they are used everywhere to increase usability and to give you the touch and feeling of important tasks being performed.
Unfortunately creating efficient animations is not an easy task, you need to know a lot of implementation details, you need to spend time performing complex math operations and most of the time you don't have a real time feedback about what is happening. 
<br>
<br>
**Creo** introduces a new way to create animations with an intuitive timeline interface like the one you can find in professional video maker tool. Just drop the object you want to animate into the animation panel and start experimenting with properties, settings and timing. Once done the result will be a native Core Animation object that will be executed at native speed on your device.

By default, once finished, animations will restore all values to the initial state. If you want the animation to remains at the final state, then check the **Preserve final state** setting in the Animation inspector.

![Creo](images/creo_animations_1.png)

### Creating animation with code

Each object with a user interface (technically speaking each object that inherits from the UIView class) has an animate method that can be used to perform animations via code.
```
func animate(duration: Float, delay: Float, options: AnimationOption, closure: Closure, completion: Closure)

duration: The total duration of the animations, measured in seconds. If you specify a negative value or 0, the changes are made without animating them.
delay: The amount of time (measured in seconds) to wait before beginning the animations. Specify a value of 0 to begin the animations immediately.
options: A mask of options indicating how you want to perform the animations. See AnimationOptions enum for more information.
closure: A block object containing the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.
completion: A block object to be executed when the animation sequence ends. This block has no return value and takes a single Boolean argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle. This parameter may be null.
```

