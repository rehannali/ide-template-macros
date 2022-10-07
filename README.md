# IDETemplateMacros
This repo contains template macro for Xcode during file creation.

## Creating/Updating Macro File Using Terminal

1. `cd Location Directory` using terminal. For directories [Click Here](https://github.com/rehannali/ide-template-macros/edit/main/README.md#macro-file-locations).
2. Use `touch IDETemplateMacros.plist` for creating file `IDETemplateMacros.plist` using `touch` or open it if already present there.
3. Open file in your favorite editor. I'm using `VS Code`
4. You can use boilerplate code for plist file white creating File Headers.

## Creating/Updating Macro File Using Xcode

1. Open Xcode.
2. Create new file, the shortcut is CMD + N.
3. Scroll down to Resources files, and choose Property List.
4. Click Next, and give the filename IDETemplateMacros.plist.
5. Save it at the Desktop for now so we can easily find it.

### Customizing Property File

1. Open plist file you created earlier by double click on file. It'll open it in Xcode.
2. Highlight the first row named `root` and make sure it is dictionary type.
3. Click on "+" icon.
4. Select the newly created pair and type `FILEHEADER` as key and make sure the type of this row is `String`. If it is not, open dropdown and select `String`.
5. Open your favorite text editor and make your custom header or your can copy default from below or from directory mentioned below. I prefer to use VS Code.
6. Copy all of it and paste it next to `FILEHEADER` value you type earlier. It is okay if you see last line as there is only one line you can see.
7. Save the file and place it in you desired location as per your preference. For directories [Click Here](https://github.com/rehannali/ide-template-macros/edit/main/README.md#macro-file-locations).

## Macro File Locations

> Project - Single User :
`<YourProjectName>.xcodeproj/xcuserdata/[username].xcuserdatad/`

> Project - Shared by all users :
`<YourProjectName>.xcodeproj/xcshareddata/`

> Workspace - Single User :
`<YourWorkspaceName>.xcworkspace/xcuserdata/[username].xcuserdatad/`

> Workspace - Shared by all Users :
`<YourWorkspaceName>.xcworkspace/xcshareddata/`

> Global for Xcode :
`~/Library/Developer/Xcode/UserData/`

### Default Content For Macro File
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
<key>FILEHEADER</key>
<string>
// ___FILEBASENAME___.swift
// Project Name
// 
// 
// Created by ___FULLUSERNAME___ on ___DATE___ at ___TIME___.
// Copyright © ___YEAR___ Your Name or Company Name. All rights reserved.
// 
</string>
</dict>
</plist>
```

> ***If you want to use file, I have created some custom template inside `IDETemplateMacros` folder.
You can download it or copy paste content in mentioned directory file named `IDETemplateMacros.plist`.***

**NOTE**
In my example of default content, I used `___FILEBASENAME___`, `___FULLUSERNAME___`, `___DATE___`, `___TIME___` and `___YEAR___` macros. 
Apple provided other macros as well.

To see all of them, then [Click Here](https://help.apple.com/xcode/mac/current/#/dev7fe737ce0)
