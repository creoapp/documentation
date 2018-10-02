A map view lets you display geographical data within your app and supports most of the functionality provided by the built-in Maps app. A map view can be configured to show a standard map, satellite imagery, or both. It can include pins and overlays, and supports zooming and panning. If your app supports routing, such as in a run-tracking app, you can use a map view to display the route.

![MapView](images/mapview1.png)

### Best practices
* **In general, keep your map interactive.** People are accustomed to using gestures to interact with the Maps app, and expect to be able to interact with your map in similar ways.
* **Use expected pin colors.** A pin identifies a point of interest on your map. People are familiar with the standard pin colors in the Maps app. Avoid redefining the meaning of these colors in your app. Use red for a destination, green for a starting location, and purple for a user-specified location.

### How to use
1. Drop a `MapView` control from the object panel to a `Window`
2. Use the `MapView Inspector` to customize its properties like `Map Type`, `Address`, `Latitude`, `Longitude` and `Zoom`

If you need to write code for MapView:

3. Open the `Code Editor` (cmd + 6)
4. Select the `LocationDidChange` item inside the `Events` area and write your custom code in the `Code Editor`

![`MapView` inspector](images/mapview2.png)
The inspector where the `MapView` class can be configured.

### Example
1. Open the `Code Editor` (cmd + 6)
2. Select the `LocationDidChange` item inside the `Events` area and write your custom code in the `Code Editor`
```
Console.write("MapView value: \(self.value)")
```

### Most important properties
Several UI aspects can be configured in the `MapView` class but the `address`, `latitude`, and `longitude` are the most populars to be configured.
- `address`: A string describing the location you want to center the map to.
- `latitude`: The latitude of the center point of the visible area.
- `longitude`: The longitude of the center point of the map.

### References
[MapView class reference](../classes/MapView.html) contains a complete list of properties and methods that can be used to customize a `MapView` object.
