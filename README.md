# JNBBottombar

[![CI Status](https://img.shields.io/travis/jnblanchard@mac.com/JNBBottombar.svg?style=flat)](https://travis-ci.org/jnblanchard@mac.com/JNBBottombar)
[![Version](https://img.shields.io/cocoapods/v/JNBBottombar.svg?style=flat)](https://cocoapods.org/pods/JNBBottombar)
[![License](https://img.shields.io/cocoapods/l/JNBBottombar.svg?style=flat)](https://cocoapods.org/pods/JNBBottombar)
[![Platform](https://img.shields.io/cocoapods/p/JNBBottombar.svg?style=flat)](https://cocoapods.org/pods/JNBBottombar)

![](https://static.wixstatic.com/media/8e69fb_e74803bfa5144e44bc429689a8d67465~mv2.gif)

## Requirements

iOS 11+

## Installation

JNBBottombar is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'JNBBottombar'
```

## Example

Here's how one may show a greeting label for two and a half seconds.
```swift
JNBBottombar.shared.showWith(contentView: label,
                             contentBackgroundColor: UIColor.black,
                             cornerRadius: 6,
                             screenInsets: UIEdgeInsets(top: 0, left: -8, bottom: -16, right: -8),
                             shadowColor: UIColor.black.cgColor,
                             shadowOpacity: 0.7,
                             shadowRadius: 10,
                             borderWidth: 2.0,
                             borderColor: UIColor.white.cgColor,
                             forDuration: 2.5,
                             completion: nil)

If you do not specify a forDuration; the bar will show until hide or another call to show is made.
JNBSnackbar.shared.hide { (completed) in
  guard completed else { return }
  // bar has finished animating down
}
```

## License

MIT license. See the LICENSE file for more info.

## Author

jnblanchard@mac.com
