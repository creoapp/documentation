#### Concepts
The eBook tutorial will show you how to use the powerful PageContainer control bounds to an Images folder. This example will also show you how to build a single Window application for iPad and how to change orientation.

#### Classes
* [Page Container](../classes/PageContainer.md)
* [CustomView](../classes/CustomView.md)
* [ImageView](../classes/ImageView.md)
* [View](../classes/View.md)	
		
#### Assets
* [Images](../assets/ebook_assets.zip) - images credits to [freephotos.cc](https://freephotos.cc)


#### Steps
++1++ Create a new empty Creo project and start by dragging the Images folder into the Assets folder (then press Yes to the object conversion question).
![eBook](../images/tutorials/ebook1.gif)

++2++ We do not need a Navigation in this example, so remove it:
![eBook](../images/tutorials/ebook2.gif)

++3++ Change device from iPhone 7 to iPad:
![eBook](../images/tutorials/ebook-2.png)

++4++ Change orientation from Portrait to Landscape Right:
![eBook](../images/tutorials/ebook-3.png)

++5++ Set Zoom level to "Fit To Screen" (command 0 as shortcut):
![eBook](../images/tutorials/ebook-4.png)

++6++ Set Window1 Status Bar Visibility to "Hidden":
![eBook](../images/tutorials/ebook-5.png)

++7++ Drag a View from Objects to Templates in order to create a new CustomView1:
![eBook](../images/tutorials/ebook-6.png)

++8++ Drag an ImageView into the CustomView, resize it to fit CustomView1 size and set its Constraints as shown in the screenshot:
![eBook](../images/tutorials/ebook-7.png)
In Object Inspector set ImageView1 Mode to Aspect Fill

++9++ Expose the ImageView1.image property to the CustomView (as Image):
![eBook](../images/tutorials/ebook-8.png)

++10++ Drag a PageContainer control from Object into Window1 and resize it to fit Window1 size:
![eBook](../images/tutorials/ebook-9.png)
What is a ContainerControl? So far we manually created the Windows for our app, so we needed to know in advance how many Windows our app will use. Most of the time this is perfectly fine but sometimes it would be really helpful to have a way to automatically creates Windows based on a DataSet and this is exactly what a ContainerControl does.

++11++ Configure PageContainer to have CustomView1 as Template and Assets as DataSet. You'll end up with something like:
![eBook](../images/tutorials/ebook-10.png)

++12++ Press RUN and enjoy the eBook app!
![eBook](../images/tutorials/ebook3.gif)

You can now send the app to **[CreoPlayer](../creo/creoplayer.md)** or **[build it](../creo/build-your-app.md)** and then submit to the App Store.

#### Project
* [eBook.creoproject]({{github_raw_link}}/assets/ebook.zip) (6.6MB)
