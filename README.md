# Adobe Mobile SDK & SQLCipher Issue Reproduction

Reproduces an iOS build error when using [Adobe Experience Platform Mobile SDKs](https://github.com/adobe/aepsdk-core-ios) and [SQLCipher](https://www.zetetic.net/sqlcipher/sqlcipher-ios/) together in the same iOS project.

<img src="@docs/issue.png">

Summary of the problem is [this line of code](https://github.com/adobe/aepsdk-core-ios/blob/4.2.3/AEPServices/Sources/dataqueue/SQLiteWrapper.swift#L14) in Adobe's lib causes [this issue](https://www.zetetic.net/sqlcipher/ios-tutorial/#option-2-cocoapod-integration):

<img src="@docs/sqlcipher.png">