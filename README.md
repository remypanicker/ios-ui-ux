![iOS 12 logo](https://developer.apple.com/assets/elements/icons/ios-12/ios-12-96x96_2x.png)

## Official Apple Resources
[Official Resources](https://developer.apple.com/resources) - Great way to familiarize yourself with technologies and best practicies; not just limited to design.

[Design Resources](https://developer.apple.com/design)

[iOS Human Interface Guidelines](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/index.html)

[UI Design Do’s and Don’ts](https://developer.apple.com/design/tips)

## UI

### UIKit

UIKit is a framework provided by Apple to aid in the development of an app's user interface. UIKit has all the basic components to build nearly any UI/UX you can dream up. You can think of UIKit as a designer/developer's LEGO kit for app development. Becoming familiar with the basic components in UIKit and their default behavior is essential to understanding which parts of your design are possible without having to develop a custom component. Understanding UIKit components and  Apple's Human Interface Guidelines will enable you to design a beautiful, native UI.

[UIKit User Interface Catalog](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/UIKitUICatalog/index.html#//apple_ref/doc/uid/TP40012857-UIView-SW1) - This is an invaluable reference document which describes each component in UIKit and provides information about suggested and default behaviors. Parts of this document dive into technical details, but even if you ignore those sections, this reference provides a great outline of UIKit.

### Xcode and Interface Builder

Xcode is an application used to write apps for various Apple platforms. Interface Builder is a tool within Xcode which allows users to develop portions of an app visually, without having to write code. The screenshot below shows all of the UI elements available in Interface Builder.

[UI Objects](https://github.com/remypanicker/ios-ui-ux/blob/master/interface-builder-uikit.png)

### Points vs Pixels

Pixel density varies across devices. The tools used to develop apps expect specifications to be in points, thus design specs should be in points. But why points and not pixels? Here's an excerpt from Apple in the official [iOS Drawing Concepts Reference](https://developer.apple.com/library/ios/documentation/2DDrawing/Conceptual/DrawingPrintingiOS/GraphicsDrawingOverview/GraphicsDrawingOverview.html#//apple_ref/doc/uid/TP40010156-CH14-SW2)

> > **One point does not necessarily correspond to one physical pixel.**

> The purpose of using points (and the logical coordinate system) is to provide a consistent size of output that is device independent. For most purposes, the actual size of a point is irrelevant. The goal of points is to provide a relatively consistent scale that you can use in your code to specify the size and position of views and rendered content. How points are actually mapped to pixels is a detail that is handled by the system frameworks. For example, on a device with a high-resolution screen, a line that is one point wide may actually result in a line that is two physical pixels wide. The result is that if you draw the same content on two similar devices, with only one of them having a high-resolution screen, the content appears to be about the same size on both devices.

It's worth pointing out that design specs given in pixels should equate to whole (integer) point values. For example, an asset which is 201px x 201px @2x resolution, is equivalent to an asset which is 100.5pts x 100.5pts ... but we don't want this because now we are relying on subpixel rendering for the beautiful UI we have designed.

PaintCode has created an easy-to-digest infographic which depicts the conversion from points to pixels:

[The Ultimate Guide to iPhone Resolutions](http://www.paintcodeapp.com/news/ultimate-guide-to-iphone-resolutions)

[Designing at 1x](https://medium.com/shyp-design/design-at-1x-its-a-fact-249c5b896536#.mjwsur8e7)

### Auto Layout

Auto Layout is a constraint-based approach to design which allows you to build user interfaces that dynamically respond to both internal and external changes. App developers set up constraints such as fixed height/width, aspect ratio, leading/trailing/top/bottom spacing between elements, etc. In order for Auto Layout to figure out how to lay out a view, the system needs to be able to calculate an element's position in the x and y coordinate space as well as the element's height and width. Keeping this in mind will help you deliver design documents with enough specs for a developer to implement a fully adaptive user interface.

[Auto Layout Guide](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/AutolayoutPG) - The first section of this guide explains some high level concepts nicely.

[Adaptive User Interfaces](https://developer.apple.com/design/adaptivity)

### Assets

Apple officially announced support for vector based assets at [WWDC 2017 Session 201](https://developer.apple.com/videos/play/wwdc2017/201?time=2046) for users running Xcode 9+. Assets generated for iOS should be exported @1x in PDF format.

_If you are running an older version of Xcode, assets generated for iOS should be **pixel-specific** in PNG format. I know we just determined that design specs should be given in points, but PNGs are already rasterized unlike programatically created views which are rasterized at runtime. Thus assets must be pixel-specific. If your app is only supporting iOS 8+, then assets should be @2x and @3x resolution._ 

If you are supplying an asset which needs to be rendered with rounded corners, drop shadow, border, etc., those effects can be applied programatically. Whether or not you provide a raw asset or apply the effects before exporting the asset will vary depending on your use case. Apple provides some guidance about templated icon design in the [iOS Human Interface Guidelines: Icons](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/BarIcons.html).

#### Designing for iOS

[5 Things to Know When Designing for iOS](http://www.teehanlax.com/blog/5-things-to-know-when-designing-for-ios)

[Best Practices for Great iOS UI Design](https://developer.apple.com/videos/play/wwdc2013/225) - Kind of old, but still has some good info.

[Ivo Mynttinen Design - iOS Design Guidelines](http://iosdesign.ivomynttinen.com)

[5 Reasons Why Your Android App Should Not Mirror Your iOS App (And Vice Versa)](http://www.detroitlabs.com/blog/2015/10/28/5-reasons-you-dont-want-your-iphone-app-to-look-like-your-android-app) - ... Only 5 reasons?

[Designing for Both Android and iOS](http://webdesign.tutsplus.com/articles/a-tale-of-two-platforms-designing-for-both-android-and-ios--cms-23616)

#### Inspiration

[Mobile Design Patterns](http://pttrns.com)

[Mobile Empty States](http://emptystat.es/tagged/mobile)

## UX

[Thinking Like an App Designer](https://www.smashingmagazine.com/2015/04/thinking-like-an-app-designer)

[The Guide To UX Design Process & Documentation](https://speckyboy.com/2014/10/21/guide-ux-design-process-documentation-2)

### View States
[Mobile Views: The FIVE State Solution](http://scotthurff.com/posts/why-your-user-interface-is-awkward-youre-ignoring-the-ui-stack) - Informative article about how to consider each view in your app for a more informative user experience.

[Powers of 10: Time Scales in User Experience](https://www.nngroup.com/articles/powers-of-10-time-scales-in-ux) - This is a generic article which focuses on UX responsiveness on the web, but the underlying message definitely carries over to mobile.

### Prototyping

Creating a prototype is a powerful way to quickly iterate through ideas. Prototypes are also a low(er?) cost way to validate your UX and communicate complex interactions. 

[Prototyping - Fake It Till You Make It (WWDC 2014)](https://developer.apple.com/videos/play/wwdc2014/223/)

#### Prototyping Tools

[Deciding which prototyping tool to use](http://www.cooper.com/prototyping-tools)

###### My Quick List:

[Interface Builder](https://developer.apple.com/xcode/interface-builder)

[Flinto](https://www.flinto.com)

[InVision](https://www.invisionapp.com)

[Marvel](https://marvelapp.com/prototype-with-sketch/)

[Origami](https://facebook.github.io/origami/)

[Origami Studio](https://www.facebook.com/media/set/?set=a.606446952851229.1073741828.245766762252585&type=3) - Will be available for free late 2016.

## Deliverables

After reading up on best practices and designing a beautiful, native app, it's time to hand off your masterful work. There's lots of ways to deliver your work product to developers

Ideally your deliverables will adhere to the following guidelines:
- One source of truth. There will be **one**, easily **accessible** document which can be referenced for all UI/UX guidance.
- All assets will be exported as PDF files @1x resolution. Documentation should reference the exported assets by name. This will make it easier for other team members to easily find the correct asset when there are several assets being delivered.
- Storyboard/artboard depicting the user flow(s) to be developed.
- Explicit specs for font family, font weight, and font size in points.
- When providing specs for labels, it is helpful to provide additional details such as the number of lines and how to handle long text (truncate word, wrap text, scale font, etc.).
- Provide dimensions in points.
- Provide all relevant layout constraints (margins, spacing between elements, etc.) in points. Remember what we learned about Auto Layout.
- Specify colors used in designs specified as HEX or RGB, but pick one format and stay consistent. Similarly, don't forget to not any changes in alpha, otherwise it is assumed that alpha is 1.
- Provide prototypes, videos, descriptive diagrams to document and explain how animations and interactions should be implemented.
- Don't forget to include details about transitions and states (loading, refreshing, etc.)

It's best to provide as much detail as possible. Anything which is not explicitly defined will be left to the interpretation of the developer and/or operating system. _Example: You are designing a user profile. In your designs, the user's name is displayed in System Font, 17pt on one line. You provide specs and only include information about the text font. Now it is up to the developer to determine how a long name should be displayed. If the developer doesn't explicitly specify how to handle a long name, then the label will default to iOS' default handling of text overflow on a label. The lack of additional information has introduced two paths for deviation from your original design, and that's not even including Android, Web, etc. You have been thourough in your design, now it's time to make sure those details are accurately documented so that your hard work is not lost._

#### Automated Red Lining

[Zeplin](https://zeplin.io/features.html#designer)

[Sketch Measure](https://github.com/utom/sketch-measure)

[Markly](http://marklyapp.com)

[SpecKing](http://www.wuwacorp.com/specking)

[Slicy](http://macrabbit.com/slicy)

**Advanced asset delivery - proceed with caution**

If you want to take asset delivery to the next level, add the relevant assets to the Xcode project asset catalog and submit a pull request!

## Found an issue?
Open a [GitHub issue](https://github.com/remypanicker/ios-ui-ux/issues) with details so that it can get fixed!

## Contribute
Open a [pull request](https://github.com/remypanicker/ios-ui-ux/pulls) or contact me with suggestions to make this collection better.

## Contact
Feel free to reach out

Twitter: [@remypanicker](http://twitter.com/remypanicker)

Email: [rpanicke@gmail.com](mailto:rpanicke@gmail.com)
