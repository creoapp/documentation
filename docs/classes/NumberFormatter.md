**super**: **[NSFormatter](NSFormatter.md)**

A formatter that converts between numeric values and their textual representations. The representation encompasses integers, floats, and doubles; floats and doubles can be formatted to a specified decimal position.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **numberStyle**: **[Int](../gravity/int.md)**
The number style used by the receiver. Styles are essentially predetermined sets of values for certain properties. Examples of number-formatter styles are those used for decimal values, percentage values, and currency.

* **var** **generatesDecimalNumbers**: **[Bool](../gravity/bool.md)**
Determines whether the receiver convert numbers to decimal when it converts strings to number objects.

* **var** **locale**: **[Locale](Locale.md)**
The locale of the receiver. The locale determines the default values for many formatter attributes, such as ISO country and language codes, currency code, calendar, system of measurement, and decimal separator.

* **var** **roundingIncrement**: **[Int](../gravity/int.md)**
The rounding increment used by the receiver.

* **var** **roundingMode**: **[Int](../gravity/int.md)**
The rounding increment used by the receiver.

* **var** **minimumIntegerDigits**: **[Int](../gravity/int.md)**
The minimum number of digits before the decimal separator. (Default to 0).

* **var** **maximumIntegerDigits**: **[Int](../gravity/int.md)**
The maximum number of digits before the decimal separator. (Default to 42).

* **var** **minimumFractionDigits**: **[Int](../gravity/int.md)**
The minimum number of digits after the decimal separator. (Default to 0).

* **var** **maximumFractionDigits**: **[Int](../gravity/int.md)**
The maximum number of digits after the decimal separator. (Default to 0).

* **var** **usesSignificantDigits**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the formatter uses minimum and maximum significant digits when formatting numbers.

* **var** **minimumSignificantDigits**: **[Int](../gravity/int.md)**
The minimum number of significant digits for the number formatter. You must set the usesSignificantDigits property to true in order for this property to affect formatting behavior. By default, the minimum number of significant digits is 1.

* **var** **maximumSignificantDigits**: **[Int](../gravity/int.md)**
The maximum number of significant digits for the number formatter. You must set the usesSignificantDigits property to true in order for this property to affect formatting behavior. By default, the maximum number of significant digits is 6. Values less than 1 are ignored.

* **var** **negativeFormat**: **[String](../gravity/string.md)**
The format the receiver uses to display negative values. More information about expected format values from http://www.unicode.org/reports/tr35/tr35-numbers.html#Number_Format_Patterns

* **var** **positiveFormat**: **[String](../gravity/string.md)**
The format the receiver uses to display positive values. More information about expected format values from http://www.unicode.org/reports/tr35/tr35-numbers.html#Number_Format_Patterns

* **var** **formatWidth**: **[Int](../gravity/int.md)**
The format width is the number of characters of a formatted number within a string that is either left justified or right justified based on the value contained in paddingPosition.

* **var** **multiplier**: **[Int](../gravity/int.md)**
A multiplier is a factor used in conversions between numbers and strings (that is, numbers as stored and numbers as displayed). When the input value is a string, the multiplier is used to divide, and when the input value is a number, the multiplier is used to multiply. These operations allow the formatted values to be different from the values that a program manipulates internally.

* **var** **formattingContext**: **[Int](../gravity/int.md)**
The capitalization formatting context used when formatting a number.

* **var** **percentSymbol**: **[String](../gravity/string.md)**
The string used to represent a percent symbol. By default, this property is set to the percent sign (%).

* **var** **perMillSymbol**: **[String](../gravity/string.md)**
The string used to represent a per-mill (per-thousand) symbol. By default, this property is set to the per mille sign (‰).

* **var** **minusSign**: **[String](../gravity/string.md)**
The string used to represent a minus sign. By default, this property is set to the minus sign (-).

* **var** **plusSign**: **[String](../gravity/string.md)**
The string used to represent a plus sign. By default, this property is set to the plus sign (+).

* **var** **exponentSymbol**: **[String](../gravity/string.md)**
The string used to represent an exponent symbol. By default, this property is set to the latin capital letter e (E).

* **var** **zeroSymbol**: **[String](../gravity/string.md)**
The string used to represent a zero value. If not specified, zero values are formatted normally.

* **var** **nilSymbol**: **[String](../gravity/string.md)**
The string used to represent a null value. By default, this property is set to an empty string ("").

* **var** **notANumberSymbol**: **[String](../gravity/string.md)**
The string used to represent a NaN (“not a number”) value. By default, this property is set to the string "NaN".

* **var** **negativeInfinitySymbol**: **[String](../gravity/string.md)**
The string used to represent a negative infinity symbol. By default, this property is set to the string "-∞".

