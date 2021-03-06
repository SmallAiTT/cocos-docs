We are happy to announce the release of:

* cocos2d-x v3.0-beta and cocos2d-x v2.2.2
* cocos2d-html5 v2.2.2
* CocoStudio v1.2


# cocos2d-x #

<img src="https://lh3.googleusercontent.com/-glwwzmFyUmk/UQgPnlx40uI/AAAAAAAArzg/WPRW10kkecM/s800/cocos2d-x-logo.png">

## v3.0beta ##

### Download ###

[cocos2d-x-3.0beta.zip](http://cdn.cocos2d-x.org/cocos2d-x-3.0beta.zip)

### Highlights ###

* New renderer. Renderer has being decoupled from the Scene Graph. It supports auto-batching and auto-culling.
* Added template containers. `cocos2d::Map<>`, `cocos2d::Vector<>`
* Label supports: `shadow`, `glow` and `outline` (beta)
* Added Joint support in the physics subsystem
* Added Console: A simple TCP console that lets you debug and inspect your game remotely
* `tools/project_creator/project_creator.py` includes a GUI to simplify the game creation process. It also allows you to create the game in any given directory.
* Added support to build Android's APK files in the `android-build.py` script
* Added `Scheduler::performFunctionInCocosThread()`. It supports executing a function in the cocos2d thread
* `Director` emits the following events using the `EventDispatcher`: `AFTER_UPDATE`, `AFTER_DRAW`, `AFTER_VISIT` and `PROJECTION_CHANGED`

### More information ###

Read more about all the new features at [cocos2d-x v3.0 release notes](http://www.cocos2d-x.org/projects/cocos2d-x/wiki/Release_Node_v300).


## V2.2.2 ##

### Download ###

[cocos2d-x-2.2.2.zip](http://cdn.cocos2d-x.org/cocos2d-x-2.2.2.zip)

### Highlights ###

* supports CocoStudio v1.2. It includes JS and Lua bindigns for CocoStudio
* WinPhone8 & Windows8: added XAML support, updated to latest version of ANGLE

# Cocos2d-html5 #

<img src="http://www.cocos2d-x.org/attachments/download/1508" height=180>

## Download

[Cocos2d-html5-v2.2.2.zip](http://cdn.cocos2d-x.org/Cocos2d-html5-v2.2.2.zip)

## Highlights


* Resolution policy now act as a combination of `cc.ContainerStrategy` and `cc.ContentStrategy` so that user can beautifully customize its behavior.
* cc.LabelTTF's now support perfectly automatic line break with occidental and Chinese characters.
* `cc.ClippingNode` for canvas render mode is implemented.
* Refactored cc.Node and cc.Sprite by adding cc._PointConst and cc._SizeConst for better Performance. Now the performance of setPosition and getPosition is `65% faster` than before.
* CCNode's setContentSize and setAnchorPoint support two types of parameters, more friendly and more efficient. setAnchorPoint(x,y) is `35% faster` than setAnchorPoint(cc.p(x,y)).
* Added `NPM` support and adjusted folder structure. It supports modules customization, the packaged mini engine and HelloWorld is just `185KB` in single file mode. Please visit [NPM Guide](http://www.cocos2d-x.org/wiki/Cocos-utils_for_NPM) for more details.
* Added SpriteFrameCache `JSON` format support.


## Note
Cocos2d-html5 will support new event dispatcher and new label in next release.  


### More information ###

Read more about all the new features at [Cocos2d-html5 v2.2.2 release notes](http://www.cocos2d-x.org/projects/cocos2d-x/wiki/Release_Notes_for_Cocos2d-html5_v222).

# CocoStudio #

<img src="http://upyun.cocimg.com/CocoStudio/Img/CocoStudio-Name-Logo.png" width=140>

## V1.2 ##

### download ###

[CocoStudio-1.2.0.0.exe](http://126.am/COCOSTUDIO1200FULL)

### Highlights ###

 * Added Japanese and Spanish localizations
 * Added the function: the scale and the reference line.
 * Added the function: export the unformatted Json when exporting the project.

#### Animation Editor ####

 * Improved the efficiency after several switching animation lists.
 * Drew the polygon collision : automatic image matching, profile tracing point, since the painting outline, etc.
 * Curve control easing up.
 * Added the shortcuts of the level adjustment.

#### UI Editor ####
 * Merged UI controls: Button and TextButton, TextArea and TextBox.
 * Added UI controls: ListView and PageView.
 * Added the function: Curve control easing up.
 * Modified the custom front settings in the text controls.
 * Modified the bugs in UI Editor.
   
#### Scene Editor ####
 * Added the Trigger setting.
 * Previewed Armature animation collision zone.
 * Set the simulator and the command line.
 * Download Scene Editor cloud optimized resources to support up to five devices simultaneously connected Scene Editor.
 * Download the open source scene editor Cloud Connector source code and the simulator source code.
 <https://github.com/chukong/CocoStudioConnector>
 
### Bugs fixed ###
 * Solved the problem when modifying the file name in the resource zone, it could not synchronize the modified file name to save the data.
 * Solved the problem when using the Plist to create a sequence Frame, resources were not displayed correctly.
 * Solved the problem when switching animation, mirroring reference was not set properly .
 * Solved the problem when modifying the properties in the properties area, it would cause multiple undo.
 * Solved the problem when input in the frame event , it would not be saved immediately.
