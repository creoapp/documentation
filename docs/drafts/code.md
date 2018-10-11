Creo greatly reduces app development time by automate the most common tasks with a simple drag'n drop interface but there are time where you need to write Gravity code in order to customize behaviours or to enhance default cases.
<br><br>
In Creo **everything is an object**. That means that every object can be selected and modified using both the Inspector or the Code Editor on the bottom. You usually use the Code Editor to modify values that can change at runtime while the Inspector is usually used to modify values that changes at design time.
![Creo](images/code_1.png)

Each object comes with a predefined set of events and an empty set of methods and properties that you can customize. Events notify you about important changes that could require your interactions. For example, a Slider notifies that its value has changed using the Changed event, while a Button notifies that it has been touched using the Action event. By filling the appropriate events you can customize object’s behaviors to better fit your needs.

Every object can be further customized by adding functionalities (methods) and properties. 
When a property is transformed to a computed property, it can be much more than a simple static value. It can hide a lot of implementation details and it can be used as a way to add a lot of power to your custom classes.

For example, if you add a _state__ property to a Window then it will represent a static information that you can use later in your programming logic but if you transform that variable to a computed property (right-click on its name) then you can add a lot of logic when it is set (written) or get (read).

![Creo](images/code_2.png)

The _get_ section represents the code that needs to be executed when your property is read or accessed in your code (for example in ```var myState = Window1.state```). The _set_ section represents the code that needs to be executed when your property is written (for example in ```Window1.state = myState```).

![Creo](images/code_3.png)

In order to know which methods and properties an object can respond to you can consult the [Classes](https://docs.creolabs.com/classes/) section of the documentation. An object respond to its own methods and properties and to all the methods and properties of its super classes.