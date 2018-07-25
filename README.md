
##arcore HL
1. Set up your development environment
* Install Android Studio version 3.1 or higher with Android SDK Platform version 7.0 (API level 24) or higher.
2. Open the sample project
* Get the sample projects
  > git clone https://github.com/google-ar/arcore-android-sdk.git<br>
  > git clone https://github.com/google-ar/sceneform-android-sdk.git

In Android Studio, open the hellosceneform sample project in <sceneform samples folder>/hellosceneform.

This project uses Sceneform, a 3D framework for that makes it easy for Java developers to build ARCore apps without Open GL.

All sample projects have build dependencies on certain versions of software, such as Gradle and the Android SDK. If the required dependencies are not installed, Android Studio will ask you for permission to download and install them on your machine.

Prepare your device or emulator
You can run AR apps on a supported device or emulator.

There are additional requirements to run Sceneform apps in the emulator:

You need Android Emulator version 27.2.9 or later.
OpenGL ES 3.1 must be supported and enabled in the Android Emulator.

Make sure your emulator is configured to use the latest version. In the menu, select Settings > Advanced > Renderer maximum (up to OpenGL ES 3.1).

Run the emulator and check whether OpenGL ES 3.1 is being used:

adb logcat | grep eglMakeCurrent
If you see ver 3 1, then you can run Sceneform apps. If you see a lower version, then your desktop GPU does not support OpenGL ES 3.1 and you must use a supported device to run Sceneform apps.

Run the sample
Make sure your Android device is connected to the development machine and click Run  in Android Studio. Then, choose your device as the deployment target and click OK.



Android Studio builds your project into a debuggable APK, installs the APK, and then runs the app on your device. For more information, see Build and Run Your App.

You may be prompted to install or update the ARCore app if it is missing or out of date. Select CONTINUE to install it from Google Play Store.

The hellosceneform app lets you place and manipulate Android figurines on flat surfaces.

Next steps
Try building and running other sample projects in the ARCore SDK and Sceneform samples.
Learn how to Enable ARCore in your app.
Use Augmented Images to build apps that can respond to 2D images, such as posters or logos, in the user's environment.
Use Cloud Anchors to create AR experiences that Android and iOS users can share.
