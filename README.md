# aws-sdk-ios-mobileanalytics
Mobile Analytics binaries from [AWS Mobile SDK for iOS](https://github.com/aws/aws-sdk-ios), and dependencies.

## How to build AWS Mobile Analytics
1. Clone `https://github.com/aws/aws-sdk-ios` from GitHub and build with Xcode
2. Get both `AWSMobileAnalytics.framework` and `AWSCore.framework` 
3. Pack `AWSMobileAnalytics.framework` and `AWSCore.framework` in a zip archive with the following structure:

   |--Carthage

        |--Build

             |--iOS

                  |--AWSCore.framework

                  |--AWSMobileAnalytics.framework


4. Name the zip: `aws-sdk-ios-mobileanalytics.framework.zip`
5. **Draft a new release** for `eggheadgames/aws-sdk-ios-mobileanalytics`
6. Add zip file `aws-sdk-ios-mobileanalytics.framework.zip` into the **Attach binaries** section
7. **Publish release**
8. *Note - when dependencies are built with Carthage*, in another project: 

`AWSCore.framework` and `AWSMobileAnalytics.framework` are not downloaded if `--no-use-binaries` option is used in Carthage



