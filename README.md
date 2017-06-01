# Amazon Mobile Analytics for iOS
Mobile Analytics binaries from [AWS Mobile SDK for iOS](https://github.com/aws/aws-sdk-ios).

The `aws-sdk-ios` library can take 30 minutes to compile.
This can be painful when all you need is a couple of pieces of it.
This library has just the compiled binary for [AWSMobileAnalytics](https://github.com/aws/aws-sdk-ios/tree/master/AWSMobileAnalytics).

## How to Use with Carthage

Add the following line to your `Cartfile`:
```
github "eggheadgames/aws-sdk-ios-mobileanalytics"
```
This will include the latest version. Look under the Releases tab to see other versions that might be available.


## How to build

1. Clone `https://github.com/aws/aws-sdk-ios`
2. Build in Xcode
3. Locate `AWSCore.framework` and `AWSMobileAnalytics.framework` build artifacts
4. Create `aws-sdk-ios-mobileanalytics.framework.zip` with the following structure:
    ```
    |-+ Carthage
      |-+ Build
        |-+ iOS
          |- AWSCore.framework
          |- AWSMobileAnalytics.framework
    ```
5. Draft GitHub release of `eggheadgames/aws-sdk-ios-mobileanalytics`
6. Add `aws-sdk-ios-mobileanalytics.framework.zip` as binary attachement
7. Publish new release
