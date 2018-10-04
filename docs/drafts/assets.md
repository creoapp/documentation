An asset is a resource needed at some point by your application. Common assets are images, sounds, movies and in general any other document. The Assets folder represents the central repository for all your resources. Just drop a resource from the Finder to the Assets folder in order to automatically have it copied into your Creo project. For common resources like images, sounds and movies, Creo offers a real-time preview (and play) directly from within the Assets folder.

![Creo App](images/creo_assets_1.png)

Each time you drop your resources, Creo ask if you want to have them converter to Object.

![Creo App](images/creo_assets_2.png)

If you choose No then the file is copied to the Creo project without any further processing and you'll be able to access it using FileManager's functionality like we shown in the [FileManager](tutorials/file-manager.md) tutorial. If you reply Yes then the assets is internally converted to the appropriate Creo object (Image and Sound for example) and you'll be able to use it directly from Gravity code.

```
// play the submarine sound from the Assets folder
submarine.play()
```

### Images

On a standard-resolution screen, one point is equal to one pixel. High-resolution screens have a higher pixel density. Because there are more pixels in the same amount of physical space, there are more pixels per point. As a result, high-resolution displays require images with more pixels.

![Creo App](images/creo_assets_3.png)

Depending on the device, you accomplish this by multiplying the number of pixels in each image by a specific scale factor. A standard resolution image has a scale factor of 1.0 and is referred to as an @1x image. High resolution images have a scale factor of 2.0 or 3.0 and are referred to as @2x and @3x images.

Creo automatically choose the best resolution image for the device when it is running, your only responsibility is to provide the image with all the required resolutions.


![Creo App](images/creo_assets_4.png)

In this example the Desktop image is provided only at @1x resolution and you can see the missing @2x and @3x resolutions in red in the top-left corner of the image box.