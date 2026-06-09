# Karen AI Assistant

## Descriptions
- Android application powered by Tasker and Google Gemini AI
- Karen AI Assistant is a powerful Android AI Assistant which not only chats but also web search live information, automate tasks, productivity, and intelligent device interaction.

## Features
- Default Assistant Integration
- Dual AI Agents
- Voice & Text Chat
- Continue with or without You (Generate text with history without additional prompt)
- Screen Info (Requires this app to be set as default assistant app)
- Latest/Auto Screenshot
- Front/Rear/Latest Camera
- Supports any type Files but .dex and .exe file is unsupported
- Apps
  - Launch any apps (offline if app name (ignore case) or package name match)
  - Show all installed apps with "list" (ignore case)
  - Launch YouTube Music with song keywords (ignore case). Example: "youtube music i see stars running with scissors"
  - Launch a package name with a specific class name separated with slash "/". Example: com.google.android.apps.bard/com.google.android.apps.bard.shellapp.BardEntryPointActivity
  - Launch an app with the specific URL data separated with a comma ",". Example: tradingview,https://www.tradingview.com/symbols/BTCUSD/?exchange=CRYPTO&utm_source=androidapp&utm_medium=share
- Search Song Lyrics/Chords in currently played music
- Reads a URL content
- Web Search
- Add/update/delete calendar events
- Real time weather
- Create Image (Can create image without toggling to Create Image feature)
- Add Text to Image
- Modify AI Agents data
- User Personalization
- Multi languages
- Google Speech and ElevenLabs Speech
- Workspace (Does not allow root and cannot access outside of Karen_AI_Assistant/workspace/ directory)
- Java Code (Prompt to control device via java code automatically. Does not use root nor adb shell nor Shizuku nor Accessibility Service permission.)
- Accuracy of any mathematical calculations using Java Code (without toggling to Java Code feature)
- Read My Text (Just paste your copied text and it will be read directly with Speech)

## Advanced Features
These features can only be activated if WRITE_SECURE_SETTINGS permission is granted:
- Auto Screenshot without activating the Accessibility Service
- Screen Info without setting this app as default assistant app

You can grant WRITE_SECURE_SETTINGS permission via root in Termux/Terminal if your device is rooted:

`su -c pm grant android.permission.WRITE_SECURE_SETTINGS reiryuki.karenaiassistant`

Or just grant root to grant android.permission.WRITE_SECURE_SETTINGS automatically if it's asked at boot.

Or via adb shell:

`adb shell pm grant android.permission.WRITE_SECURE_SETTINGS reiryuki.karenaiassistant`

## Changelog

v4.6
- Change target SDK to 35 (yeah it bloats the app size significantly)
- Shows running tasks in Stop Process long press
- Add Latest Camera picture feature option
- Fix actions flow logic fault in Java Code task
- Fix bugs in math calculations
- Remove directory restrictions in Java Code

v4.5
- Process any math calculations via Java Code (without toggling to Java Code feature) for accuracy of results
- Fix Add Text to Image bugs
- Fix persistent bug at initialization
- Fix excluding mathematical calculation from Web Search
- Mentions battery level if it's lower than 21% and discharging
- Fix error handlings
- Change default Agents Data
- Improvements

v4.4
- Fix time zone in system instruction
- Add timestamp correction
- Fix error while adding files/image URI
- Improvements

v4.3
- Exclude mathematical calculations from Web Search
- Fix some unexpected responses
- Add switch Latest/Auto Screenshot in long press
- Fix persistent bug in Screen Info feature
- Fix Web Search Data text display
- Improvement in Settings pop up
- Add Notify trigger button
- Use root to force stop Google Speech automatically if possible
- Change Agents Data (add timestamp)

v4.2
- Support upload .sh file
- Fix search song lyrics/chords keywords bug
- Fix bug while sorting URLs
- Fix Tasker variables escape

v4.1
- Fix Screen Info feature bug
- Fix extracting file bugs
- Improvements

v4.0
- No files size limit (implementing Google Files API)
- Fix history changes not saved to KarenSave.txt
- Assistant request also triggers notification and quick access notifications
- Asks permission at boot if it fails to re-set default assistant
- Fix keywords in search song lyrics/chords feature
- Support multi users (using /storage/emulated/\<uid\>)
- Improvements

v3.9
- Fix persistent bug at initialization
- Prevent Agents from creating their own calendar events without being instructed to do so by user
- Redirect to online mode if offline mode is error in Apps feature

v3.8
- The Continue feature also has the ability to read URL content and Web Search if Agents want to use that
- Now you can change upload length limit in settings
- Voice Chat output maximum 3 results for better experience
- Fix workspace retry context
- Fix latest screenshot bug
- Fix wrong logic in upload files
- Fix other #ah bugs and typos

v3.7
- Add gemini-3.5-flash
- Only trigger Web Search if toggler is Nothing
- Merge some detections into one JSON format for efficiency
- Remove calendar event colour set because it does not affect the calendar app event colour
- Fix wind direction explanation
- Fix language in search song lyrics (without changing the lyrics language)
- Fix typo

## Screenshots
- https://t.me/ryukimodsscreenshots/117

## Requirements
- Android 8.1 (SDK 27) and up
- Create your own API key here first (it's free): https://aistudio.google.com/api-keys
- https://play.google.com/store/apps/details?id=com.google.android.tts

## Download Link & Instructions
- https://devuploads.com/1u1uw8icjw14
- In Android 13 and above, enable notification permission manually to get features from notification.
- Long press functions:
  - Files > Add/remove files
  - Add Text to Image > Add image
  - Screenshot > Latest/Auto
  - Keep Speech > System speech settings
  - Search Song > Lyrics/Chords
  - Continue > with You/without You
  - Stop Speech > Manual force stop Google Speech
  - Stop Process > Shows running tasks
  
## Troubleshootings
If you can't allow Notification Listener Service or Accessibility Service, try to uninstall the app and reinstall again.
If the issue still persist, try to search "Restricted Settings" in your Settings app and allow this app there.
But if you can't find it, then you can allow it via root access:
  
`su -c appops set reiryuki.karenaiassistant ACCESS_RESTRICTED_SETTINGS allow`
  
Or just grant the root access if it's asked in the app and it will run the line above automatically. 
  
Or run via adb shell:
  
`adb shell appops set reiryuki.karenaiassistant ACCESS_RESTRICTED_SETTINGS allow`
  

## Known Issues
- You need to re-set default assistant app (if you are using it) in every device boot. You can grant WRITE_SECURE_SETTINGS permission to fix that.
- Sometimes Google Speech is not stopping even if you have clicked Stop Speech button. To fix that, you can long press the Stop Speech to force stop Google Speech manually. If you are rooted, just grant root if it's asked, so you don't need to force stop manually.
- If error "javax.net.ssl.SSLPeerUnverifiedException: Hostname lite.duckduckgo.com not verified" is occur, that means it's blocked by your provider and you need to use DNS or VPN.

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and contributors
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this app/project here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


