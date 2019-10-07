Starting from Creo version 2.2, CreoPlayer is no longer available through TestFlight but it can be exported directly from within Creo. In this way, we can guarantee to release the most up-to-date version the same day we release a new Creo build.

Once exported with your **Development Distribution** provisioning profile you can install it [on your device](https://docs.creolabs.com/creo/transfer-to-device.html).

Select **Export CreoPlayer** from the **File** menu and the fill-in the Bundle ID and Provisioning Profile fields. Please note that you must use a Bundle ID that belongs to your certificate to be able to export a correct build.

![Export CreoPlayer](export_creoplayer_1.png)

### Apple Developer Program - Certificates, Identifiers & Profiles

In the [Apple Developer Center](https://developer.apple.com/account/) you can manage the certificates, identifiers, profiles, and devices you need to develop and distribute apps. If not yet registered, enroll for the [Apple Developer Program](https://developer.apple.com/programs/) \(\*\).

### Signing Identity

The Signing Identity consists of a public-private key pair that Apple creates for you. You need a **Development** Signing Identity (Apple Development or iOS Development) to export the CreoPlayer.
If you don't have a **Development** Signing Identity, create one with the following instructions:
    * [Create a Certificate Signing Request](https://help.apple.com/developer-account/#/devbfa00fef7) (CSR) through the Keychain Access Application. Keychain Application will create a private key (private key will be stored in the keychain) and a certSigningRequest file which you’ll then upload to Apple.
    * Create a new certificate on the Apple Developer website, choose the `Apple Development` type and upload the certSigningRequest file. Apple will proof the request and issue a certificate for you. The Certificate will contain the public key that can be downloaded to your system.
    * Downloaded it and put it into your Keychain Access Application by double-clicking it. The Certificate will be pushed into the Keychain and paired with the private key to form the Code Signing Identity.

### Bundle ID

A bundle ID or bundle identifier uniquely identifies an application in Apple's ecosystem. This means that no two applications can have the same bundle identifier. To avoid conflicts, Apple encourages developers to use reverse domain name notation for choosing an application's bundle identifier. For example, `com.yourdomain.creoplayer`.

### Provisioning Profile

 A Provisioning profile act as a link between the device and the developer account. During development, you choose which devices can run your app and which app services your app can access. A provisioning profile is downloaded from your developer account and embedded in the app bundle, and the entire bundle is code-signed. A Development Provisioning Profile must be installed on each device on which you wish to run your application code. If the information in the provisioning profile doesn’t match certain criteria, the app won’t launch.
 Each Development Provisioning Profile will contain:
* Development Certificates — development certificate. These are for developers who want to test the app on a physical device while writing code: set your Development Signing Identity
* Devices: select the list of devices that the app can run on, you can add missing devices in the **Devices** section.
* an App ID (this can include a * wild card to be used for many applications with similar bundle identifiers). — An App ID is a two-part string used to identify one or more apps from a single development team. For the CreoPlayer, you need an App ID that matches the Bundle ID used in the **Export CreoPlayer** panel. You can add an App ID from the **Identifiers** section using the following parameters:
    * Platform: iOS,tvOS,watchOS
    * Description: a name to identify this App ID
    * Bundle ID: choose the `Wildcard` option and write the `*` char in the text field. At the moment the CreoPlayer doesn't need any Capability so the Wildcard Bundle ID works file. An explicit Bundle ID will be required if some capabilities will be needed in the future.

### System Requirements

The **Export CreoPlayer** uses the **Xcode Command Line Tools** to export the CreoPlayer App.
Use `xcode-select -p` in the Terminal to check the current location of the command line tools. 
If missing or wrong, use `xcode-select --install` to install the standalone command line developer tools (without Xcode) or use `sudo xcode-select --switch <path/to/Xcode.app>` to specify the Xcode that you wish to use for command line developer tools.

<br/>
**\(\*\) Do I need to purchase the Apple Developer $99/year membership to install CreoPlayer on my device?**

You don't need to purchase the Apple Developer $99/year membership to be able to transfer your own app to your own device. Note: Without enrolling in the Apple Developer Program, your app will only last for 7 days on your device. After that, you'll have to re-deploy it to your device via Xcode. More on [https://codewithchris.com/deploy-your-app-on-an-iphone/](https://codewithchris.com/deploy-your-app-on-an-iphone/)
