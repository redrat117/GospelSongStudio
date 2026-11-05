# Gospel Song Studio (Android)

Create gospel worship songs (2 to 6 minutes) from an idea or from your own lyrics, plus everything YouTube needs:
3 viral titles, description, hashtags, 25 keywords, a 16:9 thumbnail and a ready-to-upload MP4.

All rights reserved Nji Nelson · redrat117@gmail.com

## What you need
- **Gemini API key** (free): https://aistudio.google.com/apikey — writes lyrics + YouTube text and paints the thumbnail background.
- **ElevenLabs API key** (paid plan with music): https://elevenlabs.io — turns the lyrics into the sung song.
  No ElevenLabs? Use **Copy for Suno**, make the song in Suno, then **Import audio**. The app still builds the video and package.

Paste both keys in the app under **Settings**, then tap **Save settings**.

## Build the APK (pick one)

### A. GitHub (no software needed)
1. Create a new repository on github.com and upload all files from this folder (keep the folder structure, including `.github`).
2. Open the **Actions** tab. The "Build APK" workflow runs on every upload (or press **Run workflow**).
3. When it turns green, open the run and download **GospelSongStudio-APK**. Unzip it and install `app-debug.apk` on your phone
   (allow "Install unknown apps" for your browser or Files app).

### B. Android Studio
Open this folder in Android Studio (Ladybug or newer), wait for Gradle sync, then **Build > Build APK(s)**.

## How to use
1. **Create** tab: choose *From an idea* or *From my lyrics*, pick language, style, vocals and length (2:00 to 6:00).
2. Tap **Create everything in 1 tap** (text → thumbnail → song → video), or do each step with its own button.
3. Every field has **Copy**, **Paste**, **Clear** and **Regenerate**, and you can type in all of them.
4. **Publish**: *Copy all* puts title + description + hashtags + tags on the clipboard. *Upload to YouTube* opens the YouTube app
   with the MP4 (the title is copied first). *Save everything* writes `video.mp4`, `thumbnail.png`, the song and
   `YouTube_package.txt` to `Download/GospelSongStudio/<song title>/`.
5. **Projects** tab keeps every song so you can reopen and edit it.

## Notes
- Model names can be changed in Settings if Google or ElevenLabs retire one.
- Song generation can take a few minutes for 5 to 6 minute songs. Keep the app open.
- The video is 1280x720, showing your thumbnail for the full song, encoded on the phone (no extra apps).
