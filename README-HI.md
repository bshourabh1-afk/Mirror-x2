# MirrorX – Android starter project

Yeh **v0.1.0 starter UI** hai, complete screen-mirroring app nahi.

## Is version mein
- Android Kotlin + Jetpack Compose project
- Wi-Fi, USB data aur HDMI mode selection UI
- Android 8.0+ minimum target
- GitHub Actions cloud build workflow

## Zaroori sachchai
- HDMI output tabhi chalega jab phone hardware DisplayPort Alt Mode ya compatible wired video output support kare.
- USB OTG support ka matlab yeh nahi ki TV USB port screen receiver ban jayega.
- Wi-Fi mirroring ke liye TV par compatible receiver/protocol implementation chahiye.
- Is starter mein abhi MediaProjection capture, video encoding, audio forwarding, WebRTC, USB streaming ya TV receiver implement nahi hain.

## Phone se APK build karne ka raasta
1. ZIP ko extract karo.
2. GitHub par naya repository banao aur extracted files upload karo.
3. Repository ke Actions tab mein `Build MirrorX APK` workflow run karo.
4. Workflow ke Artifacts section se `MirrorX-debug-apk` download karo.
5. ZIP extract karke `app-debug.apk` install karo.

Note: Cloud build workflow ko Gradle wrapper ki jagah installed Gradle command ki zaroorat hoti hai; agar runner par Gradle command available na ho, workflow ko Gradle setup action ke saath update karna hoga.
