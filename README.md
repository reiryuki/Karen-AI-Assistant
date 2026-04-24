# Karen AI Assistant

## Descriptions
An app powered by Tasker

## Features
- Device Assistant
- 2 AI Agents
- Voice & text prompt
- Continue with or without you (Generate text with history without additional prompt)
- Screen Info
- Screenshot
- Front & rear camera
- Any files
- Previous files
- Modify AI Agents data
- Launch apps & URL
- Multi language
- Text to speech
- Real time, date, zone, weather, search, & news
- Run shell (Does not allow root and cannot access outside of Karen_AI_Assistant/workspace/ folder)
- Java (Prompt to control device via java code automatically. Does not use root nor adb shell nor Shizuku nor accessibility service permission. Cannot access outside of Karen_AI_Assistant/workspace/ folder.)
- Java uses an additional input prompt of about 50 KiB, so it might use up your quota faster.

## Changelog

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

v1.4
- Fix bugs & UI improvements
- Offline detection
- Auto resolve model
- Dark/light theme
- Re-Speech toggle (long press on Stop Speech)

v1.3
- New icon
- Launch animation
- UI improvements
- System TTS does not read character name at the beginning of each paragraph
- Resizeable text
- Fix bugs

v1.2
- New better UI
- Rename feature Agent to Java
- Add "Data 2" for one more AI Agent
- Add "Agent Auto", "Agent 1", "Agent 2", & "Agent Random" to control response between them
- Add "Continue" to generate with history without additional prompt
- Add "User Name" to change your name
- Add "User Personality" to describe who you are
- Add "Previous Files" to re-upload your files that you uploaded previously
- Fix bugs

## Screenshots
https://t.me/ryukimodsscreenshots/77

## Requirements
- Android 8.1 (SDK 27) and up
- Create your own API key here first (it's free): https://aistudio.google.com/api-keys
- https://play.google.com/store/apps/details?id=com.google.android.tts

## Download Link & Instructions
- https://devuploads.com/9xtq7m0hsyvy
- If you installed app v1.2 or below, then uninstall it first before installing app v1.3 or above.
- In Android 13 and above, enable notification permission manually to get features from notification.

## Known Issue
You need to re-set default assistant app (if you are using it) in every device boot. You can grant WRITE_SECURE_SETTINGS via root to fix that:

`su -c pm grant android.permission.WRITE_SECURE_SETTINGS reiryuki.karenaissistant`

Or via adb shell:

`adb shell pm grant android.permission.WRITE_SECURE_SETTINGS reiryuki.karenaissistant`

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and contributors
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this app/project here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


