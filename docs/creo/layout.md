Setting up the main navigation hierarchy using a traditional system involves a considerable amount of time because it requires you to know the underline architecture of such components. With **Creo** the entire process is greatly simplified and you just drag and drop to setup your navigation hierarchy and it will be ready to use as soon as you release the mouse button.

### Setting up navigation hierarchy
You setup the navigation hierarchy by adding new windows and navigations to the **LAYOUT** panel. Everything is explicit and intuitive. Navigations are containers for Windows and Windows are containers for objects. Navigations and Windows can be moved or rearranged inside the Layout panel enabling you to perform test and experiments without writing a single line of code. A Window can contain controls (UI objects) and objects (objects without a UI like databases, classes, HTTP connections and so on).

![Creo](creo_layout_1.png)
You add Navigations and Windows using the containers panel located below the Layout section:
![Creo](creo_layout_2.png)

### Startup Window
Startup Window is the first window to display at startup. You can set the Startup Window using a contextual menu.  If you do not set a Startup Window in the **LAYOUT** panel then you’ll need to set it up using code inside the DidStart Application event.
![Creo](creo_layout_3.png)
