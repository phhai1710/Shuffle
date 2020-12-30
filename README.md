<p align="center">
<img src="https://raw.githubusercontent.com/mac-gallagher/Shuffle/master/Assets/logo.png" width="650">
</p>

## What is the difference from original Shuffle?

💡 Open numberOfVisibleCards to decide how many cards will be shown in the same time. 

💡 Implement underlay view 

## Example

To run the example project, clone the repo and run the `ShuffleExample` target.

<p align="left">
<img src="https://raw.githubusercontent.com/mac-gallagher/Shuffle/master/Assets/swipe_example.gif" width="280">
</p>

## Card Layout

The following methods are available on `SwipeCardStack`.

### 1. numberOfVisibleCards

Change the number of visible cards (Default is 2):

```swift
cardStack.numberOfVisibleCards = 2
```

<p align="left">
<img src="https://raw.githubusercontent.com/phhai1710/Shuffle/master/Assets/underlayView.gif" width="280">
</p>

```
cardStack.numberOfVisibleCards = 1
```

<p align="left">
<img src="https://raw.githubusercontent.com/phhai1710/Shuffle/master/Assets/numberOfVisibleCards.gif" width="280">
</p>



### 2. Underlays

An underlay is a view whose alpha value reacts to the user's dragging. The underlay are laid out below the top visible card. 

```swift
func underlay(forDirection direction: SwipeDirection) -> UIView?
func setCardUnderlay(_ cardUnderlay: UIView?, forDirection direction: SwipeDirection)
func setCardUnderlays(_ cardUnderlays: [SwipeDirection: UIView])
```

<p align="left">
<img src="https://raw.githubusercontent.com/phhai1710/Shuffle/master/Assets/underlayView.gif" width="280">
</p>

## Installation

### CocoaPods

Shuffle is available through [CocoaPods](<https://cocoapods.org/>). To install it, simply add the following line to your `Podfile`:

	pod 'Shuffle-iOS', :git => 'https://github.com/phhai1710/Shuffle.git'

The import statement in this case will be

```swift
import Shuffle_iOS
```

### Manual

Download and drop the `Shuffle` directory into your project.

## Requirements

* iOS 9.0+
* Xcode 10.2+
* Swift 5.0+
