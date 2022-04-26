# adaptive_icon_example

An Android example App project that shows how to check adaptive icons fit the official guidelines.<br/>
    <img src="/images/screenshots/Adaptive_icon-squire.png" width="24%"/>
    <img src="/images/screenshots/Adaptive_icon-circle.png" width="24%"/>
    <img src="/images/screenshots/Adaptive_icon-rounded_corners.png" width="24%"/>
    <img src="/images/screenshots/Adaptive_icon-squircle.png" width="24%"/>

## How to create adaptive launcher icons?

 1. Choose a vector image design tool which can export SVG formot file (eg. [Illustrator](https://helpx.adobe.com/tw/illustrator/how-to/export-svg.html), [Adobe XD](https://helpx.adobe.com/tw/xd/help/export-design-assets.html), [Affinity](https://designbundles.net/design-school/how-to-make-an-svg-in-affinity-designer), [Sketch](https://www.sketch.com/docs/importing-and-exporting/#how-to-export-css-and-svg-code)).
 1. Create a canvas with width and height 108px. If it's too small, you can create a 10x canvas.
 1. Create a top layer. Import adaptive icon mask lines to ensure safe area.
 1. Craete a background layer and then draw background.
 1. Create a foreground layer and then draw foreground. 
 1. Export foreground and background SVG files. Note, if 
 1. In Android Studio, create new Vector Assets. Convert foreground and background SVG files to Vector Drawable format files. <br/>
    <img src="/images/screenshots/Vector_Asset_Studio.png" width="70%"/>
 1. In Android Studio, create new Image Asset. Choose Icon Type="Launcher Icons(Adaptive and legacy)". Choose source assets for foreground and background layers.<br/>
    <img src="/images/screenshots/Image_Asset_Studio.png" width="70%"/>

## Which icon shows in which target? 
 - Android 8 (API 26, O) or above :   Adaptive launcher icons in mipmap-anydpi-v26 folder.
 - Android 7.1.1 (API 25, N_MR1)  :   android:roundIcon and android:icon in mipmap folders. 
 - Android 7 (API 24, N) or below :   android:icon in mipmap folders.

## Dev env

 - macOS 12.2.1 (Monterey) x64
 - Android Studio Bumblebee Patch 2
 - Android SDK version 32
 - JDK: 11
 - Gradle: 7.2
 - Kotlin: 1.6.10

 ## References

 - [Android 如何設計使用 Adaptive Icon](https://wm4n.github.io/Android-%E5%A6%82%E4%BD%95%E8%A8%AD%E8%A8%88%E4%BD%BF%E7%94%A8-Adaptive-Icon/)
 - [Adaptive icons](https://developer.android.com/guide/practices/ui_guidelines/icon_design_adaptive)
 - [Create app icons with Image Asset Studio](https://developer.android.com/studio/write/image-asset-studio#create-adaptive)
 - [Add multi-density vector graphics](https://developer.android.com/studio/write/vector-asset-studio)
 - [Designing Adaptive Icons](https://medium.com/google-design/designing-adaptive-icons-515af294c783)
   - You can find some design tool templates here.


 ## Todos

 - Find a easier way to launch Vector Assets Studio and Image Asset Studio for designers.<br/>
   Since there is no standalone Vector Assets Studio and Image Asset Studio program.
