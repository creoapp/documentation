A date picker is an efficient interface for selecting a specific date, time, or both. It also provides an interface for displaying a countdown timer.

![DatePicker](../images/creo/datepicker1.png)

### Best practices
* **Consider providing less granularity when specifying minutes.** By default, a minute list includes 60 values (0 to 59). You can optionally increase the minute interval as long as it divides evenly into 60. For example, you might want quarter-hour intervals (0, 15, 30, and 45).
* **Avoid switching screens to show a picker.** A picker works well when displayed in context, below or in close proximity to the field being edited.
* **Use a table instead of a picker for large value lists.** Long lists can be tedious to navigate in a picker. A table has adjustable height and can include an index, making scrolling much faster.

### How to use
1. Drop a `DatePicker` control from the object panel to a `Window`
2. Use the `DatePicker Inspector` to customize its properties like `Show`, `Date`, `Locale`, `Time Zone` and `Calendar`

If you need to write code for DatePicker:

3. Open the `Code Editor` (cmd + 6)
4. Select the `Changed` item inside the `Events` area and write your custom code in the `Code Editor`

![`DatePicker` inspector](../images/creo/datepicker2.png)
The inspector where the `DatePicker` class can be configured.

### Example
1. Open the `Code Editor` (cmd + 6)
2. Select the `Changed` item inside the `Events` area and write your custom code in the `Code Editor`
```
Console.write("DatePicker value: \(self.date)")
```

### Most important properties
Several UI aspects can be configured in the `DatePicker` class but the `datePickerMode`, `date`, and `localDate` are the most commons to be configured.
- `datePickerMode`: The date picker mode. Determines whether the date picker should display a time, a date, a time and date or a countdown interval. For modes that include date or time values, you can also configure the locale, calendar, and time zone information as appropriate.
- `date`: The date displayed by the date picker.
- `localDate`: The date displayed by the date picker computed with timezone and locale.

### References
[DatePicker class reference](../classes/DatePicker.html) contains a complete list of properties and methods that can be used to customize a `DatePicker` object.
