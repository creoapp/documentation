**super**: **[Object](../gravity/object.md)**

Information about standard time conventions associated with a specific geopolitical region. Time zones represent the standard time policies for a geopolitical region. Time zones have identifiers like “America/Los_Angeles” and can also be identified by abbreviations, such as PST for Pacific Standard Time.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **local**: **[TimeZone](TimeZone.md)**
Current system time zone. \(read-only\)

* **var** **system**: **[TimeZone](TimeZone.md)**
The time zone currently used by the system. \(read-only\)

* **var** **default**: **[TimeZone](TimeZone.md)**
The default time zone for the current app. If no defaultTimeZone time zone has been set, the current system time zone is used. If the current system time zone cannot be determined, the GMT time zone is used instead. The defaultTimeZone time zone is used by the app for date and time operations. You can set it to cause the app to run as if it were in a different time zone. Setting the defaultTimeZone property clears any value that was previously set.



### Properties

* **var** **name**: **[String](../gravity/string.md)**
The geopolitical region ID that identifies the receiver.

* **var** **abbreviation**: **[String](../gravity/string.md)**
The abbreviation for the receiver, such as "EDT" (Eastern Daylight Time). \(read-only\)

* **var** **secondsFromGMT**: **[Int](../gravity/int.md)**
The current difference in seconds between the receiver and Greenwich Mean Time. \(read-only\)

* **var** **isDaylightSavingTime**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the receiver is currently using daylight saving time. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **reset**()
Clears any time zone value cached for the system property.



### Constructors

* **func** **TimeZone**(**identifier**: **[String](../gravity/string.md)**)
Returns the time zone object identified by a given name/abbreviation.





