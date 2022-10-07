# IDETemplateMacros
This repo contains template macro for Xcode during file creation.

## Creating/Updating Macro File

1. `cd Location Directory` using terminal. For directories [Click Here](https://github.com/rehannali/ide-template-macros/edit/main/README.md#macro-file-locations).
2. Use `touch IDETemplateMacros.plist` for creating file `IDETemplateMacros.plist` using `touch` or open it if already present there.
3. Open file in your favorite editor. I'm using `VS Code`
4. You can use boilerplate code for plist file white creating File Headers.

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
