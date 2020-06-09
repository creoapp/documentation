**super**: **[Object](../gravity/object.md)**

The AppStore module provides support for in-app purchases and interactions with the App Store. In-app purchases capabilities can be tested on Apple iOS Simulator (with some limitations) but we recommed to test it with a debug build on a real device.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **ProductRequested**(**result**: **[Bool](../gravity/bool.md)**, **product**: **[Map](../gravity/map.md)**)
Event raised when a product request information is processed by the App Store. Your app uses this information when presenting products to users in its in-app store.

* **TransactionUpdated**(**status**: **<a href="#_enum_PaymentTransactionState">PaymentTransactionState</a>**, **transaction**: **[Map](../gravity/map.md)**)
Event raised when a payment transaction is updated, created or deleted. The code in this event should be responsible to handle payments and enable/disable features based on payments. **This event is mandatory and must be implemented.**

* **ReceiptRefreshed**(**result**: **[Bool](../gravity/bool.md)**, **error**: **[String](../gravity/string.md)**)
Event raised when a receipt refresh action is requested to the App Store.

* **ReceiptValidated**(**result**: **[Bool](../gravity/bool.md)**, **transaction**: **[Map](../gravity/map.md)**, **error**: **[String](../gravity/string.md)**)
Event raised when a receipt validation is requested by your app. This is not a recommended method to validate a receipt, the method and the corresponding event are here for developer's convenience but you should follow Apple's guidelines and implement your receipt validation server side code.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **validationReceiptEndpoint**: **[String](../gravity/string.md)**
The URL for verifying receipts.

* **var** **forceUseProductionVerifyEndpoint**: **[Bool](../gravity/bool.md)**
Force to use real production ready URL endpoint for receipt validation.



### Class Methods

* **func** **requestReview**()<strong>: [Bool](../gravity/bool.md)</strong> 
Ask the user to rate or review your app, if appropriate. Although you should call this method when it makes sense in the user experience flow of your app, the actual display of a rating/review request view is governed by App Store policy. Because this method may or may not present an alert, it's not appropriate to call it in response to a button tap or other user action.

* **func** **canMakePayments**()<strong>: [Bool](../gravity/bool.md)</strong> 
Indicates whether the user is allowed to make payments. An iPhone/iPad can be restricted from accessing the Apple App Store. For example, parents can restrict their children’s ability to purchase additional content. Your application should confirm that the user is allowed to authorize payments before adding a payment to the queue. Your application may also want to alter its behavior or appearance when the user is not allowed to authorize payments.

* **func** **receipt**()<strong>: [String](../gravity/string.md)</strong> 
Returns a Base64 encoded receipt data. If an App Store receipt cannot be found then null is returned.

* **func** **receiptPath**()<strong>: [String](../gravity/string.md)</strong> 
Returns the file path for the bundle's App Store receipt. For an application purchased from the App Store, use this method to locate the receipt. It makes no guarantee about whether there is a file at the path. Only that if a receipt is present, that is its location.



### Methods

* **func** **addProductID**(**productID**: **[String](../gravity/string.md)**)
Add product identifier to the list of products you wish to retrieve descriptions of.

* **func** **requestProductsInfo**(**closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (result: Bool, product: Map)" data-content="The completion closure, if set, is executed when the App Store returns information about requested products. If productID is not valid the result if false and product contains only the id field. If productID is valid, true is set as result and the product parameter contains all the details.">Closure</a> = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
Retrieve localized information from the App Store about a specified list of products (products are specified via the addProductID method). If device cannot make payments or if the list of products is not set then false is returned. **This method is mandatory and must be called before initiating a purchase.**

* **func** **validateReceipt**(**sharedSecret**: **[String](../gravity/string.md) = null**, **closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (result: Bool, details: Map, error: String)" data-content="The completion closure, if set, is executed when the App Store receipt validation completes. If result is true then the details parameter contains all the details about the receipt, otherwise if result is false the error parameter contains details about the error.">Closure</a> = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
An App Store receipt provides a record of the sale of an app or any purchase made from within the app. You can authenticate purchased content by adding receipt validation code to your app or server. Receipt validation requires an understanding of secure coding techniques in order to employ a solution that is secure and unique to your application.

Do not call the App Store server validateReceipt endpoint from your app. You can't build a trusted connection between a user’s device and the App Store directly, because you don’t control either end of that connection, which makes it susceptible to a man-in-the-middle attack.

* **func** **purchaseProductID**(**productID**: **[String](../gravity/string.md)**, **quantity**: **[Int](../gravity/int.md) = 1**, **closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (status: Bool, transaction: Map)" data-content="The completion closure, if set, is executed when the App Store purchases completes. The status parameter contains the current state of the transaction. The product parameter contains all the details about the transaction.">Closure</a> = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
Submit your payment request to the App Store by initiating a purchase operation for the specified productID. If productID is not found (or if the requestProductsInfo was not called) then it immediately returns false. For every payment request your app submits, it receives a corresponding transaction to process (via the closure parameter and via the TransactionUpdated event.

* **func** **restorePurchases**(**closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (status: Bool, transaction: Map)" data-content="The completion closure, if set, is executed when the App Store purchases completes. The status parameter contains the current state of the transaction. The product parameter contains all the details about the transaction.">Closure</a> = null**)
Users sometimes need to restore previously purchased content, such as when they upgrade to a new phone (or when they delete and re-install the app). Include some mechanism in your app, such as a Restore Purchases button, to let them restore their purchases. Apple may reject an app if it cannot restore non-consumable purchases.

* **func** **refreshReceipt**(**closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (result: Bool, error: String)" data-content="The completion closure, if set, is executed when the App Store restore purchases completes. If result is false the error parameter contains details about the error.">Closure</a> = null**)
 Asks the App Store for the latest copy of the receipt. Refreshing a receipt does not create any new transactions. The refreshed receipt contains a record of the user’s purchases in this app, on this device or any other device.





### Enums

<div id="_enum_PaymentTransactionState"></div>

#### PaymentTransactionState
 * .Deferred
 * .Failed
 * .Purchased
 * .Purchasing
 * .Restored



