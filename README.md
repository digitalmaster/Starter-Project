Swift 3.0 Standard Project Template
===================

A standard project meant to help jumpstart any new Swift applications. Includes a number of common and/or useful dependencies. Updates will continue as dependencies improve/change. Feel free to propose any additions or thoughts. A linter is included to ensure all projects are kept up to code standards. 

----------
### Table of contents

[TOC]

----------

Project Initialization Steps
-------------


#### 1. Run Pod Install

Within the terminal, navigate to the project directory holding Podfile. Type command Pod Install

```
pod install
```
If you find that build times are very slow - you may want to comment out some pods that you arent using.


#### 2. Open Xcode Workspace

It is critical you open a workspace, as opposed to a project, in order for any dependencies to be loaded and run correctly


#### 3. Add Swiftlint Script

***Ignore if Swiftlint Script is already present*

After you have installed the included pods, and opened a workspace, add a new run build phase script to the project. Add the following script to run swiftlint upon project build.

```bash
"${PODS_ROOT}/SwiftLint/swiftlint"
```
Hint: Building project often will help catch linter mistakes more frequently, and allow for more consistent code.

#### 4. Dummy

After you have installed the included pods, and opened a workspace, add a new run build phase script to the project. Add the following script to run swiftlint upon project build.

```bash
"${PODS_ROOT}/SwiftLint/swiftlint"
```
Hint: Building project often will help catch linter mistakes more frequently, and allow for more consistent code.

----------


Included Dependencies
-------------------

A number of dependencies have been added as default to this project. They have been added using Cocoapods, and therefore can be referred to as "Pods" throughout this documentation. These were defined by a number of criteria, including (but not limited to) the following:
> **Dependency Criteria:**

> - Used commonly throughout projects to perform a common, straightforward task. Example: Alamofire simplifies HTTP Networking.
> - Consistently across the project would be lacking without defining ahead of time. This can include UI, Linter, Extensions, Etc. These are included and expected to be used (or attempted to be used) prior to any additional pods are added. Example: Material defines the UI and Animation Framework.
> - Multiple pods perform similar functions, albeit slightly differently. Decisions around these should be made early, and follow that protocol throughout. Example: Kingfisher performs a similar function to many pods, but for consistency, Kingfisher is used for all Image downloading and caching

All pods added have been confirmed to have sufficient documentation and are currently at a stable build. If you believe an update in required to the pods, see the Cocoapods Shortcuts section of this document for further information. Below is a short description and any necessary links for included Cocoapods:

 - Material 
 - SwiftyJSON
 - Alamofire
 - SwiftLint
 - SwiftIconFont
 - Kingfisher
 - Motion


#### **[Material](https://github.com/CosmicMind/Material)**

Material is an animation and graphics framework for Material Design in Swift. It is used due to its numerous components allowing for a slick and consistent flat, material design based approach. By using only one graphics framework, out of the box consistency can be achieved for projects, before you could create any custom UI components

#### **[SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON)**

SwiftyJSON makes it easy to deal with JSON data in Swift. By using this pod we can simplify any JSON work that is performed, greatly increasing development speed, while encouraging standardized frameworks for cross platform communication, resulting in fewer errors.

#### **[Alamofire](https://github.com/Alamofire/Alamofire)**

Alamofire is an HTTP networking library written in Swift. It simplifies networking requests and responses, and when combined with SwiftyJSON, can greatly simplify any standard server requests. This allows projects to get up and running quickly and efficiently.

In order to keep Alamofire focused specifically on core networking implementations, additional component libraries have been created by the [Alamofire Software Foundation](https://github.com/Alamofire/Foundation) to bring additional functionality to the Alamofire ecosystem.

- [AlamofireImage](https://github.com/Alamofire/AlamofireImage) - An image library including image response serializers, `UIImage` and `UIImageView` extensions, custom image filters, an auto-purging in-memory cache and a priority-based image downloading system.
- [AlamofireNetworkActivityIndicator](https://github.com/Alamofire/AlamofireNetworkActivityIndicator) - Controls the visibility of the network activity indicator on iOS using Alamofire. It contains configurable delay timers to help mitigate flicker and can support `URLSession` instances not managed by Alamofire.



#### **[SwiftLint](https://github.com/realm/SwiftLint)**
A tool to enforce Swift style and conventions, loosely based on GitHub's Swift Style Guide.

SwiftLint allows us to check style and conventions from the first line of code. This in turn allows errors and standards to be minimized, while still making code as readable as possible.

Swiftlint uses a specific file to define what rules are checked or not checked, as well as which directories are ignored. This file, ".swiftlint.yml", should be present to ensure that all standards are enforced across projects.

The SwiftLint documentation has a list of the rules that are standard within the linter, and an explanation for each, in case the in-line descriptions within Xcode are not sufficient.

#### **[SwiftIconFont](https://github.com/0x73/SwiftIconFont)**

Icons fonts for iOS (FontAwesome, Iconic, Ionicon, Octicon, Themify, MapIcon, MaterialIcon). Multiple icon fonts included - allows for quick and dirty icon creation through buttons as required. Use sparingly, as assets are preferred in a final product, but used correctly Icon Fonts can be very useful

#### **[Kingfisher](https://github.com/onevcat/Kingfisher)**

Kingfisher is a lightweight, pure-Swift library for downloading and caching images from the web. This project is heavily inspired by the popular SDWebImage. It provides you a chance to use a pure-Swift alternative in your next app. Simple enough.

#### **[Motion](https://github.com/CosmicMind/Motion)**

A library used to create beautiful animations and transitions for views, layers, and view controllers. http://cosmicmind.com. Motion is a tool used to create transition animations between view controllers. A strong animation framework when required, and works very well with Material. Other animation frameworks exist, so be aware when adding other animation dependencies.

#### **[PromiseKit](https://github.com/mxcl/PromiseKit)**

Promises simplify asynchronous programming, freeing you up to focus on the more important things. They are easy to learn, easy to master and result in clearer, more readable code. Allows for checking completion of async process, and run a callback or completion on finish. Greatly simplifies chaining of events and methods.

#### **[Fabric](https://get.fabric.io/)**

Fabric is a platform that helps your mobile team build better apps, understand your users, and grow apps. Fabric acts as a framework to use the following products (also included as pods):

- [Answers](https://answers.io/) - Part of Google Fabric, Answers is real-time mobile analytics that you don't need to analyze. It was created to make understanding your user base incredibly simple -- so you can spend your time building amazing experiences in your product, not digging through data.

- [Crashlytics](http://try.crashlytics.com/) - Part of Google Fabric, Crashlytics offers the most powerful, yet lightest weight crash reporting solution for iOS. Crashlytics also provides real-time analytics through Answers and app distributions to testers using Beta.


----------

CocoaPods Shortcuts
-------------------

Coming Soon...

Other Stuff
-------------------

Also Coming Soon.
