# deprecated
Themes moved to the main [repository](https://github.com/AnySoftKeyboard/AnySoftKeyboard/tree/master/addons/themes).

Theme
=====

A keyboard theme pack for AnySoftKeyboard.

This is an example of an AnySoftKeyboard Theme. Please follow the TODO list to create your own:

To-Do:
------
- Change package name in _AndroidManifest.xml_
- Change the package (and folder name) of the Java class _KeyboardThemeReceiver.java_
- Change the App name, theme name and description at _/values/strings.xml_
- Generate a new [GUID](http://www.guidgenerator.com/), and update the _id_ attribute at */xml/keyboard_themes.xml*
- Change the *ic_launcher* to your liking.

This was the easy part, mostly administration. Now, to the hard part - assets, dimensions, etc.
The example (master) branch has the basic plumbing. I would suggest **deleting** all drawables which are not in the _drawable_ folder (e.i., _drawable-mdpi_, _drawable-hdpi_, etc), and add your own assets instead. This will ensure that you have all the required assets - the build will fail until all minimum assets are there.

Flow the _ExampleAnyKeyboardTheme_ style (at _/values/styles.xml_) to fill the assets and dimensions for the layout. Notable mentions:
- Add normal key assets: */drawable/btn_keyboard_key.xml*
- Add popup keyboard key assets: */drawable/btn_keyboard_key_popup.xml*
- Add key-feedback assets: */drawable/keyboard_key_feedback.xml*
 
And the _ExampleAnyKeyboardPopupTheme_ style.

Follow the ExampleAnyKeyboardIconsTheme style (at _/values/styles.xml_) to fill the assets for the icons. Notable mentions:
- Add _Action_ key assets: */drawable/key_action_set.xml*
- Add _Shift_ key assets: */drawable/key_action_set.xml*
- Add _Delete_ key assets: */drawable/key_action_set.xml*
- Etc.

When all is done, you can try to build your project:
```gradle clean build```

Install the APK on your device: 
```gradle installDebug```

And test it. If you feel fine with that, take a screenshot:
- Take a screenshot, and copy it to */drawable-nodpi/theme_screen_shot.png*. Don't forget to crop the screenshot to include only your layout (and not the entire screen).

**GOOD LUCK**

License
-------

    Copyright 2013 Menny Even-Danan
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
    

