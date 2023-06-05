# Trusting SDKs - HTTPS

A crowd-sourced list of SDKs and how they protect their downloads with HTTPS.

Based on the [Trusting SDKs post](https://krausefx.com/blog/trusting-sdks) by [@KrauseFx](https://twitter.com/KrauseFx) this repo contains a crowd-sourced list of SDKs and their status when it comes to security when downloading the binary or source c
✅ | ✅ | ✅ | ⚠️ |
| [Amplitude](https://amplitude.zendesk.com/hc/en-us/articles/115002278527-iOS-SDK-Installation) | ✅ | ✅ | ✅ | ✅ |

| [Crashlyti(https://try.crashlytics.com/) | ✅ | ✅ | ✅ | ⚠️ |
| [leanplum] (https://www.leanplum.com/) | ✅ | ✅ | ✅ | ✅ |
| 
| [AskingPoint) | ❌ | ✅ | ❌ | ⚠️ |
) | ✅ | 
| [SDK de Custo(https://www.customerly.io/customers-intelligence) | ✅ | ✅ | ✅ | ✅ |
| [VS
| [SDK de Evernote] ( 
- ✅ Un CocoaPod está disponible en CocoaPods.org y lo mantiene la empresa que proporciona  DK.
- ❌ No CocoaPod is available, or the pod that's available is published or maintained by a third party

As soon as the pod is maintained by a third party, the SDK is out of the control of the company providing it, adding an extra layer of security risks.

#### Download uses HTTPS

This section is about the `Manual Installation` section most SDKs provides. As mentioned in [trusting SDKs](https://krausefx.com/blog/trusting-sdks) most of the pods on CocoaPods are secure.

- ✅ The download of the SDK happens via HTTPS by default
- ❌ The download of the SDK uses unencrypted HTTP by default, or doesn't support HTTPS at all

If the download doesn't happen via HTTPS be extra cautious when using the SDK, and notify the SDK provider.

## Contributing

This repo is community-driven. To update the information of an SDK, just submit a Pull Request to this repo. You can use [the GitHub online editor](https://github.com/trusting-sdks/https/edit/master/README.md) to easily edit text online, without having to manually clone the repo.

[**Click here to edit this file**](https://github.com/trusting-sdks/https/edit/master/README.md)
