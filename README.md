# ABWebView
A utility control which is using fast WKWebView which is introduced in iOS8. Just set URL to load and it will do the rest. Very easy to implement.

## Demo
![gif1](https://raw.githubusercontent.com/asifbilal786/ABPasscodeViewController/screenshots/ABPasscode.gif)

## Requirements

- iOS 8 and above.
- Xcode 8 and above


## Adding ABPasscodeViewController to your project

### METHOD 1:
1. Add a pod entry for `ABWebView` to your Podfile

```ruby
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!

pod 'ABWebView', '~> 0.1'
``` 

2. Install the pod(s) by running `pod install`.

### MEHTOD 2: (Source files)
Alternatively, you can directly add all files under the folder Core to your project.

1. Download the [latest code version](https://github.com/asifbilal786/ABWebView/archive/master.zip) or add the repository as a git submodule to your git-tracked project.
2. Open your Xcode project, then drag and drop source directory onto your project. Make sure to select Copy items when asked if you extracted the code archive outside of your project.
 

## Usage

Create instance variable of PhotoPicker in your view controller and push in navigation controller.

```
let passcodeVC = PasscodeViewController()
passcodeVC.delegate = self
navigationController?.pushViewController(passcodeVC, animated: true)
```

And then call the delegate functions for different event.

```
let webViewController = ABWebViewController()
webViewController.URLToLoad = "https://apple.com"
navigationController?.pushViewController(webViewController, animated: true)
```

See example projects for detail.

## License
This code is distributed under the terms and conditions of the [MIT license](LICENSE). 

