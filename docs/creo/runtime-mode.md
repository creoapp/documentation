Much of the time **Creo** will show runtime data directly into the Design Board without requiring any further interaction from your side. In case you want to force runtime mode, **Creo** offers you several possibilities.


#### Executing your app inside CreoKit simulator
Most of the tools out there use a web view to emulate the mobile operating system while others force you to install Xcode and then use Apple iOS Simulator to execute iOS code launched as a separate process. CreoKit is an ObjC/Swift native framework that enables us to execute any iOS code on Mac. That means that everything you see on your screen is not emulated in any way but it is real iOS code.


In order to start executing your app inside CreoKit just press the Play button on the toolbar.
![Creo](../images/creo/runtime-mode-2.png)

Once pressed a new CreoKit instance will be created and all your runtime code will be executed immediately (the Design Board is effectively another CreoKit instance, that’s the reason why you can see real time data while you are in design mode). Simulator size and orientation will automatically reflect device type and orientation currently selected into the Design Board.


#### Switching between design mode and runtime mode
When you drop a control into the Design Board you can resize it because you are in Design Mode, if you want to really interact with it you need to enter the Runtime Mode just pressing key combination ALT + CMD:
![Creo](../images/creo/runtime-mode.png)
