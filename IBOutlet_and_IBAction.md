# IBOutlets and IBActions in iOS 📱


## What are `IBOutlets` and `IBActions`?
`IBOutlet` and `IBAction` are both methods used in Swift that directly bind to the Interface components that are used in your UI when building your iOS app. The prefix `IB` is a reference to the XCode Interface Builder.

## `IBOutlet`
An `IBOutlet` is used to reference a UI component on the storyboard and is used to change different properties of the referenced component. To connect a UI component to your code, command-click and drag a UI component onto your view controller file (usually named `ViewController.swift`) the resulting varible should look something similar to this:
```swift
@IBOutlet weak var myButton: UIButton!
```
Now, using the `myButton` variable, you can change various properties of the UI component (a `UIButton` in this case) like this:
``` swift
myButton.setTitleColor(UIColor.red)
```
## `IBAction`
An `IBAction` is used when you want to perform an action whenever the user interacts with a UI component, for example, handling a button click. In order to create a `IBAction` method, command-click and drag and drag a UI component onto your view controller file (usually named `ViewController.swift`) and the resulting method should look something like this:
```swift
@IBAction func buttonPress(sender: AnyObject) {
   print("HEY! I'VE PRESSED THE BUTTON")
}
```







