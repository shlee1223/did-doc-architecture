# Wallet 정책
# Wallet Policy
## 앱 재설치하는 경우 사용할 수 있는 월렛
## Wallets Available for Use Upon Reinstallation
앱을 재설치할 때, 사용자가 사용할 수 있는 월렛 유형과 그에 따른 정책은 다음과 같습니다.

When reinstalling the app, the types of wallets available to the user and the corresponding policies are as follows.
### File Wallet
- **새로운 월렛 사용**: 앱을 재설치하는 경우 사용하려는 월렛이 File Wallet이면, 반드시 새로운 월렛을 사용해야 합니다.
    - **데이터 손실 방지**: 기존 월렛 데이터는 재설치 과정에서 손실될 수 있으므로 새로운 월렛을 생성하는 것이 필수적입니다.
- **단말기 제약**: File Wallet은 1인 다단말 정책을 지원하지 않습니다.
    - **단말기 제한**: 하나의 File Wallet은 단 하나의 단말기에서만 사용할 수 있습니다.
### File Wallet
- **Use a New Wallet**: If the wallet to be used is a File Wallet when reinstalling the app, a new wallet must be used.
    - **Prevent Data Loss**: Existing wallet data may be lost during the reinstallation process, so it is essential to create a new wallet.
- **Device Restrictions**: File Wallet does not support a one-person, multiple-device policy.
    - **Device Limitation**: One File Wallet can only be used on a single device.
### App Wallet
- **동일 단말기 사용**: 앱을 재설치하는 경우 사용하려는 월렛이 App Wallet이면, 같은 단말기에서만 이전 월렛을 사용할 수 있습니다.
    - **단말기 확인**: TAS는 반드시 App의 단말 정보를 알고 있어야 합니다.
- **단말기 제약**: App Wallet은 1인 다단말 정책을 지원하지 않습니다.
    - **단말기 제한**: 하나의 App Wallet은 단 하나의 단말기에서만 사용할 수 있습니다.
### App Wallet
- **Use on the Same Device**: If the wallet to be used is an App Wallet when reinstalling the app, the previous wallet can only be used on the same device.
    - **Device Verification**: TAS must know the device information of the App.
- **Device Restrictions**: App Wallet does not support a one-person, multiple-device policy.
    - **Device Limitation**: One App Wallet can only be used on a single device.
### Cloud Wallet
- **이전 월렛 사용 가능**: 앱을 재설치하는 경우 사용하려는 월렛이 Cloud Wallet이면, 단말 정책과 상관없이 이전 월렛을 사용할 수 있습니다.
    - **연속성 보장**: Cloud Wallet을 통해 사용자는 여러 단말기에서 동일한 월렛을 사용할 수 있습니다.
    - **편리성 강화**: 단말기 변경이나 앱 재설치 후에도 이전 월렛에 접근할 수 있어 사용자 편리성이 높아집니다.
    - **데이터 보존**: Cloud Wallet은 데이터를 클라우드에 저장하여 재설치나 단말기 변경 시에도 안전하게 데이터를 보존할 수 있습니다.
### Cloud Wallet
- **Previous Wallet Usable**: If the wallet to be used is a Cloud Wallet when reinstalling the app, the previous wallet can be used regardless of device policy.
    - **Ensure Continuity**: Through the Cloud Wallet, users can use the same wallet on multiple devices.
    - **Enhanced Convenience**: Users can access the previous wallet even after changing devices or reinstalling the app, increasing user convenience.
    - **Data Preservation**: Cloud Wallet stores data in the cloud, ensuring safe data preservation even during reinstallation or device changes.
## 요약
- **File Wallet**: 앱 재설치 시 새로운 월렛 사용, 1인 1단말 정책.
- **App Wallet**: 동일 단말기에서만 이전 월렛 사용 가능, 1인 1단말 정책.
- **Cloud Wallet**: 단말 정책과 상관없이 이전 월렛 사용 가능, 1인 다단말 정책 지원.

이러한 정책을 통해 사용자는 각 월렛 유형에 따른 적절한 사용 방식을 선택할 수 있으며, 보안과 편의성을 모두 고려한 월렛 관리가 가능합니다.
## Summary
- **File Wallet**: Use a new wallet upon app reinstallation, one-person, one-device policy.
- **App Wallet**: Previous wallet can only be used on the same device, one-person, one-device policy.
- **Cloud Wallet**: Previous wallet can be used regardless of device policy, supports a one-person, multiple-device policy.

These policies enable users to choose the appropriate usage method for each wallet type, allowing for wallet management that considers both security and convenience.