* **var** **positiveInfinitySymbol**: **[String](../gravity/string.md)**
The string used to represent a positive infinity symbol. By default, this property is set to the string "+∞".

* **var** **currencySymbol**: **[String](../gravity/string.md)**
The string used by the receiver as a local currency symbol. A country typically has a local currency symbol and an international currency symbol. The local symbol is used within the country, while the international currency symbol is used in international contexts to specify that country’s currency unambiguously. The local currency symbol is often represented by a Unicode code point.

* **var** **currencyCode**: **[String](../gravity/string.md)**
The receiver’s currency code. A currency code is a three-letter code that is, in most cases, composed of a country’s two-character Internet country code plus an extra character to denote the currency unit. For example, the currency code for the Australian dollar is “AUD”. Currency codes are based on the ISO 4217 standard.

* **var** **internationalCurrencySymbol**: **[String](../gravity/string.md)**
The international currency symbol used by the receiver. A country typically has a local currency symbol and an international currency symbol. The local symbol is used within the country, while the international currency symbol is used in international contexts to specify that country’s currency unambiguously. The international currency symbol is often represented by a Unicode code point.

* **var** **currencyGroupingSeparator**: **[String](../gravity/string.md)**
The currency grouping separator for the receiver.

* **var** **positivePrefix**: **[String](../gravity/string.md)**
The string the receiver uses as the prefix for positive values.

* **var** **positiveSuffix**: **[String](../gravity/string.md)**
The string the receiver uses as the suffix for positive values.

* **var** **negativePrefix**: **[String](../gravity/string.md)**
The string the receiver uses as a prefix for negative values.

* **var** **negativeSuffix**: **[String](../gravity/string.md)**
The string the receiver uses as a suffix for negative values.

* **var** **groupingSeparator**: **[String](../gravity/string.md)**
The string used by the receiver for a grouping separator. For example, the grouping separator used in the United States is the comma (10,000) whereas in France it is the space (10 000).

* **var** **usesGroupingSeparator**: **[Bool](../gravity/bool.md)**
Determines whether the receiver displays the group separator.

* **var** **thousandSeparator**: **[String](../gravity/string.md)**
The character the receiver uses as a thousand separator.

* **var** **hasThousandSeparators**: **[Bool](../gravity/bool.md)**
Determines whether the receiver uses thousand separators.

* **var** **decimalSeparator**: **[String](../gravity/string.md)**
The character the receiver uses as a decimal separator.

* **var** **alwaysShowsDecimalSeparator**: **[Bool](../gravity/bool.md)**
Determines whether the receiver always shows the decimal separator, even for integer numbers.

* **var** **currencyDecimalSeparator**: **[String](../gravity/string.md)**
The string used by the receiver as a currency decimal separator.

* **var** **groupingSize**: **[Int](../gravity/int.md)**
The grouping size of the receiver.

* **var** **secondaryGroupingSize**: **[Int](../gravity/int.md)**
The secondary grouping size of the receiver. Some locales allow the specification of another grouping size for larger numbers. For example, some locales may represent a number such as 61, 242, 378.46 (as in the United States) as 6,12,42,378.46. In this case, the secondary grouping size (covering the groups of digits furthest from the decimal point) is 2.

* **var** **paddingCharacter**: **[String](../gravity/string.md)**
The string that the receiver uses to pad numbers in the formatted string representation.

* **var** **paddingPosition**: **[Int](../gravity/int.md)**
The padding position used by the receiver.

* **var** **allowsFloats**: **[Bool](../gravity/bool.md)**
Determines whether the receiver allows as input floating-point values (that is, values that include the period character [.]). By default, floating point values are allowed.

* **var** **minimum**: **[Int](../gravity/int.md)**
The lowest number allowed as input by the receiver.

* **var** **maximum**: **[Int](../gravity/int.md)**
The highest number allowed as input by the receiver.

* **var** **lenient**: **[Bool](../gravity/bool.md)**
Determines whether the receiver will use heuristics to guess at the number which is intended by a string. If the formatter is set to be lenient, as with any guessing it may get the result number wrong (that is, a number other than that which was intended).

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **numberFromString**(**string**: **[String](../gravity/string.md)**): <strong>[Int](../gravity/int.md)</strong> 
Returns an Number object created by parsing a given string. If a string contains any characters other than numerical digits or locale-appropriate group or decimal separators, parsing will fail. Any leading or trailing space separator characters in a string are ignored.

* **func** **stringFromNumber**(**number**: **[Int](../gravity/int.md)**): <strong>[String](../gravity/string.md)</strong> 
Returns a string containing the formatted value of the provided number object.



* None

