Need help exporting CreoPlayer? [Click here](export_creoplayer.html) for more information.

Once you created an IPA executable using **Development Distribution** as Package Distribution option you can transfer it to your USB connected device using one of the following methods:
* **Xcode:** From the Window menu select "Devices and Simulators" then just drop your IPA file to the **Installed Apps** section.
![Creo](creo_transfer_app_2.png)
* **Apple Configurator 2: ** Download **[Apple Configurator 2](https://itunes.apple.com/us/app/apple-configurator-2/id1037126344?mt=12)** from MacOS App Store. Connect your iOS device to your Mac and then double click on the device icon. Select the Apps section and then drop your IPA file.
![Creo](creo_transfer_app_3.png)
* **ios-deploy:** It is an open source command line tool that can be installed from **[https://github.com/phonegap/ios-deploy](https://github.com/phonegap/ios-deploy)**. 
Once installed execute **ios-deploy -d -b myapp.ipa**