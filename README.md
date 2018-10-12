# CocoaPods Support for Carthage Projects
Simple Cocoa Touch project providing support of CocoaPods libraries in projects using Carthage as a dependency manager.

## Included CocoaPods libraries
* [GoogleTagManager](https://cocoapods.org/pods/GoogleTagManager) version 6.0

## Requirements
* [CocoaPods](https://cocoapods.org/)
  * `sudo gem install cocoapods`

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
In order to add "YourCocoaPodsLibrary" you need to specify it in the `Podfile` of the project:

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
