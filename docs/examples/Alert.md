### Examples

#### A simple Alert:
```
var alert = Alert("Title", "Hello, I am an Alert.");
alert.show();
```
Result:
![Simple Alert](../images/examples/alert-2.png)

#### A two buttons Alert:
```
var alert = Alert("Title", "Hello, I am an Alert.", ["Cancel", "OK"]);
alert.show();
```
Result:
![Two buttons Alert](../images/examples/alert-3.png)

#### A three buttons Alert:
```
var alert = Alert("Title", "Hello, I am an Alert. Are you ready?", ["Maybe", "Yes", "No"]);
alert.show();
```
Result:
![Three buttons Alert](../images/examples/alert-4.png)


#### Use a callback to check for button pressed:
```
var callback = func (index) {
	var alert = Alert("", "You pressed button \(index).")
	alert.show();
}

var alert = Alert("Title", "Hello, I am an Alert. Are you ready?", ["Maybe", "Yes", "No"], callback);
alert.show();
```
Result:
![Complex Alert](../images/examples/alert-5.png)
