#phonegap-plugin-push [![Build Status](https://travis-ci.org/phonegap/phonegap-plugin-push.svg)](https://travis-ci.org/phonegap/phonegap-plugin-push)

> Register and receive push notifications

#iSense it fork

**Why a fork?**
To be compatible with the Kinvey notification service. https://www.kinvey.com/
Kinvey sends the body content of the message as "MESSAGE" which is a the name already used in android. It isn't a problem as long as you don't need to send a title or any other custom element.
But if you need to send custom keys, the GCMInterService will overwrite the message custom element with the original kinvey packet.
Which will put an object in place of text on the Message property, leading to a very ugly notification.

In all other use cases, use the official plugin.
https://github.com/phonegap/phonegap-plugin-push

# What is this?

This plugin offers support to receive and handle native push notifications with a **single unified API**. 

Starting with version `1.9.0`, this plugin will support `CocoaPods` installation of the `Google Cloud Messaging` library. More details are available in the [Installation](docs/INSTALLATION.md#cocoapods) documentation.

- [Reporting Issues](docs/ISSUES.md)
- [Installation](docs/INSTALLATION.md)
- [API reference](docs/API.md)
- [Typescript support](docs/TYPESCRIPT.md)
- [Examples](docs/EXAMPLES.md)
- [Platform support](docs/PLATFORM_SUPPORT.md)
- [Cloud build support (PG Build, IntelXDK)](docs/PHONEGAP_BUILD.md)
- [Push notification payload details](docs/PAYLOAD.md)
- [Contributing](.github/CONTRIBUTING.md)
- [License (MIT)](MIT-LICENSE)


# Do you like tutorial? You get tutorial!

 - [PhoneGap Day US Push Workshop 2016 (using node-gcm)](http://macdonst.github.io/push-workshop/)
 - [PhoneGap Day EU Push Workshop 2016 (using PhoneGap Push)](http://macdonst.github.io/push-workshop-eu/)
