Autosize constraints (iOS Autoresizing masks) are based on the layout concept of `Struts and Springs`. You define which edges can change and which dimensions can change. Width and height are the `springs` they can stretch (if allowed) to keep the struts satisfied. The distance from left, top, right, and bottom are the `struts`. Struts can be fixed so they can't change or they can be flexible and allow change. You combine these options as a bit mask to create an Autoresizing mask to describe how you want the struts and springs to behave.

Creo offers a visual way to set Autoresizing masks but under the hood it is just a bitwise OR of values.

Here's a breakdown of what each option does:
* Autoresizing.FlexibleBottomMargin: Allow the distance between the bottom of the view and its container to change.
* Autoresizing.FlexibleHeight: Allow the height of the view to change in order to preserve the top and bottom struts (distances to the edge of the superview).
* Autoresizing.FlexibleLeftMargin: Allow the distance between the left side of the view and its container to change.
* Autoresizing.FlexibleRightMargin: Allow the distance between the right side of the view and its container to change.
* Autoresizing.FlexibleTopMargin: Allow the distance between the top of the view and its container to change.
* Autoresizing.FlexibleWidth: Allow the width of the view to change in order to preserve the top and bottom struts (distances to the edge of the superview).

You can combine these options with a bitwise OR operator '|'. This allows a very primitive 'automatic' layout system that can respond to changes in the size of a containing view.
For example, a view with frame rect of (10, 10, 50, 50) and a superview bounds of (0, 0, 70, 70)
Autoresizing.FlexibleWidth | Autoresizing.FlexibleHeight
would mean that no matter what the superview's size is, the view should always remain exactly 10pts from the top, left, bottom, and right of the superview. This means that the width and height must be able to change, which means they're flexible.

The same view with this mask
Autoresizing.FlexibleBottomMargin | Autoresizing.FlexibleRightMargin
would indicate that that view's width and height should remain fixed, as well as the top distance to the superview and the left distance to the superview. This means that a square of 50x50 would always be located at 10,10 no matter the size of the super view. The bottom and right margins were flexible, but nothing else was.

![Autoresizing](../images/technotes/autoresizing.gif)