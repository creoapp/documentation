**super**: **[Object](../gravity/object.md)**

You use the Authenticator class to evaluate the user’s identity, either with biometrics like Touch ID or Face ID, or by supplying the device passcode. The context handles user interaction, and also interfaces to the Secure Enclave, the underlying hardware element that manages biometric data. You create and configure the context, and ask it to carry out the authentication. You then receive an asynchronous callback, which provides an indication of authentication success or failure, and an error instance that explains the reason for a failure, if any.

The Authenticator class can be simulated in the Apple iOS Simulator or in CreoPlayer (not in the built-in Creo Simulator).

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Methods

* **func** **authenticateWithBiometrics**(**message**: **[String](../gravity/string.md)**, **closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (result: Bool, error: String)" data-content="The completion closure to execute when authentication completes. If result is false then error String contains the failure reason.">Closure</a>**)
This method asynchronously evaluates an authentication policy. Evaluating a policy may involve prompting the user for various kinds of interaction or authentication. The actual behavior is dependent on the evaluated policy and the device type. The behavior can also be affected by installed configuration profiles.
In the localized string you present to the user in the authentication dialog, provide a clear reason for the authentication request, and describe the resulting action. Make the message short and clear, and provide it in the user’s language. Don’t include the app name, which already appears in the authentication dialog (in macOS, in the title of the dialog; in iOS, in the subtitle).
Don’t assume that a previous successful policy evaluation means that future evaluations will also succeed. Policy evaluation can fail for various reasons, including cancellation by the user or the system.

* **func** **authenticateWithBiometricsOrPasscode**(**message**: **[String](../gravity/string.md)**, **closure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="closure (result: Bool, error: String)" data-content="The completion closure to execute when authentication completes. If result is false then error String contains the failure reason.">Closure</a>**)
This method asynchronously evaluates an authentication policy. Evaluating a policy may involve prompting the user for various kinds of interaction or authentication. The actual behavior is dependent on the evaluated policy and the device type. The behavior can also be affected by installed configuration profiles.
In the localized string you present to the user in the authentication dialog, provide a clear reason for the authentication request, and describe the resulting action. Make the message short and clear, and provide it in the user’s language. Don’t include the app name, which already appears in the authentication dialog (in macOS, in the title of the dialog; in iOS, in the subtitle).
Don’t assume that a previous successful policy evaluation means that future evaluations will also succeed. Policy evaluation can fail for various reasons, including cancellation by the user or the system.





