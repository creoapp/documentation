**super**: **[Object](../gravity/object.md)**

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **preferredLanguages**: **[List](../gravity/list.md)**
An ordered list of the user's preferred languages. Users choose a primary language when configuring a device. They may also specify one or more secondary languages in order of preference for use when localization is unavailable in a higher priority language. Use this property to obtain the current user's ordered list of languages, presented as an array of locale identifier strings. \(read-only\)



### Properties

* **var** **identifier**: **[String](../gravity/string.md)**
The identifier for the locale. Examples of locale identifiers include "en_GB", "es_ES_PREEURO", and "zh-Hant_HK_POSIX@collation=pinyin;currency=CNY". \(read-only\)

* **var** **countryCode**: **[String](../gravity/string.md)**
The country code for the locale. Examples of country codes include "GB", "FR", and "HK". \(read-only\)

* **var** **languageCode**: **[String](../gravity/string.md)**
The language code for the locale. Examples of language codes include "en", "es", and "zh". \(read-only\)

* **var** **scriptCode**: **[String](../gravity/string.md)**
The script code for the locale. Examples of script codes include "Latn" and "Hant". \(read-only\)

* **var** **variantCode**: **[String](../gravity/string.md)**
The variant code for the locale. Examples of variant code include "POSIX" and "PREEURO". \(read-only\)

* **var** **usesMetricSystem**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the locale uses the metric system. \(read-only\)

* **var** **decimalSeparator**: **[String](../gravity/string.md)**
The decimal separator for the locale. Example decimal separators include "." and ",". \(read-only\)

* **var** **groupingSeparator**: **[String](../gravity/string.md)**
TThe grouping separator for the locale. Example grouping separators include "," and " ". \(read-only\)

* **var** **currencyCode**: **[String](../gravity/string.md)**
The currency code for the locale. Example currency codes include "USD", "EUR", and "JPY". \(read-only\)

* **var** **currencySymbol**: **[String](../gravity/string.md)**
The currency symbol for the locale. Example currency symbols include "$", "€", and "¥". \(read-only\)

* **var** **calendarIdentifier**: **[String](../gravity/string.md)**
The calendar identifier for the locale. \(read-only\)

* **var** **currencySymbolIsBefore**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the currency symbol must be written before or after the amount value. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **system**()-> <strong>[Locale](Locale.md)</strong> 
The generic locale that contains fixed "backstop" settings that provide values for otherwise undefined keys.



### Constructors

* **func** **Locale**(**identifier**: **[String](../gravity/string.md)**)
Returns a locale using a given locale identifier.



### Methods

* **func** **stringForIdentifier**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified locale identifier.

* **func** **stringForCountryCode**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified country code. For example, calling this method on an American English (en_US) locale, passing "GB" for countryCode, produces the string "United Kingdom".

* **func** **stringForLanguageCode**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified language code. For example, calling this method on an American English (en_US) locale, passing "zh" for languageCode, produces the string "Chinese".

* **func** **stringForScriptCode**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified script code. For example, calling this method on an American English (en_US) locale, passing "Hant" for scriptCode, produces the string "Traditional Han".

* **func** **stringForVariantCode**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified variant code. For example, calling this method on an American English (en_US) locale, passing "POSIX" for variantCode, produces the string "Computer".

* **func** **stringForCurrencyCode**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified currency code. For example, calling this method on an American English (en_US) locale, passing "JPY" for currencyCode, produces the string "Japanese Yen".

* **func** **stringForCalendarIdentifier**(**string**: **[String](../gravity/string.md)**)-> <strong>[String](../gravity/string.md)</strong> 
Returns the localized string for the specified calendar identifier.





