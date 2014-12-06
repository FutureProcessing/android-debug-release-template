Android Debug Release Template
===============================

## Overview

This is a template Android project, which shows, how to build a single app with a different configurations for debug and release build type.
In addition, this template allows to install debug and release version of the same app on one device or emulator, which is not possible with default project configuration.

## Description

During software development process developers and QAs may want to have installed release and debug version of the app on a single device,
what can be very helpful when they want to develop and use application at the same time.
Another advantage is the fact that debug and release version of the app may need different configuration.
It this example, we are changing application name and launcher icon,
but we can also change different values during compilation in the same way (e.g. address of the webservice).
This template also generates versionName of the application, which contains SHA hash of the last commit, build date and time.
For debug version it adds -DEBUG suffix to the versionName. Installing two the same applications in different build variants on the same device is possible,
because applicationIdSuffix for debug version of the app is added during the compilation, what changes package name for this build variant.
As a result, release version of the app has package name "fp.com.debugreleasetemplate" and debug version of the app has package name "fp.com.debugreleasetemplate.debug".

## Important files with build configurations

- [build.gradle](https://github.com/FutureProcessing/android-debug-release-template/blob/master/build.gradle)
- [app/build.gradle](https://github.com/FutureProcessing/android-debug-release-template/blob/master/app/build.gradle)

## Additional information

Please note that Android Studio, Android SDK, Build Tools and Gradle are evolving very quickly and their future updates may cause compilation errors of this template.
This project was created with Android Studio 1.0 RC 4.
