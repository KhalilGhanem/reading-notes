# Android Fundamentals

Android apps can be written using:
* Kotlin 
* Java 
* C++

The Android SDK tools compile your code along with any data and resource files into an APK or an Android App Bundle.

* The Android package(.apk), contains the contents of an Android app that are required at runtime and it is the file that Android-powered devices use to install the app.

* The Android App Bundle(.aab), contains the contents of an Android app project including some additional metadata that is not required at runtime.

Each Android app lives in its own security sandbox, protected by the following Android security features:

* The Android operating system is a multi-user Linux system in which each app is a different user.
* By default, the system assigns each app a unique Linux user ID.
* Each process has its own virtual machine (VM).
* By default, every app runs in its own Linux process.

## App components
App components are the essential building blocks of an Android app. Each component is an entry point through which the system or a user can enter your app. Some components depend on others.

components Types:
* Activities: An activity is the entry point for interacting with the user. It represents a single screen with a user interface.
* Services : A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons.
* Broadcast receivers: A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.
* Content providers: A content provider manages a shared set of app data that you can store in the file system.

## The manifest file
The system must know that the component exists by reading the app's manifest file, `AndroidManifest.xml`. Your app must declare all its components in this file, which must be at the root of the app project directory.

**What the manifest file do**
1. Declaring components.
2. Identifies any user permissions the app requires.
3. Declares the minimum API Level required by the app.
4. Declares hardware and software features used or required by the app.
5. Declares API libraries the app needs to be linked against (other than the Android framework APIs).

