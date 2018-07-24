**super**: **[Object](Object.md)**

Date objects encapsulate a single point in time, independent of any particular calendrical system or time zone. The Date class provides methods for comparing dates, calculating the time interval between two dates, and creating a new date from a time interval relative to another date.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **timeIntervalSinceNow**: **[Float](../gravity/types.md)**
The interval between the date object and the current date and time. \(read-only\)

* **var** **timeIntervalSince1970**: **[Float](../gravity/types.md)**
The interval between the date object and 00:00:00 UTC on 1 January 1970. \(read-only\)

* **var** **era**: **[Int](../gravity/types.md)**
Extract era from current date. \(read-only\)

* **var** **year**: **[Int](../gravity/types.md)**
Extract year from current date. \(read-only\)

* **var** **month**: **[Int](../gravity/types.md)**
Extract month from current date. \(read-only\)

* **var** **day**: **[Int](../gravity/types.md)**
Extract day from current date. \(read-only\)

* **var** **hour**: **[Int](../gravity/types.md)**
Extract hour from current date. \(read-only\)

* **var** **minute**: **[Int](../gravity/types.md)**
Extract minute from current date. \(read-only\)

* **var** **second**: **[Int](../gravity/types.md)**
Extract second from current date. \(read-only\)

* **var** **nanosecond**: **[Int](../gravity/types.md)**
Extract nanosecond from current date. \(read-only\)

* **var** **weekday**: **[Int](../gravity/types.md)**
Extract weekday from current date. The weekday units are the numbers 1 through N (where for the Gregorian calendar N=7 and 1 is Sunday). \(read-only\)

* **var** **weekdayOrdinal**: **[Int](../gravity/types.md)**
The weekday ordinal unit describes ordinal position within the month unit of the corresponding weekday unit. For example, in the Gregorian calendar a weekday ordinal unit of 2 for a weekday unit 3 indicates "the second Tuesday in the month". \(read-only\)

* **var** **quarter**: **[Int](../gravity/types.md)**
Extract quarter from current date. \(read-only\)

* **var** **weekOfMonth**: **[Int](../gravity/types.md)**
Extract the original week of a month calendar unit. \(read-only\)

* **var** **weekOfYear**: **[Int](../gravity/types.md)**
Extract the original week of the year calendar unit. \(read-only\)

* **var** **yearForWeekOfYear**: **[Int](../gravity/types.md)**
Extract the ISO Week Date from current date. \(read-only\)



### Class Methods

* **func** **dateWithTimeIntervalSince1970**(**timeInterval**: **[Float](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set to a given number of seconds from 00:00:00 UTC on 1 January 1970.

* **func** **dateWithTimeIntervalSinceReferenceDate**(**timeInterval**: **[Float](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set to a given number of seconds from 00:00:00 UTC on 1 January 2001.

* **func** **knownTimeZoneNames**(): <strong>[List](../gravity/lists.md)</strong> 
Returns an array of strings listing the names of all the time zones known to the system.

* **func** **tomorrow**(): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set to tomorrow.

* **func** **yesterday**(): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set to yesterday.

* **func** **dateWithDaysFromNow**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set by adding reference days to the current date and time.

* **func** **dateWithDaysBeforeNow**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set by subtracting reference days to the current date and time.

* **func** **dateWithHoursFromNow**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set by adding reference hours to the current date and time.

* **func** **dateWithHoursBeforeNow**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set by subtracting reference hours to the current date and time.

* **func** **dateWithMinutesFromNow**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set by adding reference minutes to the current date and time.

* **func** **dateWithMinutesBeforeNow**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a Date object set by subtracting reference minutes to the current date and time.



### Initializers

* **func** **Date**(**timeInterval**: **[Float](../gravity/types.md)**)
Returns a Date object relative to the current date and time by a given number of seconds.

* **func** **Date**(**timeInterval**: **[Float](../gravity/types.md)**, **date**: **[Date](date.md)**)
Returns a Date object relative to another given date by a given number of seconds.

* **func** **Date**(**string**: **[String](../gravity/types.md)**, **format**: **[String](../gravity/types.md)**, **timeZone**: **[String](../gravity/types.md)**)
Returns a Date object converted from a textual representations of dates and times.



### Methods

* **func** **isEqualToDate**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object is exactly equal to a reference date.

* **func** **diff**(**refDate**: **[Date](date.md)**): <strong>[Float](../gravity/types.md)</strong> 
Returns the interval between the receiver and the reference Date parameter. If the receiver is earlier than reference Date, the return value is negative.

* **func** **isEqualToDateIgnoringTime**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object is equal to a reference Date ignoring the time value.

* **func** **isToday**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to today.

* **func** **isTomorrow**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to tomorrow.

* **func** **isYesterday**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to yesterday.

* **func** **isSameWeekAsDate**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object has the same week as a reference Date.

* **func** **isThisWeek**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to current week.

* **func** **isNextWeek**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to next week.

* **func** **isLastWeek**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to last week.

* **func** **isSameMonthAsDate**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object has the same month than a reference Date.

* **func** **isThisMonth**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to current month.

* **func** **isNextMonth**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to next month.

* **func** **isLastMonth**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to last month.

* **func** **isSameYearAsDate**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object has the same year as a reference Date.

* **func** **isThisYear**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to current year.

* **func** **isNextYear**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to next year.

* **func** **isLastYear**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to last year.

* **func** **isEarlierThanDate**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object is earlier than a reference Date.

* **func** **isLaterThanDate**(**refDate**: **[Date](date.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date object is later thana reference Date.

* **func** **isInFuture**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to sometime in the future.

* **func** **isInPast**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether a given Date is set to sometime in the past.

* **func** **dateByAddingYears**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by adding reference years to the current date.

* **func** **dateBySubtractingYears**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by subtracting reference years to the current date.

* **func** **dateByAddingMonths**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by adding reference months to the current date.

* **func** **dateBySubtractingMonths**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by subtracting reference months to the current date.

* **func** **dateByAddingDays**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by adding reference days to the current date.

* **func** **dateBySubtractingDays**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by subtracting reference days to the current date.

* **func** **dateByAddingHours**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by adding reference hours to the current date.

* **func** **dateBySubtractingHours**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by subtracting reference hours to the current date.

* **func** **dateByAddingMinutes**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by adding reference minutes to the current date.

* **func** **dateBySubtractingMinutes**(**reference**: **[Int](../gravity/types.md)**): <strong>[Date](date.md)</strong> 
Creates and returns a new Date object set by subtracting reference minutes to the current date.

* **func** **format**(**format**: **[String](../gravity/types.md)**, **timeZone**: **[String](../gravity/types.md) = null**): <strong>[String](../gravity/types.md)</strong> 
Returns a textual representations of the Date. Parameters: <code>format</code> is the date format string (use the <a href="http://www.unicode.org/reports/tr35/tr35-19.html#Date_Format_Patterns">Unicode Date Format Patterns</a>, for example "yyyy-MM-dd HH:mm:ss"), <code>timezone</code> is the name (for example "America/Los_Angeles", see the <code>knownTimeZoneNames</code> class method for more infomation) or the abbreviation (for example "PDT") of the time zone to be used. If unspecified or invalid, the system time zone is used.





