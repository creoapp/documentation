**super**: **[Object](../gravity/object.md)**

The Font class provides the interface for getting and setting font information. The class provides you with access to the font's characteristics and also provides the system with access to the font’s glyph information, which is used during layout. You use font objects by passing them to methods that accept them as a parameter.



### Properties

* **var** **familyName**: **[String](../gravity/string.md)**
The font family name. \(read-only\)

* **var** **fontName**: **[String](../gravity/string.md)**
The font face name. \(read-only\)

* **var** **pointSize**: **[Float](../gravity/float.md)**
The receiver’s point size, or the effective vertical point size for a font with a nonstandard matrix. \(read-only\)

* **var** **ascender**: **[Float](../gravity/float.md)**
The top y-coordinate, offset from the baseline, of the receiver’s longest ascender.  \(read-only\)

* **var** **descender**: **[Float](../gravity/float.md)**
The bottom y-coordinate, offset from the baseline, of the receiver’s longest descender.  \(read-only\)

* **var** **capHeight**: **[Float](../gravity/float.md)**
The receiver’s cap height information. \(read-only\)

* **var** **xHeight**: **[Float](../gravity/float.md)**
The x-height of the receiver. \(read-only\)

* **var** **lineHeight**: **[Float](../gravity/float.md)**
The height of text lines (measured in points). \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **systemFont**(**size**: **[Float](../gravity/float.md)**): <strong>[Font](Font.md)</strong> 
Returns the font object used for standard interface items in the specified size.

* **func** **boldSystemFont**(**size**: **[Float](../gravity/float.md)**): <strong>[Font](Font.md)</strong> 
Returns the font object used for standard interface items that are rendered in boldface type in the specified size.

* **func** **italicSystemFont**(**size**: **[Float](../gravity/float.md)**): <strong>[Font](Font.md)</strong> 
Returns the font object used for standard interface items that are rendered in italic type in the specified size.

* **func** **familyNames**(): <strong>[List](../gravity/list.md)</strong> 
Returns an array of font family names available on the system.

* **func** **fontNames**(**familyName**: **[String](../gravity/string.md)**): <strong>[List](../gravity/list.md)</strong> 
Returns an array of font names available in a particular font family.

* **func** **systemFontSize**(): <strong>[Float](../gravity/float.md)</strong> 
Returns the size of the standard small system font.



### Initializers

* **func** **Font**(**name**: **[String](../gravity/string.md)**, **size**: **[Float](../gravity/float.md)**)
A new font object with the given PostScript name and point size.

<pre><code class="swift">var font = Font("Helvetica", 12.0);</code></pre>





