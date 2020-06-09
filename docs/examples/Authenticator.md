# 

```
func closure (result:Bool, error:String) {
    if (result) {
		Console.write("Authentication OK");
	} else {
		Console.write("Authentication failed: \(error)")
	}
}

Authenticator.authenticateWithBiometrics("Please Authenticate", closure)
```
