Setting up a user interface for a mobile application usually involves the creation of a navigation hierarchy and then the creation of controls that can interact with the end user. Using a traditional design tool you are usually forced to use static objects that can simulate an UI and then the developers should translate these static representations into objects and other software components. With **Creo** there are no differences between design and development and so once you created a user interface you'll end up having a ready to use system without any further development.



Setting up the main navigation hierarchy using a traditional system involves a considerable amount of time because it requires you to know the underline architecture of such components. With **Creo** the entire process is greatly simplified and you just need to use drag and drop to setup your navigation hierarchy that will be ready to use as soon as you'll release the mouse button.


#### Setting up navigation hierarchy
To setup the navigation hierarchy add new windows and navigations into the **LAYOUT** panel. Everything is explicit and really intuitive. Navigations are containers for Windows and Windows are containers for objects. Navigations and Windows can be moved or rearranged inside the Layout panel enabling you to perform test and experiments without writing a single line of code. A Window can contain controls (UI objects) and objects (objects without an UI like databases, classes, HTTP connections and so on).

![Creo](../images/creo/user-interface-creation.png)
You add Navigations and Windows using the containers panel located below the Layout section:
![Creo](../images/creo/user-interface-creation-3.png)


#### Adding controls and objects
As we already said a Window is a container for controls and objects and in order to create objects you just need to use drag and drop from the Objects panel to the currently selected Window displayed in the Design Board.
![Creo](../images/creo/user-interface-creation-4.png)


Once a control has been instantiated using drag and drop, you can customize its appearance and behaviour using the Inspector Panel. The same inspector can be used to configure navigations, windows and more generally every object listed in the Layout panel.
![Creo](../images/creo/user-interface-creation-5.png)


#### Startup Window
Startup Window is important because it instructs your app about what is the first window to display at startup. A Startup Window can be set using a contextual menu, if you do not set a Startup Window then you’ll need to setup it using the code. The appropriate way to setup a Startup Window is inside the DidStart Application event.
![Creo](../images/creo/user-interface-creation-2.png)
