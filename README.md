# CocoaPods Support for Carthage Projects

[![Build Status](https://travis-ci.org/emirandm/CocoaPodsSupport.svg?branch=master)](https://travis-ci.org/emirandm/CocoaPodsSupport)
![Carthage Compatible](https://img.shields.io/badge/carthage-compatible-4BC51D.svg?style=flat)
![Swift Version](https://img.shields.io/badge/swift-4.0-brightgreen.svg)


Simple Cocoa Touch project providing support of CocoaPods libraries in projects using Carthage as a dependency manager.

## Included CocoaPods libraries
* [GoogleTagManager](https://cocoapods.org/pods/GoogleTagManager) version 6.0

## Usage
### [Carthage](https://github.com/Carthage/Carthage)
Add the following line to your `Cartfile`:
```
github "massiveinteractive/CocoaPodsSupport"
```
And run:
```
carthage update
```

## Adding a new CocoaPods library
### Prerequisites
* [CocoaPods](https://cocoapods.org/)
  * `sudo gem install cocoapods`

In order to add `YourCocoaPodsLibrary` you need to specify it in the `Podfile` of the project:

```ruby
target 'CocoaPodsSupport' do
    pod 'GoogleTagManager', '6.0'
    # ...
    pod 'YourCocoaPodsLibrary'
end
```
And run:
```
pod install
```
To download and install `YourCocoaPodsLibrary` into the project.
