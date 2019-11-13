If you don't have an Apple developer account or if you don't have any certificate, then you should first follow the tutorials from the excellent **[raywenderlich.com](https://raywenderlich.com)** website. Everything in part 1 and part 2 (except the Submit An App With Xcode paragraph) is valid and must be followed:
* **[How to Submit An App to Apple - Part 1](https://www.raywenderlich.com/184709/submit-app-apple-no-account-app-store-part-1)**
* **[How to Submit An App to Apple - Part 2](https://www.raywenderlich.com/184825/submit-app-apple-no-account-app-store-part-2)**
Once everything has been setup with Apple, you can press the Build Package button and start creating your app:
![Creo](../images/creo/creo_submit_your_app_1.png)
Please note that you should provide your Signing Identity and Provisioning Profile.

### Upload to the App Store

The result of the build is an ipa/app archive that you can submit to App Store using:
* **[Transporter](https://developer.apple.com/news/?id=10152019a)** from Apple (distributed on the **[Mac App Store](https://apps.apple.com/us/app/transporter/id1450874784?mt=12)**)
<!--* **[Application Loader](https://help.apple.com/itc/apploader/)** from Apple (distributed within the **[Xcode](https://developer.apple.com/xcode/) package**)-->
* **[Fastlane](https://docs.fastlane.tools/getting-started/ios/appstore-deployment/)** from Google
