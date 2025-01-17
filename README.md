# Steps to reproduce

1. `npm install`
2. `npx expo prebuild`
3. `npm run ios`

Observe the error in the console.

Removing either `@react-native-firebase/app` or `@stytch/react-native` causes the build to succeed.

The error I get is the following:

```

❌  (ios/Pods/Target Support Files/StytchReactNativeModule/StytchReactNativeModule-umbrella.h:14:9)

  12 | 
  13 | #import "StytchReactNativeModule.h"
> 14 | #import "RCAActionProtocol.h"
     |         ^ 'RCAActionProtocol.h' file not found
  15 | #import "RCARecaptchaClientProtocol.h"
  16 | #import "RCARecaptchaProtocol.h"
  17 | #import "RecaptchaInterop.h"
  ```
