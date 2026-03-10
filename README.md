# Zen Browser for Android

NOT AFFILIATED WITH THE ZEN OSS TEAM!


Zen browser mobile is the all-new Firefox-based Android browser, based on [GeckoView](https://mozilla.github.io/geckoview/) and [Mozilla Android Components](https://mozac.org/).

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
