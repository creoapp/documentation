Applications built with Creo acts and behave like any other regular iOS app compiled with Xcode. Some technical details and customizations can be configured using an Info.plist file.
If you choose **Project** **›** **Properties** from the menu then you can customize your iOS specific settings.
Please note that Creo take care of configuring and writing a correct Info.plist file for you. You should change these settings only if you really know what you are doing.

![Creo App](images/creo_properties_1.png)

For a complete list of supported keys and values, you can consult official [Apple Documentation](https://developer.apple.com/library/archive/documentation/General/Reference/InfoPlistKeyReference/Articles/iPhoneOSKeys.html#//apple_ref/doc/uid/TP40009252-SW1).

### Privacy messages

Users must grant permission for an app to access personal information, including the current location, calendar, contact information, reminders, and photos. Although people appreciate the convenience of using an app that has access to this information, they also expect to have control over their private data. For example, people like being able to automatically tag photos with their physical location or find nearby friends, but they also want the option to disable such features.
The Privacy panel lets you personalize all the requests (with a detailed explanation) to your end user.

![Creo App](images/creo_properties_2.png)