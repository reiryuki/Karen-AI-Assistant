# Karen AI Assistant

## Descriptions
- An app powered by Tasker
- Karen AI Assistant is an Android AI Assistant that can chat, search live information, help operate your device, and automate tasks.

## Features
- Default Assistant
- 2 AI Agents
- Voice & Text Prompt
- Continue with or without You (Generate text with history without additional prompt)
- Screen Info (Requires this app to be set as default assistant app)
- Latest Screenshot
- Front & Rear camera
- Any Files
- Previous Files (Re-use previously uploaded files)
- Modify AI Agents data
- Launch any Apps
- Multi languages
- Google Speech and ElevenLabs Speech
- Real time, date, time zone, and weather.
- Web Search & News
- Web Deep Search (Reads the entire articles from the top 3 links of live search, adding up to 300 KiB of input, so it might use up your quota faster.)
- Create Image (Tips for adding any text to the image, then edit the image using Java Code feature instead)
- Run Shell (Does not allow root and cannot access outside of Karen_AI_Assistant/workspace/ folder)
- Java Code (Prompt to control device via java code automatically. Does not use root nor adb shell nor Shizuku nor accessibility service permission. Cannot access outside of Karen_AI_Assistant/workspace/ folder.)
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

v2.4
- Add Create Image feature
- Add Read My Text feature
- Backup deleted chats to /sdcard/Karen_AI_Assistant/Backups
- Update Java Code feature rules
- Remove unavailable model gemini-robotics-er-1.5-preview
- Fix bugs and improvements

v2.3
- API keys encoding format in the internal data for security
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

v1.9
- Fix default data
- Fix weather

v1.8
- Continue with or without you
- Greetings at device boot
- Run shell ability (It does not allow root and cannot access outside of Karen_AI_Assistant/workspace/ folder)

v1.7
- Fix text size fit mode
- Fix crash
- Improvement

v1.6
- Fix bugs and improvements

v1.5
- Add notify quick access
- Changeable notify text character limit
- No longer read write API keys to internal storage
- Fix bugs

## Screenshots
- https://t.me/ryukimodsscreenshots/77
- https://t.me/ryukimodsscreenshots/116

## Requirements
- Android 8.1 (SDK 27) and up
- Create your own API key here first (it's free): https://aistudio.google.com/api-keys
- https://play.google.com/store/apps/details?id=com.google.android.tts

## Download Link & Instructions
- https://devuploads.com/hz3lysyxc5dq
- In Android 13 and above, enable notification permission manually to get features from notification.

## Known Issues
- You need to re-set default assistant app (if you are using it) in every device boot. You can grant WRITE_SECURE_SETTINGS permission to fix that.
- Sometimes Google Speech is not stopping even you have clicked Stop Speech button. To fix that, you can long press Stop Process button to force stop Google Speech manually.

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and contributors
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this app/project here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


