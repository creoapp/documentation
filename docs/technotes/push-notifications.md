**Preliminary documentation**


**Prepare your application**

- Go to the inspector for the App object, section Push Notifications
  - Check the Enable flag.
  - Choose the Options:
    - badge: Display a number on the corner of the app’s icon.
    - sound: Play a sound.
    - alert: Display text.
    - carPlay: Display notifications in CarPlay.
    - provisional: Post non-interrupting notifications. The user won’t get a request for permission if you only use this option, but your notifications will only show silently in the Notification Center.
    - Announcement: The setting that indicates whether Siri can announce your app’s notifications.
    - criticalAlert: Ignore the mute switch and Do Not Disturb. You’ll need a special entitlement from Apple to use this option as it’s only meant to be used when absolutely necessary.
  - Set a Bundle ID for your App.

**Identifiers, Profiles & Keys on developer.apple.com**

- Sign in -> account -> Certificates, Identifiers & Profiles
  - Identifiers: Create a new Identifiers with the explicit Bundle ID of your App and enable the “Push Notifications” Capability.
  - Profiles: Create a new Provisioning Profile with the App ID created in the previous step and set desired Certificates and Devices.
  - Keys: Create a new key with the Apple Push Notifications service (APNs) enabled (if you don’t  already have one). Download the key (.p8 file, it will be needed to send notification through a public service, APNs API or an app used for testing push notifications (for example, https://github.com/onmyway133/PushNotifications).

**Add custom code to App Events**

- DidRegisterForPushNotification: get the token, send it to your app server.
- WillPresentNotification:
- DidReceiveNotification:

**Test your App**

- iOS Simulator: 
  
  - run the app from Creo in a iOS Simulator.
  - use xcrun from Terminal: 
    - command: xcrun simctl push booted <bundle_id> <payload.json>
    - <bundle_id>: the Bundle ID of your App.
    - <payload.json>: the content of the test notification, see the Paylod examples section.

- iOS Device:
  
  - App:
    - Build your App for “Development Distribution” with the Provisioning Profile created in the Identifiers, Profiles & Keys section.
    - Install the App (.ipa) in your device.
    - Launch the App, grant the authorization for the configured notifications and copy the token returned by the DidRegisterForPushNotification event.
  - Push Notifications Utility:
    - Install and launch the PushNotifications utility: https://github.com/onmyway133/PushNotifications
    - Under Authentication, select Token.
    - Click the Select P8 button and select the .p8 (key).
    - Enter your Key ID and Team ID in the relevant fields.
    - Under Body, enter your Bundle ID and the token provided by the App (DidRegisterForPushNotification)
    - Enter a sample payload in the message field (see the following Payload examples section)


Payload examples:
```
alert notification:
{
  "aps": {
    "alert": “Test”,
    "sound": "default",
    "link_url": "https://creolabs.com”,
    "category": “TEST”
  }
}
silent notification:
{
  "aps": {
    "content-available": 1
  }
}
```

**Project**
* [PushNotification.creoproject]({{github_raw_link}}/assets/push-notification.zip) (12KB)

**Useful links**
* [https://medium.com/better-programming/how-to-test-push-notifications-on-the-ios-simulator-9b5062519622](https://medium.com/better-programming/how-to-test-push-notifications-on-the-ios-simulator-9b5062519622)
