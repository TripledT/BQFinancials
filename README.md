## Prerequisites
#### Required tools and dependencies:
* [Node.js](https://nodejs.org)
    - Download and run the Node installation package.

    
#### For running and building in iOS:
* [Xcode](https://itunes.apple.com/us/app/xcode/id497799835)
    - Protip: Xcode takes quite a while to install from the App Store. This step should actually be the first thing you do if you know you will be developing and building in iOS.
#### For running and building in Android:
* [Homebrew](https://brew.sh/)
    - Run this in terminal: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
* [Android Studio](https://developer.android.com/studio/index.html)
    - Follow the [Getting Started](https://facebook.github.io/react-native/docs/getting-started.html) guide for Android.
    - Select Development OS, then Android from the page.
    - Install the dependencies in which you have not yet installed (e.g. you can skip `brew install node` and `npm install -g react-native-cli` at this point).
    - Follow the remaining instructions Android Studio installation instructions. Skip the "Creating a new application" section.
    - Note: you only need to use Android Studio to open AVD Manager:
        - When you first open Android Studio, it will ask you whether to open an existing project or create a new one. Choose create new project.
        - Then click the AVD Manager icon on the top right of the toolbar. Alternatively you may go to Tools -> Android -> AVD Manager.
        - Click Create Virtual Device...
        - Follow and complete the process by selecting a phone and choosing your downloaded Android version.
        - At this point you may continue to start the Android emulator by always going through Android Studio -> AVD Manager -> Start emulator... or...
        - Ditch Android Studio and just run from terminal:
            - `/Users/<user>/Library/Android/sdk/emulator/./emulator -list-avds` to list your emulator names.
            - `/Users/<user>/Library/Android/sdk/emulator/./emulator -avd <avd_name>` to run from terminal from this point onwards.


## Starting The Application
* `npm install` if running for the first time.
* For iOS:
    - `npm run start-ios`.
* For Android:
    - Manually start Android emulator.
        - Protip: after you've installed Android Studio and have your Android virtual device created, you will no longer need to start Android Studio in order to run your virtual device. Just start your Android emulator straight from [command line](https://developer.android.com/studio/run/emulator-commandline.html) (e.g. `/Users/<user>/Library/Android/sdk/emulator/./emulator -avd <avd_name>
`).
    - `npm run start-android`.
        - If upon starting, you receive an unable to locate Android SDK error message, follow the instructions of either creating a local.properties file or setting an ANDROID_HOME environment variable.