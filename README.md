# Trusting SDKs - HTTPS

A crowd-sourced list of SDKs and how they protect their downloads with HTTPS.

Based on the [Trusting SDKs post](https://krausefx.com/blog/trusting-sdks) by [@KrauseFx](https://twitter.com/KrauseFx) this repo contains a crowd-sourced list of SDKs and their status when it comes to security when downloading the binary or source code.

## iOS SDKs

You can get a list of the most used iOS SDKs on [AppSight](https://www.appsight.io/?asot=2&o=top&os=ios)

| SDK | Has official CocoaPod | Website that links encrypted | Download uses HTTPS | Open Source |
| --- | :---: | :---: | :---: | :---: |
| [Facebook SDK](https://developers.facebook.com/docs/ios/) | ✅ | ✅ | ✅ | ✅ |
| [AWS SDK](https://aws.amazon.com/documentation/sdk-for-ios/) | ✅ | ✅ | ✅ | ✅ |
| [AppsFlyer](https://support.appsflyer.com/hc/en-us/articles/207032066-AppsFlyer-SDK-Integration-iOS) | ✅ | ✅ | ✅ | ⚠️ |
| [Realm](https://github.com/realm/realm-cocoa) | ✅ | ✅ | ✅ | ⚠️ |
| [Mixpanel](https://mixpanel.com/help/reference/ios) | ✅ | ✅ | ✅ | ✅ |
| [Braintree](https://developers.braintreepayments.com/guides/client-sdk/setup/ios/v4) | ✅ | ✅ | ✅ | ✅ |
| [Branch](https://github.com/BranchMetrics/ios-branch-deep-linking) | ✅ | ✅ | ✅ | ✅ |
| [Amplitude](https://amplitude.zendesk.com/hc/en-us/articles/115002278527-iOS-SDK-Installation) | ✅ | ✅ | ✅ | ✅ |
| [Appsee](https://www.appsee.com/docs/ios/native) | ✅ | ✅ | ✅ | ⚠️ |
| [Crashlytics](https://try.crashlytics.com/) | ✅ | ✅ | ✅ | ⚠️ |
| [Firebase](https://firebase.google.com/docs/ios/setup) | ✅ | ✅ | ✅ | ⚠️ |
| [Heap](https://heapanalytics.com/) | ✅ | ✅ | ✅ | ⚠️ |
| [leanplum](https://www.leanplum.com/) | ✅ | ✅ | ✅ | ✅ |
| [Chartboost](https://answers.chartboost.com/en-us/articles/download) | ❌ | ✅ | ❌ | ⚠️ |
| [AskingPoint](https://www.askingpoint.com/documentation-ios-sdk/) | ❌ | ✅ | ❌ | ⚠️ |
| [Google Analytics](https://developers.google.com/analytics/devguides/collection/ios/v3/) | ✅ | ✅ | ✅ | ⚠️ |
| [Customerly SDK](https://www.customerly.io/customers-intelligence) | ✅ | ✅ | ✅ | ✅ |
| [HockeyApp](https://github.com/bitstadium/HockeySDK-iOS#readme) | ✅ | ✅ | ✅ | ✅ |
| [VS App Center](https://github.com/Microsoft/appcenter-sdk-apple#readme) | ✅ | ✅ | ✅ | ✅ |
| [Evernote SDK](https://github.com/evernote/evernote-cloud-sdk-ios) | ✅ | ✅ | ✅ | ✅ |
| [Carnival SDK](https://github.com/carnivalmobile/carnival-ios-sdk/)| ✅ | ✅ | ✅ | ⚠️ |
| [PSPDFKit for iOS/macOS](https://pspdfkit.com/)| ✅ | ✅ | ✅ | ⚠️ |
| [Instabug](https://instabug.com/)| ✅ | ✅ | ✅ | ⚠️ |
| [Intercom iOS SDK](https://github.com/intercom/intercom-ios)| ✅ | ✅ | ✅ | ⚠️ |
| [Zendesk Support SDK](https://github.com/zendesk/zendesk_sdk_ios)| ✅ | ✅ | ✅ | ⚠️ |
| [Zendesk Chat SDK](https://github.com/zendesk/zendesk_sdk_chat_ios)| ✅ | ✅ | ✅ | ⚠️ |
| [Sentry SDK](https://github.com/getsentry/sentry-cocoa) | ✅ | ✅ | ✅ | ✅ |
| [PhotoEditor SDK iOS](https://www.photoeditorsdk.com/)| ✅ | ✅ | ✅ | ⚠️ |

#### Has official CocoaPod

- ✅ A CocoaPod is available on CocoaPods.org, and is maintained by the company providing the SDK.
- ❌ No CocoaPod is available, or the pod that's available is published or maintained by a third party

As soon as the pod is maintained by a third party, the SDK is out of the control of the company providing it, adding an extra layer of security risks.

#### Website that links encrypted

- ✅ The website linking to the download of the SDK (or the CocoaPods page) is HTTPS encrypted by default
- ❌ The website linking to the download uses unencrypted HTTP

This is critical, as by having the marketing or docs page be unencrypted allows an attack to re-write any links to different URLs, as described in [trusting SDKs](https://krausefx.com/blog/trusting-sdks) in the `Localytics` section.

#### Download uses HTTPS

This section is about the `Manual Installation` section most SDKs provides. As mentioned in [trusting SDKs](https://krausefx.com/blog/trusting-sdks) most of the pods on CocoaPods are secure.

- ✅ The download of the SDK happens via HTTPS by default
- ❌ The download of the SDK uses unencrypted HTTP by default, or doesn't support HTTPS at all

If the download doesn't happen via HTTPS be extra cautious when using the SDK, and notify the SDK provider.

#### Open Source

- ✅ The SDK is open source, meaning you can see what kind of data the SDK tracks, and what web hosts it accesses
- ⚠️ The SDK is not open source - this doesn't mean it's bad, it just means you can't see what the SDK does

The risks of a closed source SDK is described in detail in [trusting SDKs](https://krausefx.com/blog/trusting-sdks). In particular when it comes to accessing user data, keychain entries and photos this might add an risk.

## Contributing

This repo is community-driven. To update the information of an SDK, just submit a Pull Request to this repo. You can use [the GitHub online editor](https://github.com/trusting-sdks/https/edit/master/README.md) to easily edit text online, without having to manually clone the repo.

[**Click here to edit this file**](https://github.com/trusting-sdks/https/edit/master/README.md)
