**<span class="label label-release label-version">Creo 2.3</span>November 13th 2019 (Build 19092)**
* Added new print methods to [OSSharing](https://docs.creolabs.com/classes/OSSharing.html) class
* Added support for sharing in both directions
* Added support for [macOS app builder](https://docs.creolabs.com/creo/build-macos.html)
* Improved Camera
* Improved handling for gesture recognizer
* Exposed ModalPresentationStyle to all contains (Window, NavBar, TabBar, PageCurl, PageScroll, PageSplit)
* Exposed encoding methods to HTTPRequest class
* Various iOS 13 fixes
* Various macOS 10.15 fixes
* Fixed a memory leak in imageByCombiningImage
* Fixed an issue with build numbers incremented too quickly
* Fixed an issue with SplitView and landscape mode
* Fixed camera orientation in the Creo Simulator
* Fixed Gravity JSON double serializer
* Several internal fixes and improvements

**<span class="label label-release label-version">Creo 2.2.2</span>October 7th 2019 (Build 18991)**
* Added macOS 10.15 compatibility
* Added iOS 13 compatibility
* Added experimental IPA Upload feature
* Exposed iPhone 11/11 Pro/11 Pro Max
* Improved Apple iOS Simulator support
* Improved documentation for CreoPlayer exporting
* Added new DeviceOrientationDidChange event
* Several internal fixes and improvements

**<span class="label label-release label-version">Creo 2.2.1</span>September 18th 2019 (Build 18865)**
* Improved CollectionView flex support
* Improved exposed properties support in CustomView 
* Improved query editor
* Fixed a crash bug that can occurs when Camera access control is requested
* Several obscures crash bugs have been fixed
* Added new required privacy keys to plist
* CreoPlayer is now embedded into Creo (more info [here](https://docs.creolabs.com/creo/export_creoplayer.html))
* Several internal fixes and improvements

**<span class="label label-release label-version">Creo 2.2.0</span>September 16th 2019 (Build 18841)**
* Introduced new [Community Edition](https://creolabs.com/community_edition) version
* Added missed UIView events to CollectionView, TextField, TextView, Toolbar and WebView
* Added closure parameters to documentation
* Added macOS 10.15 compatibility (not yet notarized)
* Added animation flag to close method
* Added a new imageByCombiningImage method to Image class
* Added a new serverError property to DataSet
* Improved source code exporter
* Improved bindToSQL method
* Improved internal memory management on iOS
* Updated Gravity
* Exposed app.memoryUsage() method
* Fixed several cubeSQL issues
* Fixed HTTPRequest percent encoding
* CreoPlayer is now embedded into Creo (more info [here](https://docs.creolabs.com/creo/export_creoplayer.html))
* Several internal fixes and improvements

**<span class="label label-release label-version">Creo 2.1.8</span>August 31st 2019 (Build 18466)**
* Fixed a Window.openModal() issue

**<span class="label label-release label-version">Creo 2.1.7</span>August 30th 2019 (Build 18441)**
* Fixed two issues introduced in the 2.1.6 version
* **[Gravity documentation](https://docs.creolabs.com/gravity/)** has been updated.
* **[CreoPlayer 2.1.7](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.1.6</span>August 28th 2019 (Build 18423)**
* Added new OSSharing class
* Added new JSON class
* Added flex support to cell for automatic height
* Added localIdentifier (String), location (Map) and other properties to data returned by the CameraRoll dataset
* Added the possibility to use a multikey keypath for DataSet properties
* Added explicit toggleTorch method to Camera class
* Exposed enable, title and image of BarItems
* Exposed requireGestureRecognizerToFail method
* Improved OAuth2 authentication
* Improved syntax highlighter
* Improved Log Panel
* Fixed a double invocation of the DidShow event
* Fixed a TextField crash
* Fixed closures issues that can lead to a crash
* Fixed crash in database queries
* Fixed cubeSQL crash bug and fixed a BLOB related issue
* Several internal fixes and improvements
* **[CreoPlayer 2.1.6](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.1.5</span>July 15th 2019 (Build 18328)**
* Added support for Apple Simulator
* Several internal fixes and improvements
* **[CreoPlayer 2.1.5](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.1.2</span>June 28th 2019 (Build 18207)**
* Improved CubeSQL support
* Added a deleteAccessToken method to HTTPClient
* Added support for third party code editor themes
* Gravity console now support themes
* Exposed the modalPresentationStyle property to Windows (not simulated)
* Code Editor detached is now a global setting (and not a per project setting)
* Fixed a crash with NULL sql
* Fixed an issue with optional arguments in constructors
* New TechNote about code editor themes added to https://docs.creolabs.com/technotes/
* Several internal fixes and improvements
* **[CreoPlayer 2.1.2](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.1.1</span>June 14th 2019 (Build 18106)**
* Added the ability to mark code using Accent color
* Improved Code Editor
* Improved Exporter
* Fixed a couple of issues with split panels introduced in version 2.1.0
* Two new TechNotes added to https://docs.creolabs.com/technotes/
* Several internal fixes and improvements
* **[CreoPlayer 2.1.1](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.1.0</span>June 6th 2019 (Build 18073)**
* Added new split panel display mode
* Added new Live Code
* Added query parameters that may be included in the path of the HTTPClient class
* Added closures to capture and startRecording Camera methods
* Added TechDoc about sending an email with gmail
* Added support for application icon badges
* Exposed minPosition and maxPosition to Gradient class
* Exposed Camera position property
* Exposed the start and stop methods and isRunning property to Camera
* Exposed html property to WebView
* Improved Autocompletion
* Improved Exporter
* Improved documentation for BluetoothCentral
* Improved Camera control
* Fixed an issue with TabBar
* Fixed the order of calls of WillAppear/DidAppear/WillMoveToWindow/DidMoveToWindow methods 
* Fixed an issue with drag and drop of customviews to a new project
* Fixed an incorrect float to string conversion
* Several internal fixes and improvements
* **[CreoPlayer 2.1.0](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.0.8</span>May 9th 2019 (Build 17790)**
* Exposed Locale.preferredLanguages
* Fixed an issue with class properties/methods autocompletion
* Fixed an issue with range in shouldChangeCharactersInRange TextField event (still a work in progress)
* Improved position of autocompletion popover
* **[CreoPlayer 2.0.8](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.0.7</span>May 7th 2019 (Build 17756)**
* Improved autocompletion popover
* Improved local autocompletion
* Improved clone method (init constructor, if presents, must be manually called)
* Improved internal view drawing
* Improved subview handling
* Improved CAR file detection and generation 
* Improved save/restore size in Gravity Console
* Exposed imageInsets property to NavigationBar items
* Exposed backgroundObject property of views
* Exposed keyboardType, autocorrectionType, autocapitalizationType and spellCheckingType properties to TextView and TextField
* Exposed objectName to all objects
* Exposed Local to iOS
* Exposed NumberFormatter class
* Exposed Locale class
* Exposed methods indexPathForItemAtPoint, indexPathsForVisibleItems, indexPathForCell and cellForItemAtIndexPath to CollectionView and TableView
* Exposed view property to GestureRecognizer in order to be able to access the view the gesture recognizer is attached to
* Exposed view property to Window
* Exposed hitTest method to View
* ImageFilters can now be applied to Camera video too
* String split/loop is now unicode savvy
* Added initiallyStarted property to ActivityIndicator
* Added support for local enum
* Vectors filters are now float values
* Image/highlightedImage are now automatically updated when user programmatically changes the imagesRenderingMode of an ImageView
* Several improvements to the Camera control
* Several issues fixed related to ImageFilters
* Updated CubeSQL SDK
* Home/End keys mapped to beginning/end of line in code editor
* Various improvements to support subclassing of Creo native controls
* Various improvements to ImageView and ImageFilters:
* Fixed backgroundColor property of views
* Fixed an issue with the saveVideoToCameraRoll method
* Fixed an issue with internal nextCameraRollCount method
* Fixed an issue with continue keyword and for loops
* Fixed an issue with filters applied directly to Image (the issue was an infinite computed destination rect)
* Fixed an issue with views and autoresizing mask
* Fixed an issue where animation.isRunning always return false
* Fixed an issue related to clone method
* Fixed the initial orientation of the simulator when it is started from the design board presenting a custom view
* Fixed self parameter in complex postfix expression (loadat case)
* Fixed an issue in the color inspector with rgb/rgba string that only contain digits
* Fixed checkerboard for ImageView
* Fixed a layout issue when an object is deleted
* Fixed an issue with plist builder (bundle and short version switched)
* Fixed a frame conversion issue related to autoresizing mask
* Several other internal improvements and enhancements
* **[CreoPlayer 2.0.7](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.0.6</span>April 12th 2019 (Build 17448)**
* Added support for latest App Store requirements
* Added support for Compiled Asset Catalog (app icon CAR builder)
* Added ImageFilters support (based on CIFilters) to both Image and ImageView
* Added preliminary support for manifest typing to Gravity (used for local autocompletion in code editor)
* Added GravityConsole to quickly test Gravity code
* Added RGBBuffer object to Images in order to access pixel information
* Added Documents to the list of reserved keywords
* Exposed renderedImage property to ImageView
* Exposed clipsToBounds property to View inspectors
* Exposed reset method to WebView
* Exposed showAnnotations to MapView
* Exposed zoomValue property to MapView
* Exposed convertRect/convertPoint to all View subclasses
* Improved app builder generator
* Improved Flex documentation
* Improved code editor
* Improved Gravity language and virtual machine
* Preserved origin points when controls are dragged inside a view
* Fixed an issue with detached code editor
* Fixed custom view orientation in the custom view editor
* Fixed a disappearing bug in design board when resizing the document window with design board context created directly in landscape orientation
* Fixed visibleRect property and the trackingArea to update correctly the proposed selection frames in each possible interface orientation.
* Fixed first selected object when opening a detached code editor window
* Fixed an issue with AppStore.requestReview() method
* Fixed a couple of issue with TextField in secure mode
* Fixed a codegen issue
* Fixed a crash with gradient color
* Fixed a multiple selection issue after copying/duplicating multiple objects in design board
* Fixed a flex issue in calculating the content size when the view has flex width/height and content size flex
* Fixed a bug in resizing a TextView in landscape orientation, particularly evident if the TextView height is small and width is large
* Fixed a refresh issue with dataset not correctly reloaded when in cache
* Fixed a Gravity issue with nested for loops
* Fixed a padding issue in some Button configurations
* Fixed an issue that prevents two or more gestures to be recognized simultaneously
* Thanks to a new compilation process Creo should be now about 40% faster
* Several internal fixes and improvements
* **[CreoPlayer 2.0.6](https://creolabs.com/creoplayer)** will be available in about 24 hours via TestFlight

**<span class="label label-release label-version">Creo 2.0.4</span>March 8th 2019 (Build 16978)**
* Added new AudioRecorder class
* Added Horizontal and Vertical centered magnetic guides
* Added grid view to controls list
* Added an option to autoclose panel after a project has been sent to a device
* Added a new option to generate screenshots
* Added string.trim function
* Added custom fonts to plist and project in exporter
* Exposed new WillChangeToDisplayMode event to PageSplit
* Exposed view and subview to custom view
* Improved hittest on view controls and added an option to set a view as a passthrough
* Improved verification of IPA builder
* Improved Animation Panel
* Improved Sound class and fixed an issue on iOS devices
* Updated artworks for DesignBoard align menu and for bar system items
* Fixed cell height issue in the log panel
* Fixed several memory leaks in Gradients and Colors
* Fixed size of TableView header and footer
* Fixed some issues with movie assets
* Several internal fixes and improvements
* **[CreoPlayer 2.0.4](https://creolabs.com/creoplayer)** will be available via TestFlight in 24 hours

**<span class="label label-release label-version">Creo 2.0.3</span>February 21th 2019 (Build 16855)**
* Added a new RegEx class
* Added a new BonjourBrowser class
* Exposed several methods to the MoviePlayer
* Exposed insertRows method to the TableView
* TextField placeholder can now be customized 
* Redesigned and improved the Design Board Utility Bar
* Several UI improvements in MacOS 10.13
* Several CameraRoll related improvements and fixes
* Several cubeSQL and Database related fixes
* Improved OAuth2 HTTP authentication
* Improved Flex inspector
* Improved and fixed some issues in the GestureRecognizer
* Improved Carousel control (new itemHeight property and new DidScrollToCell event)
* Improved preview of Audio assets
* Improved exporter
* Fixed ActivityIndicator exporter
* Fixed an infinite loop with ActivityIndicator and Flex layout
* Fixed ghost windows issue
* Fixed an issue with the HTTPServer class
* Several internal fixes and improvements
* [CreoPlayer 2.0.3](https://creolabs.com/creoplayer) is now available on TestFlight

**<span class="label label-release label-version">Creo 2.0.2</span>February 5th 2019 (Build 16782)**
* Improved error reporting for runtime errors
* Improved performance of the Design Board
* Improved Yoga Layout
* Autocompletion is now case insensitive
* Added a new simpler way to send HTTPRequest from code
* Exposed DidTapReturn event and endEditingOnReturn property to TextField
* Code Editor now remembers selections for each object
* Double click on DesignBoard or Layout now loads Code Editor
* Added Keyboard dismiss mode to scrollview
* Exporter is now able to export Navigation Items, Gradients and Shapes
* Fixed exposition of iPad Pro 11"
* Fixed an issue with SegmentedControl
* Fixed objects toggle (cmd-6 now automatically set focus in SearchField)
* Fixed the Keyboard event sequences (Will/Did Show/Hide Keyboard and Will/Did Rotate window events) when a keyboard is presented and the interface is rotated
* Fixed the rotation animation of the Keyboard
* Several improvements for non-retina displays
* Several issues fixed in exposed properties for CustomViews
* Several issues fixed in the Exporter
* Several autoscroll issues has been fixed
* Several internal fixes and improvements
* **[CreoPlayer 2.0.2](https://creolabs.com/creoplayer)** will be available via TestFlight in 24 hours

**<span class="label label-release label-version">Creo 2.0.1</span>January 23th 2019 (Build 16655)**
* Exposed dismissMode property to ScrollView
* Added support for iPad Pro 11"
* Added a way to change text color for DatePicker and PickerView
* Updated AFNetworking to the latest version 3
* Improved registration process
* Improved memory usage and checker
* Fixed an issue with app builder process
* Several internal fixes and improvements
* **[CreoPlayer 2.0.1](https://creolabs.com/creoplayer)** will be available via TestFlight in 24 hours

**<span class="label label-release label-version">Creo 2.0</span>January 17th 2019 (Build 16612)**
* Dark and Light Mojave UI
* Swift code exporter
* Flex Layout support
* New DataSet classes for files and user's code
* Tons of others internal fixes and improvements
* **[CreoPlayer 2.0](https://creolabs.com/creoplayer)** is available now via TestFlight

**<span class="label label-release label-version">Creo 1.2.2</span>December 12th 2018 (Build 15618)**
* Added cubeSQL support
* Added isCreoKit, isCreoPlayer and isRealDevice to Device class
* Improved readString method in FileManager class
* Fix a crash that occurred with a NULL font 
* Fixed random issue with registered creo versions not correctly recognized
* Fixed ipa builder
* Several fixes related to TableView
* Several fixes related to TabBar
* Updated Gravity to the latest version
* A lot of other internal fixes and improvements
* **[CreoPlayer 1.2.7](https://creolabs.com/creoplayer)** is required and it should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.2.0</span>November 23th 2018 (Build 15544)**
* Exposed a lot of new properties and methods to Camera control
* Extended Camera control with barcode scanning capabilities
* Extended CameraRoll (it can now save metadata)
* Extended Crypto class with base64 encoding methods
* Added IP address methods to NetworkReachability class
* Improved autocompletion for some classes
* Exposed new events to all UI controls: WillShow, DidShow, WillHide, DidHide
* Added a second ndigits precision parameter to the Math.round method
* Fixed an old issue with the TextField in secure mode
* Fixed a Mojave specific issue that affects the Font class
* Several issues fixed related to Undo/Redo
* Several issue fixed in the HTTPServer class
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.8</span>October 29th 2018 (Build 15378)**
* Improved error reporting on App building panel
* Improved Math.random
* Improved NavigationBar emulation
* Improved Toolbar and BarButtons
* Extended RecordSet with intValue, int64Value, floatValue, doubleValue and boolValue
* Exposed lensAperture to Camera
* Exposed a new valueForIndex method to DataSet
* Exposed TimeZone class
* Added DidSelectAnnotation/DidDeselectAnnotation events to MapView
* Exposed ShouldChangeText event to TextField (see )
* Query editor is now able to succesfully execute non select statements
* TableView dataSet can now be set to null
* Fixed a FileManager issue
* Fixed a Map annotation issue
* Fixed a HTTPRequest issue
* Several issues fixed in Gesture objects
* New general Creo documentation available on **[https://docs.creolabs.com/creo](https://docs.creolabs.com/creo)**
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.7</span>October 9th 2018 (Build 15242)**
* Several UI fixes for 10.14 Mojave
* Improved TableView
* Improved Label, TextField and TextView
* Improved SQLite support
* Navigation has been renamed to NavigationBar
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.6</span>September 26th 2018 (Build 15134)**
* Improved error reporting
* Improved DataSet selection from Inspectors
* Improved HTTPClient JSON handling
* Improved PageContainer
* Improved InputView support
* Added support for new iPhone XR/XS/XS Max devices
* Added support for custom url in Application
* Fixed a potential crash bug introduced in 1.1.5 version
* Fixed some potential issue due to race conditions
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.5</span>September 19th 2018 (Build 15032)**
* Added Search panel
* Greatly improved compiler and runtime error reporting
* SQLite databases can now be automatically copied on a read-write directory on real iOS devices
* Added a new Advanced preference to control message sent to NULL behaviours
* Application events are now correctly raised within the Simulator
* Console.write on a real device now log directly to system log
* Added the ability to schedule local notifications
* Added the NetworkReachability class to check the network status
* Added Device.vibrate() method
* Fixed an issue with Large Title in NavigationBar
* Fixed an issue with WebView
* Fixed minor issues with TableView header and footer
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.1</span>September 10th 2018 (Build 14655)**
* Fixed several ScrollView issues (introduced in the 1.1.0 version). These issues affect several controls like PickerView, DatePicker and TableView.
* Increased compatibility with the upcoming MacOS 10.14 Mojave release.

**<span class="label label-release label-version">Creo 1.1.0</span>September 7th 2018 (Build 14633)**
* Added support for Safe Area (with preview)
* Added new DatabaseRecord class
* Added Toolbar item subnodes to NavigationBar
* New inspectors for all objects
* New subnodes added to several controls
* Improved Simulator performance
* Several fixes and enhancements to ScrollView
* Several fixes to PickerView
* Several fixes to SQLite database built-in inspector
* Several fixes to TableView
* Fix for SystemButton in iPhone X
* Fix for BezierPath image method
* Fix for RefreshControl position in NavigationBar
* Tons of others internal fixes and improvements
* **[CreoPlayer](https://creolabs.com/creoplayer)** has been updated and it is now available through the TestFlight program

**<span class="label label-release label-version">Creo 1.0.8</span>July 31st 2018 (Build 14201)**
* Improved NavigationBar class with new blur layer and others internal improvements
* Improved Window class with exposed firstResponder and new methods to convert from/to the Window's view coordinate system
* Improved TableView
* Improved Open/OpenIn/OpenModal methods
* Improved ChartView
* Improved Map with new Annotations related methods and properties
* Improved performance for large projects
* Added an optional closure parameter to the Open method (that will be executed by the newly opened Window/Navigation)
* Exposed autoresizingMask property to all UIView subclasses
* Fixed an issue with ExposedEvents
* Fixed an issue with Image class
* Others internal improvements and fixes
* New documentation engine at **[https://docs.creolabs.com/](https://docs.creolabs.com/)**. Users can submit examples, articles or any other improvement via our new public **[GitHub](https://github.com/creoapp/documentation/)** repo.

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
* **[CreoPlayer](https://creolabs.com/creoplayer)** is now available through the TestFlight program
* Added a new Properties and Privacy panel
* Added support for class properties and methods in custom classes
* Improved StatusBar support
* Exposed anchorPoint property in Inspector Geometry
* Fixed an issue with application builder and the Development Distribution target
* Fixed the default redirect callback url scheme for oAuth1 and oAuth2 in HTTPClient class. The new uri is **com.creolabs.creo://oauth2Callback**
* Several crashes has been fixed thanks to the feedback from our users
* Several others internal fixes and improvements

**<span class="label label-release label-version">Creo 1.0.2</span>June 21st 2018 (Build 13657)**
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
* **[CreoPlayer](https://creolabs.com/creoplayer)** version 1.1 or higher is now required
