# Amazon IVS Broadcast with Snap Camera Kit for Android Demo

This repository contains a demo app, which shows how to integrate the Amazon IVS mobile broadcast SDK with Snap's Camera Kit to create a mobile streaming app on Android using Kotlin. It is based on [Snap's Camera Kit Sample Custom Lenses Carousel and Camera Preview app](
https://github.com/Snapchat/camera-kit-reference/tree/main/samples/android/camerakit-sample-custom-carousel) has been modified to use the Amazon IVS Broadcast SDK for Android to live stream the processed camera feed.


## Build

### Amazon IVS Setup
 
Enter values for your Amazon IVS channel's stream key and ingest server endpoint in `gradle.properties`.
The stream key should be assigned to `com.amazon.aws.ivs.key` and ingest server endpoint should be assigned
to `com.amazon.aws.ivs.endpoint`. See 
[Getting Started with Amazon IVS](https://docs.aws.amazon.com/ivs/latest/userguide/getting-started.html) for
reference on how to create a channel and get your stream key and ingest server endpoint.

### Snap Camera Kit SDK Setup

Open project's `gradle.properties` file and enter values for `com.snap.camerakit.application.id`
, `com.snap.camerakit.api.token` from [Snap Kit Developer Portal](https://snapkit.com/manage)
and `com.snap.camerakit.lenses.group.id` from
your [Camera Kit Portal](https://camera-kit.snapchat.com/). 

After that to build, install and launch
the `camerakit-sample-custom-carousel` on a connected device follow one of the following options:

### Command Line

- `./gradlew camerakit-sample-custom-carousel:installDebug`

- `adb shell am start -n com.snap.camerakit.sample.carousel/com.snap.camerakit.sample.carousel.MainActivity`

### IDE

Select the `camerakit-sample-custom-carousel` module configuration and click run.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

---

This package requires and may incorporate or retrieve a number of third-party
software packages (such as open source packages) at install-time or build-time
or run-time ("External Dependencies"). The External Dependencies are subject to
license terms that you must accept in order to use this package. If you do not
accept all of the applicable license terms, you should not use this package. We
recommend that you consult your company’s open source approval policy before
proceeding.

Provided below is a list of External Dependencies and the applicable license
identification as indicated by the documentation associated with the External
Dependencies as of Amazon's most recent review.

THIS INFORMATION IS PROVIDED FOR CONVENIENCE ONLY. AMAZON DOES NOT PROMISE THAT
THE LIST OR THE APPLICABLE TERMS AND CONDITIONS ARE COMPLETE, ACCURATE, OR
UP-TO-DATE, AND AMAZON WILL HAVE NO LIABILITY FOR ANY INACCURACIES. YOU SHOULD
CONSULT THE DOWNLOAD SITES FOR THE EXTERNAL DEPENDENCIES FOR THE MOST COMPLETE
AND UP-TO-DATE LICENSING INFORMATION.

YOUR USE OF THE EXTERNAL DEPENDENCIES IS AT YOUR SOLE RISK. IN NO EVENT WILL
AMAZON BE LIABLE FOR ANY DAMAGES, INCLUDING WITHOUT LIMITATION ANY DIRECT,
INDIRECT, CONSEQUENTIAL, SPECIAL, INCIDENTAL, OR PUNITIVE DAMAGES (INCLUDING
FOR ANY LOSS OF GOODWILL, BUSINESS INTERRUPTION, LOST PROFITS OR DATA, OR
COMPUTER FAILURE OR MALFUNCTION) ARISING FROM OR RELATING TO THE EXTERNAL
DEPENDENCIES, HOWEVER CAUSED AND REGARDLESS OF THE THEORY OF LIABILITY, EVEN
IF AMAZON HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. THESE LIMITATIONS
AND DISCLAIMERS APPLY EXCEPT TO THE EXTENT PROHIBITED BY APPLICABLE LAW.

---

License for Camera Kit:

© 2023 Snap Inc. All Rights Reserved.

Access to or use of Camera Kit and its associated documentation, software code, and other materials (collectively, “Camera Kit”), made available by Snap Inc. and its affiliates ("Snap"), is subject to the Snap Camera Kit Terms, which you have already accepted and can be found at:

https://www.snap.com/terms/snap-camera-kit

If you no longer want to be a party to these terms, or if you do not agree to all of these terms, do not use or otherwise access Camera Kit and notify Snap immediately. Camera Kit may contain Snap confidential information.

