```
var pattern = "A.C";
var string = "AABCAABCBBABC";
var replacement = "ZZZ";
var options = 0;

var count = RegEx.count(pattern, string, options)
var list = RegEx.search(pattern, string, options)
var ranges = RegEx.ranges(pattern, string, options)
var replace = RegEx.replace(pattern, string, replacement, options)

Console.write("Count: \(count)")
Console.write("List: \(list)")
Console.write("Ranges: \(ranges)")
Console.write("Replace: \(replace)")
```
Result in Creo Console panel:
```
Count: 3
List: [ABC,ABC,ABC]
Ranges: [1...3,5...3,10...3]
Replace: AZZZAZZZBBZZZ
```

More on RegEx syntax can be found at:
* [https://developer.apple.com/documentation/foundation/nsregularexpression](https://developer.apple.com/documentation/foundation/nsregularexpression)
* [https://www.raywenderlich.com/2725-nsregularexpression-tutorial-and-cheat-sheet](https://www.raywenderlich.com/2725-nsregularexpression-tutorial-and-cheat-sheet)
* [http://userguide.icu-project.org/strings/regexp](http://userguide.icu-project.org/strings/regexp)
* [http://www.unicode.org/reports/tr18/](http://www.unicode.org/reports/tr18/)

