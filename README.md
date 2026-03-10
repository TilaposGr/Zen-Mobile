# Zen Browser for Android

NOT AFFILIATED WITH THE ZEN OSS TEAM!


Zen browser mobile is the all-new Firefox-based Android browser, based on [GeckoView](https://mozilla.github.io/geckoview/) and [Mozilla Android Components](https://mozac.org/).

## I want to file an issue!

Great! We encourage you to participate in this open source project. We love Pull Requests, Bug Reports, ideas, (security) code reviews or any other kind of positive contribution.

To make it easier to triage, we have these issue requirements:

* Please do your best to search for duplicate issues before filing a new issue so we can keep our issue board clean.
* Every issue should have **exactly** one bug/feature request described in it. Please do not file meta feedback list tickets as it is difficult to parse them and address their individual points.
* Feature Requests are better when they’re open-ended instead of demanding a specific solution -ie  “I want an easier way to do X” instead of “add Y”
* Issues are not the place to go off topic or debate. If you have questions, please join the [#fenix:mozilla.org channel](https://chat.mozilla.org/#/room/#fenix:mozilla.org).
* Please always remember our [Community Participation Guidelines](https://www.mozilla.org/en-US/about/governance/policies/participation/)
* Please do not tag specific team members to try to get your issue looked at faster. We have a triage process that will tag and label issues correctly in due time. If you think an issue is very severe, you can ask about it in Matrix.

Please keep in mind that even though a feature you have in mind may seem like a small ask, as a small team, we have to prioritize our planned work and every new feature adds complexity and maintenance and may take up design, research, marketing, product, and engineering time. We appreciate everyone’s passion but we will not be able to incorporate every feature request or even fix every bug. That being said, just because we haven't replied, doesn't mean we don't care about the issue, please be patient with our response times as we're very busy.

## Build Instructions

Pre-requisites:
* Android SDK
* To run command line tools, you'll need to configure Java: see [our how-to guide](https://github.com/mozilla-mobile/shared-docs/blob/master/android/configure_java.md).

1. Clone or Download the repository:

  ```shell
  git clone https://github.com/mozilla-mobile/fenix
  ```

2. **Import** the project into Android Studio **or** build on the command line:

  ```shell
  ./gradlew clean app:assembleDebug
  ```

  If this errors out, make sure that you have an `ANDROID_SDK_ROOT` environment
  variable pointing to the right path.

3. Make sure to select the correct build variant in Android Studio. See the next section.

4. Make sure to select "Default APK" under Installation Options inside Run/Debug configuration: see [this bug](https://bugzilla.mozilla.org/show_bug.cgi?id=1529082).
