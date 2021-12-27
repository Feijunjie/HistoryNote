1.xcode编译命令

```
1.
xcodebuild build -workspace YppLife.xcworkspace -scheme YppLife SYMROOT="$(pwd)/Res/analyse_Package/tempApp" -destination 'platform=iOS Simulator,name=iPhone 12' CODE_SIGN_IDENTITY= CODE_SIGNING_REQUIRED=NO CODE_SIGNING_ALLOWED=NO

2.xcodebuild build -workspace YppLife.xcworkspace -scheme YppLife SYMROOT="$(pwd)/Res/analyse_Package/tempApp" -configuration Debug -sdk iphoneos14.5 CODE_SIGN_IDENTITY= CODE_SIGNING_REQUIRED=NO CODE_SIGNING_ALLOWED=NO
```

第二中有时候编译会失败，找不到路径，可以用第一个，如果失败再用第二个。

