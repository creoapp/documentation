Starting from Creo version 2.2, CreoPlayer is no longer available through TestFlight and it can be exported directly from within Creo. In this way we can guarantee to release the most up-to-date version the same day we release a new Creo build.

Once exported with your **Development Distribution** provisioning profile you can install it [on your device](https://docs.creolabs.com/creo/transfer-to-device.html). 

Select **Export CreoPlayer** from the **File** menu and the fill-in the Bundle ID and Provisioning Profile fields. Please note that you must use a Bundle ID that belongs to your certificate in order to be able to export a correct build. 

![Export CreoPlayer](export_creoplayer_1.png)

**Do I need to purchase the Apple Developer $99/year membership to install CreoPlayer on my device?**

You don't need to purchase the Apple Developer $99/year membership to be able to transfer your own app to your own device. Note: Without enrolling in the Apple Developer Program, your app will only last for 7 days on your device. After that, you'll have to re-deploy it to your device via Xcode. More on [https://codewithchris.com/deploy-your-app-on-an-iphone/](https://codewithchris.com/deploy-your-app-on-an-iphone/)