#### Share an Image:
```
var image = MyGreatImage;
OSSharing.shareImage(image);
```

#### Share a String:
```
var s = "Hello World";
OSSharing.shareString(s);
```

#### Share a URL:
```
var url= "https://creolabs.com";
OSSharing.shareURL(url);
```

#### Share an Image and a String:
```
var image = MyGreatImage;
var s = "Hello World";
var share: OSSharing = OSSharing();
share.items = [image, s];
share.show();
```