**<span class="label label-release label-version">Creo 1.0.7</span>July 19th 2018 (Build 14057)**
* Improved WebView
* Improved String.split method and added new String.replace and String.contains methods
* Exposed idleTimerDisabled Boolean flag to App instance
* Improved TextField and SearchBar
* Added Map annotation basic implementation
* Improved syntax error line recognition
* Fixed colorBorder property
* Various fixes and improvements to PageScroll and PageCurl
* Various fixes and improvements to TabBar and NavigationBar
* Added a workaround for iPad multitasking not yet supported
* Improved iOS app build process
* Various fixes and improvements to TableView
* Exposed new Application type setting
* Various fixes and improvements to the Property List editor
* Fix for Exposed Events
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.6</span>July 12th 2018 (Build 13963)**
* Fixed a crash with some combination characters in the code editor
* Added the ability to execute JavaScript from the WebView (and callback Gravity code)
* Added setFocus/clearFocus method  to controls
* Fixed Actions Inspector for non UI objects
* Added address property to MapView
* New useful properties added to Device and App objects
* Fixed an issue with mySQL TEXT field recognized as BLOB
* Fixed the status bar properties of the App object
* Various fixes and improvements to the HTTPClient Request class
* Fix for deleted gesture recognizer
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.5</span>July 6th 2018 (Build 13895)**
* Fixed an issue in generated apps with a registered Creo version
* Added format method to Date class (with an example in documentation)
* Improved autocompletion
* [Build your app](https://docs.creolabs.com/creo/build-your-app.html) tutorial has been updated with a new "Submit your app to the App Store" section and an "Apple Configurator 2" tutorial
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.4</span>July 5th 2018 (Build 13884)**
* Fixed an issue in Preferences.write method
* Fixed an issue with local html files and WebView
* Fixed an issue with Database.execute
* Fixed an issue with labelsColumn parameter of ChartView
* [Spotify](https://docs.creolabs.com/tutorials/spotify.html) tutorial has been updated
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.3</span>July 3rd 2018 (Build 13867)**
* **[CreoPlayer](http://creoplayer.creolabs.com)** is now available through the TestFlight program
* Added a new Properties and Privacy panel
* Added support for class properties and methods in custom classes
* Improved StatusBar support
* Exposed anchorPoint property in Inspector Geometry
* Fixed an issue with application builder and the Development Distribution target
* Fixed the default redirect callback url scheme for oAuth1 and oAuth2 in HTTPClient class. The new uri is **com.creolabs.creo://oauth2Callback**
* Several crashes has been fixed thanks to the feedback from our users
* Several others internal fixes and improvements

**<span class="label label-release label-version">Creo 1.0.2</span>June 21th 2018 (Build 13657)**
* Added TestFlight support
* Small improvements in the Animation panel
* Improved performance of ImageView control
* Fixed some issues related to iOS lower than 11.0
* Fixed a crash issue in the Action panel

**<span class="label label-release label-version">Creo 1.0.1</span>June 18th 2018 (Build 13630)**
* Fixed a crash that occurred when a gradient was saved in favourites
* Fixed a crash that can occurs when zoom factor in multi-screen environments was returned as zero
* Improved multi display support
* Fixed an issue in TabBar controller
* Added a new Advanced panel in Preferences to check if beta versions should be checked in in-app updates
* Custom subclasses now correctly expose events from super class (more work needs to be done)
* Added a workaround for a 10.14 issue (as a result the Font class cannot be directly used in 10.14)

**<span class="label label-release label-version">Creo 1.0.0</span>June 13th 2018 (Build 13600)**
* First official release
* **[CreoPlayer](http://creoplayer.creolabs.com)** version 1.1 or higher is now required
