# Xcode Questions

This page contains frequently asked questions about Xcode.

## Does Xcode run on Windows?

No. Xcode runs only on macOS.

## Does Xcode run on iPads?

No. You can install the [Swift Playgrounds app](https://apps.apple.com/us/app/swift-playgrounds/id908519492) on an iPad. You can use the Swift Playgrounds app to learn Swift.

If your iPad is running iPadOS 15 (iOS 15) or later, you can use the Swift Playgrounds app to develop iOS apps on an iPad.

## Can I download Xcode without using the Mac App Store?

Yes. Apple has a [Downloads and Resources page](https://developer.apple.com/xcode/resources/) where you can download Xcode.

## Where can I download older versions of Xcode?

The site [Xcode Releases](https://xcodereleases.com) has direct download links for every version of Xcode Apple has ever released.

The main reason to download an older version of Xcode is that your Mac is running an older version of macOS that cannot run the most recent version of Xcode.

* Xcode 12.4 is the latest version for macOS 10.15.
* Xcode 11.3.1 is the latest version for macOS 10.14.
* Xcode 10.1 is the latest version for macOS 10.13.
* Xcode 9.2 is the latest version for macOS 10.12.
* Xcode 8.2.1 is the latest version for macOS 10.11.
* Xcode 7.2.1 is the latest version for macOS 10.10.
* Xcode 6.2 is the latest version for macOS 10.9. 

## The App Store says I don't have enough space to install Xcode, but I do. How do I fix this?

Free up more disk space on your Mac. You need 4-5 times the size of the Xcode download to install Xcode.

If Apple is telling you that you don't have enough space to install Xcode, you don't have enough space. A mistake many people make is comparing the Xcode download size to the amount of free space on their Mac. But the Xcode file you're downloading is a compressed file. The operating system has to expand the file. While expanding the file, the operating system needs space for both the compressed and expanded files.

### How do I free up space?

The app [DevCleaner for Xcode](http://www.one-minute-games.com/portfolio/dev-cleaner/) can free up space by removing caches and old simulator files that build up over time.

If you still don't have enough free space and have an existing version of Xcode on your Mac, delete it. This will free up space, but it will make an App Store Xcode installation take longer because it will have to download the entire Xcode file instead of performing a delta update, where only the parts that need to be updated are downloaded.

### Can I install Xcode on an external drive?

Xcode must be installed on your Mac’s startup disk. If you make an external drive the startup disk, you can install Xcode on an external drive. Use the System Preferences app (Choose Apple > System Preferences from the menu bar) to set the startup disk.

## Can I have multiple versions of Xcode installed?

Yes, you can have multiple versions of Xcode installed on your Mac. 

The most common time to have multiple Xcode versions installed is right after WWDC when Apple releases a beta version of the new version of Xcode. Install the beta alongside your existing Xcode installation to try the beta.

When you install Xcode from the Mac App Store, it gets installed in your Applications folder with the name Xcode. To have multiple versions installed, rename the existing Xcode on your Mac before you install the new version of Xcode.

## I updated my iOS device. Now I can't debug on it. Why?

Xcode does not support debugging on devices running a newer iOS version than the iOS SDK Xcode has. For example Xcode 12.1 includes the iOS 14.1 SDK. If you update your device to iOS 14.2, you won't be able to debug. It's annoying that a minor iOS update makes your device unusable on Xcode, but that's the way Xcode works.

To restore debugging update to the latest version, which may be a beta version.

A better long term strategy is to turn off automatic updates on your iOS device. Turning off the automatic updates will keep you from having to constantly install Xcode every time Apple releases a minor update to iOS.

Another workaround is to [download iOS support files for the newer iOS version](https://github.com/Yatko/iOS-device-support-files) and copy them to your Xcode app bundle.