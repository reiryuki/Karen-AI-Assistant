# Karen AI Assistant

## Descriptions
- An app powered by Tasker
- Karen AI Assistant is a powerful Android AI Assistant which not only chats but also web search live information, automate tasks, productivity, and intelligent device interaction.

## Features
- Default Assistant
- 2 AI Agents
- Voice & Text Prompt
- Continue with or without You (Generate text with history without additional prompt)
- Screen Info (Requires this app to be set as default assistant app)
- Latest Screenshot
- Front & Rear camera
- Any Files
- Apps
  - Launch any apps (offline if app name (ignore case) or package name match)
  - Show all installed apps with "list" (ignore case)
  - Launch YouTube Music with song keywords (ignore case). Example: "youtube music i see stars running with scissors"
  - Launch a package name with a specific class name separated with slash "/". Example: com.google.android.apps.bard/com.google.android.apps.bard.shellapp.BardEntryPointActivity
  - Launch an app with the specific URL data separated with a comma ",". Example: tradingview,https://www.tradingview.com/symbols/BTCUSD/?exchange=CRYPTO&utm_source=androidapp&utm_medium=share
- Search Song Lyrics/Chords in currently played music
- Reads a URL content
- Web Search
- Weather
- Modify AI Agents data
- Multi languages
- Google Speech and ElevenLabs Speech
- Create Image (Tips for adding any text to the image, then edit the image using Java Code feature instead)
- Workspace (Does not allow root and cannot access outside of Karen_AI_Assistant/workspace/ directory)
- Java Code (Prompt to control device via java code automatically. Does not use root nor adb shell nor Shizuku nor accessibility service permission. Cannot access outside of Karen_AI_Assistant/workspace/ and Pictures/Karen AI Art/ directory.)
- Read My Text (Just paste your copied text and it will be read directly with Speech)

## Advanced Features
These features can only be activated if WRITE_SECURE_SETTINGS permission is granted:
- Auto screenshot without activating the accessibility service
- Screen Info without setting this app as default assistant app

You can grant WRITE_SECURE_SETTINGS permission via root in Termux/Terminal:

`su -c pm grant android.permission.WRITE_SECURE_SETTINGS reiryuki.karenaiassistant`

Or via adb shell:

`adb shell pm grant android.permission.WRITE_SECURE_SETTINGS reiryuki.karenaiassistant`

## Changelog

v2.9
- Change string alias of ElevenLabs Speech API Key (please re-set your API key if you're using it)
- Fix Run Shell
- Retry Run Shell and fixing errors max 3 times automatically
- Rename Run Shell to Workspace
- Remove Google News and fully using DuckDuckGo Search instead
- Reads another URL content if it's empty/error
- Does not show files list in Text Prompt
- Fix Files set after Create Image
- Forgot to tidy up landscape mode
- Forgot to set default model to the new gemini-3.1-flash-lite if it's not set
- Improvements

v2.8
- Encryption decryption API keys for security (you need to re-set your API keys)
- Add Search Song Lyrics/Chords feature
- Fix *prompt* and *dummy* word issue
- Separation of Settings UI
- Move Stop Process long press action to Stop Speech
- Fix bugs and improvements

v2.7
- Add a new model gemini-3.1-flash-lite
- Reads the content of a URL
- Adding Files in multi paths
- Allow Java Code to access Pictures/Karen AI Art/ directory
- Add options info in Voice Prompt dialog
- Log Offline Mode in KarenPrompt.txt if no require generate
- Fix dang bugs 😣

v2.6
- Add some new features in Apps feature
- Add skip screenshot dialog option
- Retry max 3 times and fix errors automatically in Java Code feature
- Change default agents data
- Add options info in Text Prompt dialog
- Fix upload files
- Fix other bugs and improvements

v2.5
- Tells AI the current battery level
- Fix bugs and improvements
- Change default agents data

v2.4
- Add Create Image feature
- Add Read My Text feature
- Backup deleted chats to /sdcard/Karen_AI_Assistant/Backups
- Update Java Code feature rules
- Remove unavailable model gemini-robotics-er-1.5-preview
- Fix bugs and improvements

v2.3
- API keys encoding format in the internal data
- Fix Web Search bugs
- Web Search OFF/ON/Deep button
- Add Stop Process button (You can long press to force stop Google Speech manually)
- Limit news length to 25000 characters
- Improve default agents data

v2.2
- Fix bugs and improvements
- Resume process if connection is available
- Add new model gemini-robotics-er-1.6-preview
- Google Speech unlimited length
- Add Deep Search feature
- Remove URL feature
- Add Advanced Features
- Change default agents data
- Remove Greet
- No longer log KarenWeather.txt & KarenScreenInfo.txt but KarenPrompt.txt instead

v2.1
- Add real time live Search
- Add Copy Text at notification feature
- Removes all error info before generates
- Removes /sdcard/Karen_AI_Assistant/.extract/\* before extracting new files
- Fix bugs and improvements

v2.0
- Supports xlsx file, zip, and any other else compressed files
- Independent Run Shell toggle
- No dialog confirmation on Java task
- Does not greet at boot
- Notification only on response
- Improvements
- Fix bugs

## Screenshots
- https://t.me/ryukimodsscreenshots/117

## Requirements
- Android 8.1 (SDK 27) and up
- Create your own API key here first (it's free): https://aistudio.google.com/api-keys
- https://play.google.com/store/apps/details?id=com.google.android.tts

## Download Link & Instructions
- https://devuploads.com/y54cst3sruca
- In Android 13 and above, enable notification permission manually to get features from notification.

## Known Issues
- You need to re-set default assistant app (if you are using it) in every device boot. You can grant WRITE_SECURE_SETTINGS permission to fix that.
- Sometimes Google Speech is not stopping even if you have clicked Stop Speech button. To fix that, you can long press the Stop Speech to force stop Google Speech manually.

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and contributors
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this app/project here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


