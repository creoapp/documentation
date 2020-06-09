**Starting from Creo 2.4 there is now support for GIF/MP4 movie creation starting from a series of static Images**

**Create GIF/MP4movie**

The core functionalities are included in two API:
- Movie.createMP4
- Movie.createGIF

In this example we'll use a List of path to Images (instead of a List of Images) because it makes a much better use of memory resources.

```
// Create the input List
var r = ["path_to_image1.jpg",
"path_to_image2.jpg",
"path_to_image3.jpg",
"path_to_image4.jpg",
"path_to_image5.jpg",
"path_to_image6.jpg",
"path_to_image7.jpg"];


// Setup completion closure
func completion (result: Bool, error: String) {
	Console.write("\(result) \(error)")
}


// Setup output paths
var output1 = "/Users/marco/Pictures/CameraRoll/movie.mp4";
var output2 = "/Users/marco/Pictures/CameraRoll/movie.gif";

// Perform conversions
Movie.createMP4(r, output1, 4, completion)
Movie.createGIF(r, output2, 0, 0.2, completion)
```

The resulting MP4 can be displayed in a MoviePlayer control, while the GIF file can be displayed in an ImageView using the following code:

```
// output2 is the path to the GIF file
var img = Image.loadGIF(output2);
ImageView1.image = img
ImageView1.startAnimating()
```