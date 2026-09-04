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

v6.0
- Add new models
- Data improvements

v5.9
- Add some new models
- Fix empty vars list in Apps feature if no disabled apps
- Fix malformed start time and end time calendar event
- Improvements

v5.8
- Fix dark mode while battery saver is on in AOSP
- Default Agents Data improvement
- Fix bugs

v5.7
- Exclude Web Search if user is asking for grammar check
- Default Agents Data: Fix inconsistent timestamp
- Math calculation and Java Code improvements

v5.6
- Fix Files data are deleted unexpectedly after processing mathematical calculation with Java Code
- Default Agents Data improvement

v5.5
- AI say thanks after the charger is connected in the next generate
- Default Agents Data: Fix persistent timestamp bug

v5.4
- Default Agents Data fix and improvement
- Internal prompts fix and efficiency
- Tells calendar info to AI before adding new event, not only while deleting and updating
- Force reupload files if previously uploaded files are not done yet

v5.3
- Fix force stop Speech if system Speech is not Google Speech
- System Speech speed and pitch is based on the default system settings
- Internal prompt improvements
- Default Agents Data improvement
- No longer restrict Web Search if toggler is Nothing only
- Turns off notify click monitor if not needed

v5.2
- Removes old web search data before generate
- Remove a useless ability in "Continue"
- Does not trigger Web Search if user ask to translate
- Default Agents Data impovement

v5.1
- Search Song:
  - Fix keywords
  - Exclude video/recording URLs

## Screenshots
- https://t.me/ryukimodsscreenshots/117

## Requirements
- Android 8.1 (SDK 27) and up
- Create your own API key here first (it's free): https://aistudio.google.com/api-keys
- System Speech. If your ROM doesn't have any system Speech then try to install this: https://github.com/reiryuki/Google-Text-to-Speech-Magisk-Module or https://play.google.com/store/apps/details?id=com.google.android.tts

## Download Link & Instructions
- https://bicolink.com/52k3
- In Android 13 and above, enable notification permission manually to get features from notification.
- Long press functions:
  - Files > Add/remove files
  - Add Text to Image > Add image
  - Screenshot > Latest/Auto
  - Camera > Rear/Front/Latest
  - Keep Speech > System speech settings
  - Search Song > Lyrics/Chords
  - Continue > with You/without You
  - Edit History > Focus ON/OFF
  - Stop Speech > Manual force stop Google Speech
  - Stop Process > Shows running tasks

## Download Tutorial
https://t.me/ryukinotes/97

## Troubleshootings
If you can't allow Notification Listener Service or Accessibility Service, try to uninstall the app and reinstall again.
If the issue still persists, try to search "Restricted Settings" in your Settings app and allow this app there.
But if you can't find it, then you can allow it via root access:
  
`su -c appops set reiryuki.karenaiassistant ACCESS_RESTRICTED_SETTINGS allow`
  
Or just grant the root access if it's asked in the app and it will run the line above automatically. 
  
Or run via adb shell:
  
`adb shell appops set reiryuki.karenaiassistant ACCESS_RESTRICTED_SETTINGS allow`
  

## Known Issues
- You need to re-set default assistant app (if you are using it) in every device boot. You can grant WRITE_SECURE_SETTINGS permission to fix that.
- Sometimes Google Speech is not stopping even if you have clicked Stop Speech button. To fix that, you can long press the Stop Speech to force stop Google Speech manually. If you are rooted, just grant root if it's asked, so you don't need to force stop manually.
- If error "javax.net.ssl.SSLPeerUnverifiedException: Hostname lite.duckduckgo.com not verified" occurs, that means it's blocked by your provider and you need to use DNS or VPN.
- If error "Queue full for IP:" in Create Image, it's likely the server temporary issue and not the application code error.

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and contributors
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this app/project here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


