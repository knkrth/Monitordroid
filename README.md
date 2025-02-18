Monitordroid (Mobile Application)
-----------------------------------
Developer: Tyler Butler (tyler@monitordroid.com)

Don't want to go through the stress of setting up your own server? Go to https://monitordroid.com and let us do the work for you! 10-day free trial avaliable.

Instructions:

1. If you haven't yet, first set up your Monitordroid open-source web server following the instructions in the README.md in the Monitordroid-Web-Application repository. 

2. Import the Monitordroid project into an IDE suited for Android development such as Android Studio or Eclipse. 

3. It is normal to initially have errors in each line of code that references the Google Play Services library. To resolve these errors, you must link the project with the Google Play Services library. You must first download the most recent version of the Google Play Services SDK from the Android SDK Manager. A tutorial on downloading SDKs can be found here: https://developer.android.com/sdk/installing/adding-packages.html and a tutorial on linking the Google Play Services library to a project once the SDK has been installed can be found here: https://developers.google.com/android/guides/setup#Install

4. Navigate to the 'src/com/monitordroid/app' path and open the CommonUtilities.java file in an editor. Set the 'DOMAIN' variable on line 40 to point to the link of your active Monitordroid web server. This can be a domain or an IP address. If you are using a LAN IP address, you will not be able to use Monitordroid if your device leaves your local network. To solve this, you can forward port 80 from your router to the local machine on your network running your web server and use your router's public IP address in this field. 

5. Set the 'SENDER_ID' variable on line 44 to the Sender ID you retrieved from step 2 of the instructions for the           Monitordroid-Web-Application

6. Export an APK and install it onto your Android devices.  

7. When Monitordroid is run on the device, enter a name for the device under the "Unique Device Name" field. Enter 'admin' under the 'Account Email' field and then click register. If your setup has been successful, you should receive a confirmation message on your device that it has been registed to your web server. On your web browser logged into the Monitordroid web application, refresh the page and you should see your new device and be able to issue it commands. 

Unfortunately we cannot offer support on our open-source version, but if you believe there is an error in the code or these instructions please let us know by sending us an email at help@monitordroid.com

-Monitordroid Team
