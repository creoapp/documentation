A `PageContainer` control is an onscreen element that provides a way to implement linear navigation between pages of content, such as in a document, book, notepad, or calendar. Pages fluidly scroll from one to the next or turn like pages in a physical book.

![PageContainer](images/PageContainer_main.png)

### Best practices
When a `PageContainer`is used, pages flow sequentially and there’s no way to jump between nonadjoining pages. If people may need to access pages out of sequence in your app, implement a custom control that provides this functionality.

### How to use
1. Drop a `PageContainer` control from the object panel to a `Window`
1. Use the `PageContainer Inspector` to customize its _Navigation style_ properties like `DataSet`, `Style` and its _Page Curl_ properties like `Style`

![PageContainer inspector](images/PageContainer_inspector.png)
The inspector where the `PageContainer` class can be configured.

### Example
1. Drop a `PageContainer` control from the object panel to a `Window`
1. Create a _DataSet_ of pictures by dropping images in the _Project_ -> _Assets_ folder
1. Set the `PageContainer` _DataSet_ property to _Asset_; now you can test the pages transition by tapping _Play_
1. Drop an `ImageView` and a `Label` onto the `PageContainer` -> `CustomView1`. The ending hierarchy should looks like

```
- Navigation1
 - Window1
  - PageContainer1
   - CustomView1
    - ImageView1
    - Label1
```

5. Select `CustomView1` and tap the _Custom Properties_ button on the _Inspector_ topbar.
1. Right click and select _New Property_
1. Add a property named "_Image_" and bind it to _ImageView1.image_
1. Add a property name d"_Label_" and bind it to _Label1.text_

![PageContainer binding](images/PageContainer3.png)

9. Open the `PageContainer` inspector and select _Cell Properties_
1. Assign to _Label_ the value _Name_
1. Assign to _Image_ the value _Image_
1. Tap _Play_ to see how the `PageContainer` content is now rendered with the _Assets_ image and name
1. Swipe to scroll

### Most important properties
Several aspects can be configured in the `PageContainer` class but the most important are:
- `DataSet`: To set the content source for the `PageContainer`
- `Style`: _PageCurl_ for turning pages like a book, _PageScroll_ to fluidly scroll from one to the next page

### References
[PageContainer class reference](../classes/PageContainer.html) contains a complete list of properties and methods that can be used to customize a `PageContainer` object.
