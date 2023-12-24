# app-crawler-action

Github action which runs android app crawler action.
Uses the https://developer.android.com/studio/test/other-testing-tools/app-crawler 
and inspired after reading https://medium.com/@Amr.sa/the-ultimate-guide-for-cross-platform-e2e-test-for-native-mobile-app-b87b5949ff45



## Usage

In your GitHub action, to app crawl your apk on a emulator:

```yml
- name: 'Android App Crawler'
  uses: mrgklwong/app-crawler-action@v1
  with:
    # APK path
    app-location: location_to_your_app
    # APK package name
    app-package-name: name_of_your_app
```

## Advanced Usage

```yml
- name: 'Android App Crawler'
  uses: mrgklwong/app-crawler-action@v1
  with:
    # APK path
    app-location: location_to_your_app
    # APK package name
    app-package-name: name_of_your_app
    # default inputs provided for all the below 
    ANDROID_ARCH: x86_64
    ANDROID_TARGET: google_apis_playstore
    API_LEVEL: 28'
    ANDROID_BUILD_TOOLS_VERSION: 28.0.3
    EMULATOR_TIMEOUT: '350'
    EMULATOR_NAME: nexus
```
