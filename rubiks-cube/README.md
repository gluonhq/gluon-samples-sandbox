# Rubik's Cube

A JavaFX 3D Application that allows solving the Rubik's Cube on Desktop, Android and iOS devices.

## Documentation

Read about how the JavaFX 3D Rubik's cube was originally implemented [here](http://jperedadnr.blogspot.com.es/2014/04/rubikfx-solving-rubiks-cube-with-javafx.html)

## Quick Instructions

We use [GluonFX plugin](https://docs.gluonhq.com/) to build a native image for platforms including desktop, android and iOS.
Please follow the prerequisites as stated [here](https://docs.gluonhq.com/#_requirements).

### Desktop

Run the application using:

    mvn gluonfx:run

Build a native image using:

    mvn gluonfx:build

Run the native image app:

    mvn gluonfx:nativerun

### Android

Build a native image for Android using:

    mvn gluonfx:build -Pandroid

Package the native image as an 'apk' file:

    mvn gluonfx:package -Pandroid

Install it on a connected android device:

    mvn gluonfx:install -Pandroid

Run the installed app on a connected android device:

    mvn gluonfx:nativerun -Pandroid

### iOS

Build a native image for iOS using:

    mvn gluonfx:build -Pios

Install and run the native image on a connected iOS device:

    mvn gluonfx:nativerun -Pios

Create an IPA file (for submission to TestFlight or App Store):

    mvn gluonfx:package -Pios
