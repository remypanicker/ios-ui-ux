![iOS 9 logo](https://devimages.apple.com.edgekey.net/assets/elements/icons/64x64/ios-9_2x.png)

## Official Apple Resources
[Official Resources](https://developer.apple.com/resources) - Great way to familiarize yourself with technologies and best practicies; not just limited to design.

[Design Resources](https://developer.apple.com/design)

[iOS Human Interface Guidelines](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/index.html)

[UI Design Do’s and Don’ts](https://developer.apple.com/design/tips)

[iOS 7 Transition Guide](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/TransitionGuide/index.html#//apple_ref/doc/uid/TP40013174-CH6-SW1) - This guide can be beneficial if you worked with older versions of iOS (1-6) and need a way to grasp Apple's new design principals.

## UI

### Xcode and Interface Builder

Xcode is an application used to write apps for various Apple platforms. Interface Builder is a tool within Xcode which allows users to develop portions of an app visually, without having to write code.

### UIKit

UIKit is a framework provided by Apple to aid in the development of an app's user interface. UIKit has all the basic components to build nearly any UI/UX you can dream up. You can think of UIKit as a designer/developer's LEGO kit for app development. Becoming familiar with the basic components in UIKit and their default behavior is essential to understanding which parts of your design are possible without having to develop a custom component. Understanding UIKit components and  Apple's Human Interface Guidelines will enable you to design a beautiful, native UI.

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

// todo

## Found an issue?
Open a [GitHub issue](https://github.com/remypanicker/ios-ui-ux/issues) with details so that it can get fixed!

## Contribute
Open a [pull request](https://github.com/remypanicker/ios-ui-ux/pulls) or contact me with suggestions to make this collection better.

## Contact
Feel free to reach out

Twitter: [@remypanicker](http://twitter.com/remypanicker)

Email: [rpanicke@gmail.com](mailto:rpanicke@gmail.com)
