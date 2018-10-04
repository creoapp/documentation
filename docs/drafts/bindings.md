A binding is a **continuous** connection between 2 values. Continuous means that each time a value from Object1 changes than the updated value is propagated to the connected Object2 (if the two objects are connected with a Binding).


Binding is a very powerful concept in software development but it usually forces developers to learn new programming paradigms or to write some not very intuitive code. **Creo** offers a very intuitive way to create binding and all you have to do is graphically connects two objects using the Binding knob anchor point:
![Creo](images/bindings-1.png)

Once two objects are connected then you can configure the Binding using its Inspector:
![Creo](images/bindings-2.png)
In the above example we just continuously connected the value of the Slider1.value property to the Label1.text property. A Binding is just another object in the Layout pane that you can select and customize.

#### Advanced Binding
You usually create a Binding when you need to connect the properties of two objects. **Creo** greatly enhances binding functionalities enabling you to connect more than one object in a single binding. Suppose for example that you'd like to add to the user the ability to create a new Color, a **[Color](../classes/Color.html)** is a class that can be instantiated using an RGB value.


Start by dragging 3 Sliders and a View into the Design Board:
![Creo](images/bindings-3.png)

Create a binding between Slider1.value and View1.backgroundColor and then add Slider2.value and Slider3.value to the same Binding:
![Creo](images/bindings-4.png)

Select Binding1 on the Layout pane and open the SourceConversion event. This event is called each time the binding needs to send a value from source objects to the destination object. The value parameter represents a single value when there is only one SOURCE object, while it is an array of value when objects in the SOURCE group are more than once.
The resulting value is expected to be a Color (because the destination property is View1.backgroundColor) and if you read documentation about the **[Color](../classes/Color.html)** class (under the INITIALIZERS section) you can see that a way to create a new Color is just to instantiate the class passing 3 float parameters (which represent the Red, Green and Blue value). All of this can be done with a single line of code:
![Creo](images/bindings-5.png)

If you want to test your newly created code just press Run to see your app running into the Creo Simulator:
![Creo](images/bindings-6.png)
