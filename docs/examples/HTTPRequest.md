#### Programmatically create a simple HTTPRequest to download an image
```
// Create a new HTTPRequest for with the specified URL
var request = HTTPRequest("https://www.creolabs.com/img/creo_shot1_dark.png")

// Configure the response serializer, in this example we expect the response
// content to be an Image
request.responseSerializerType = HTTPResponseSerializer.Image

// Code to execute in case of success
func onSuccess(request,value) {
	// The first argument of the closure is the HTTPRequest.
	// The second argument is the content of the response,
	// the type of this object depends on the configured
	// responseSerializerType, in this example it is an Image.
    ImageView1.image = value
}

// Code to execute in case of success
func onError(request,error) {
    // The first argument of the closure is the HTTPRequest.
	// The second argument is the returned error message.
	Console.write("Error: \(error)")
}

// Send the request
request.send(onSuccess,onError)
```

#### Download a JSON content and use it as the DataSet of a TableView
```
// Create a new HTTPRequest for with the specified URL
var request = HTTPRequest("https://jsonplaceholder.typicode.com/posts")

// Configure the response serializer, the response content will be
// deserialized to a Map object and set to the "value" property of the HTTPRequest
request.responseSerializerType = HTTPResponseSerializer.JSON

// Set the request as the dataSet of a control, in this case a TableView.
// The "KeyPath" property and the Cell Properties of the control must be configured
// to use the proper values of the desirialized JSON, for this sample URL the KeyPath
// propery must be empty and the Text property must be set to "title".
// The run() method of the dataSet is automatically called by the TableView
// when the dataSet property is set.
TableView1.dataSet = request
```
