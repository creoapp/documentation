#### How to start monitoring network availability:
```
// networkReachability instance must be saved somewhere
// (for example in a class property) otherwise it will be
// automatically deallocated
var networkReachability = NetworkReachability()
// or networkReachability = NetworkReachability("www.google.com")

func onStatusChange(networkReachability,status) {
		Console.write("NetworkReachability status changed \(status)")
		Console.write(networkReachability.statusString);
		Console.write("reachable: \(reachable)");
		Console.write("WWAN: \(networkReachability.reachableViaWWAN)");
		Console.write("WiFi: \(networkReachability.reachableViaWiFi)");
	}
	
networkReachability.setOnStatusChange(onStatusChange)
networkReachability.start();
```

