About
-----

Sample android/ios uber-like app developed as an exercise to learn [react-native](http://facebook.github.io/react-native/)/[firebase](https://firebase.google.com/).

**WARNING**: Currently the app is an early alpha stage, you should look at other samples for detailed react-native/firebase bits.

<p align="center">
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/login.png"            width="280" alt="login" />
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/signup.png"           width="280" alt="signup"/>
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/signup-completed.png" width="280" alt="signup completed"/>
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/loading.png"          width="280" alt="loading"/>
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/pickup.png"           width="280" alt="pickup"/>
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/destination.png"      width="280" alt="destination"/>
    <img src="https://raw.githubusercontent.com/javier-lopez/uber-react-native-firebase/master/screenshots/coords.png"           width="280" alt="data result"/>
</p>

Usage
-----

- Connect an Android device with developer mode enabled OR install Genymotion and install a Nexus 5 or 7 (Android version 5.1). If using Genymotion, disable its ADB by selecting Settings -> ABD -> Use custom Android SDK tools
- Install openssh and rsync using your operating system's package manager or installation tools

**If on Windows:**

1. Install Cygwin. Within the installer, choose the rsync and openssh packages as per https://github.com/mitchellh/vagrant/issues/3913#issuecomment-45761049. Install "git", under the "Devel" category, to allow cloning this repository. Install xorg-server and xinit to allow launching Chrome for debugging.
2. If Vagrant/rsync [issue](https://github.com/mitchellh/vagrant/issues/6702) is not yet resolved, you will need to follow the instructions under https://github.com/mitchellh/vagrant/issues/6702#issuecomment-166503021
3. Launch a terminal using the "Cygwin terminal" shortcut on your desktop or Start Menu.
4. Run "startxwin" to launch a local X server for Chrome.

**If on OS X:**

1. Install XQuartz to enable viewing the developer console in Chrome within the VM.
2. Clone this repository and change to the new folder.

**If using an android device**

    vagrant up

**If using an emulator (replace IP address with your emulator's IP):**

    ADB_EMULATOR_IP_ADDRESS=192.168.56.101 vagrant up

To enable live reloading use the "shake" gesture or press Ctrl-m in Genymotion and select "Enable Live Reload". Changes made to the code should automatically update on the device. To use the Chrome developer tools for debugging, start Chrome and connect to http://localhost:8081/debugger-ui and follow the instructions to install developer tools.

Login to the virtual environment and follow the instructions to get started.

    vagrant ssh
