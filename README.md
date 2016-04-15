![iOS 9 logo](https://devimages.apple.com.edgekey.net/assets/elements/icons/64x64/ios-9_2x.png)

## Official Apple Resources
[Official Resources](https://developer.apple.com/resources) - Great way to familiarize yourself with technologies and best practicies; not just limited to design.

[Design Resources](https://developer.apple.com/design)

[iOS Human Interface Guidelines](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/index.html)

[UI Design Do’s and Don’ts](https://developer.apple.com/design/tips)

[iOS 7 Transition Guide](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/TransitionGuide/index.html#//apple_ref/doc/uid/TP40013174-CH6-SW1) - This guide can be beneficial if you worked with older versions of iOS (1-6) and need a way to grasp Apple's new design principals.

## UI

### UIKit

UIKit is a framework provided by Apple to aid in the development of an app's user interface. UIKit has all the basic components to build nearly any UI/UX you can dream up. You can think of UIKit as a designer/developer's LEGO kit for app development. Becoming familiar with the basic components in UIKit and their default behavior is essential to understanding which parts of your design are possible without having to develop a custom component. Understanding UIKit components and  Apple's Human Interface Guidelines will enable you to design a beautiful, native UI.

### Xcode and Interface Builder

Xcode is an application used to write apps for various Apple platforms. Interface Builder is a tool within Xcode which allows users to develop portions of an app visually, without having to write code. The screenshot below shows all of the UI elements available in Interface Builder.

![UI Objects](https://github.com/remypanicker/ios-ui-ux/blob/master/interface-builder-uikit.png)

### Points vs Pixels

Pixel density varies across devices. The tools used to develop apps expect specifications to be in points, thus design specs should be in points. But why points and not pixels? Here's an excerpt from Apple in the official [iOS Drawing Concepts Reference](https://developer.apple.com/library/ios/documentation/2DDrawing/Conceptual/DrawingPrintingiOS/GraphicsDrawingOverview/GraphicsDrawingOverview.html#//apple_ref/doc/uid/TP40010156-CH14-SW2)

> > **One point does not necessarily correspond to one physical pixel.**

> The purpose of using points (and the logical coordinate system) is to provide a consistent size of output that is device independent. For most purposes, the actual size of a point is irrelevant. The goal of points is to provide a relatively consistent scale that you can use in your code to specify the size and position of views and rendered content. How points are actually mapped to pixels is a detail that is handled by the system frameworks. For example, on a device with a high-resolution screen, a line that is one point wide may actually result in a line that is two physical pixels wide. The result is that if you draw the same content on two similar devices, with only one of them having a high-resolution screen, the content appears to be about the same size on both devices.

PaintCode has created an easy-to-digest infographic which depicts the conversion from points to pixels:

[The Ultimate Guide to iPhone Resolutions](http://www.paintcodeapp.com/news/ultimate-guide-to-iphone-resolutions)

## UX

### View States
[Mobile Views: The FIVE State Solution](http://scotthurff.com/posts/why-your-user-interface-is-awkward-youre-ignoring-the-ui-stack) - Informative article about how to consider each view in your app for a more informative user experience.


### Prototyping

Creating a prototype is a powerful way to quickly iterate through ideas. Prototypes are also a low(er?) cost way to validate your UX and communicate complex interactions. 

[Prototyping - Fake It Till You Make It (WWDC 2014)](https://developer.apple.com/videos/play/wwdc2014/223/)

#### Prototyping Tools

[Interface Builder](https://developer.apple.com/xcode/interface-builder)

[Flinto](https://www.flinto.com)

[InVision](https://www.invisionapp.com)

[Marvel](https://marvelapp.com/prototype-with-sketch/)

[Origami](https://facebook.github.io/origami/)

[Origami Studio](https://www.facebook.com/media/set/?set=a.606446952851229.1073741828.245766762252585&type=3) - Will be available for free late 2016.

## Found an issue?
Open a [GitHub issue](https://github.com/remypanicker/ios-ui-ux/issues) with details so that it can get fixed!

## Contribute
Open a [pull request](https://github.com/remypanicker/ios-ui-ux/pulls) or contact me with suggestions to make this collection better.

## Contact
Feel free to reach out

Twitter: [@remypanicker](http://twitter.com/remypanicker)

Email: [rpanicke@gmail.com](mailto:rpanicke@gmail.com)
