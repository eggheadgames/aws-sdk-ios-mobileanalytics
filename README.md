# Amazon Mobile Analytics for iOS
Mobile Analytics binaries from [AWS Mobile SDK for iOS](https://github.com/aws/aws-sdk-ios).

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
