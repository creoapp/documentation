### Examples
#### Log Device information:
```
Device.batteryMonitoringEnabled = true;

var string = "Device Version Name: " +  Device.deviceVersionName;
string += "\nDevice Version Code: " + Device.deviceVersion;
string += "\nDevice Size: " + 
Device.deviceSizeName(Device.deviceSize);
string += "\nSystem Version: " + Device.systemVersion;
string += "\nSystem Name: " + Device.systemName;
string += "\nDevice Name: " + Device.name;
string += "\nDevice Model: " + Device.model;
string += "\nBattery: Enabled=" + Device.batteryMonitoringEnabled + ", State=" + Device.batteryState + ", Charge=" + Int(Device.batteryLevel*100) + "%";

Console.write(string);
```
Result:
```
Device Version Name: iPhone 5S
Device Version Code: 7
Device Size: 4.0 in
System Version: 8.0.0
System Name: iOS
Device Name: Xinantécatl
Device Model: iPhone
Battery: Enabled=true, State=3, Charge=100%
```