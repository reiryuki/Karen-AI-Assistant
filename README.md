# Karen AI Assistant

## Descriptions
- An app powered by Tasker and Google Gemini AI
- Karen AI Assistant is a powerful Android AI Assistant which not only chats but also web search live information, automate tasks, productivity, and intelligent device interaction.

## Features
- Default Assistant Integration
- Dual AI Agents
- Voice & Text Chat
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
- Add/update/delete calendar events
- Weather
- Create Image (Can create image without toggling to Create Image feature)
- Add Text to Image
- Modify AI Agents data
- User Personalization
- Multi languages
- Google Speech and ElevenLabs Speech
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

v4.0
- No files size limit (implementing Google Files API)
- Fix history changes not saved to KarenSave.txt
- Assistant request also triggers notification and quick access notifications
- Asks permission at boot if it fails to re-set default assistant
- Fix keywords in search song lyrics/chords feature
- Support multi users (using /storage/emulated/<uid>)
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

v3.6
- Fix colour format while adding a calendar event
- Add calendar event does not return ID to prevent confusion
- Tells calendar info if needed only for efficiency
- Summarize old chat 20000 chars length
- Fix bugs in Apps feature and backup feature
- Fix typo
- Change default Agents Data

v3.5
- Fix wrong hours format in Calendar Event Start Time & Calendar Event End Time
- Summarize old chat 10000 chars length
- Limit 900000 characters length for files and URL content to prevent failure
- Does not trigger Web Search if Screen Info is ON
- Unknown errors handling
- Improvements

v3.4
- Add an ability to add/update/delete calendar events
- Add Calendar Name setting
- Fix Create Image errors
- Fix Web Search keywords
- Prevent upload files failure
- Fix other bugs & improvements

v3.3
- Can create image without toggling to Create Image feature
- Long press Keep Speech to go to system speech settings
- Fix read a URL content bugs
- Limit 1000000 characters length for read URL content to prevent failure

v3.2
- Fix Create Image crash in Android 16
- Add Text to Image enhancements
- Improvements

v3.1
- Add a new feature "Add Text to Image"
- Fix bugs

## Screenshots
- https://t.me/ryukimodsscreenshots/117

## Requirements
- Android 8.1 (SDK 27) and up
- Create your own API key here first (it's free): https://aistudio.google.com/api-keys
- https://play.google.com/store/apps/details?id=com.google.android.tts

## Download Link & Instructions
- https://devuploads.com/amzq5ntwi0ji
- In Android 13 and above, enable notification permission manually to get features from notification.
- Long press functions:
  - Files > add/remove files
  - Add Text to Image > add image
  - Keep Speech > system speech settings
  - Search Song > Lyrics/Chords
  - Continue > with You/without You
  - Stop Speech > manual force stop Google Speech

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


