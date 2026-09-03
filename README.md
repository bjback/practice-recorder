# Practice Recorder v14

Sing against a learning track, record your voice, and compare your recording with your part.

See [USER_GUIDE.md](USER_GUIDE.md) for detailed, beginner-friendly instructions and troubleshooting.

## New in v14

- Uses WebKit's audio-session routing control, when available, to keep recording output on a connected wired or Bluetooth headset instead of the iPad speaker.
- Resets the audio session after recording so comparison returns to the normal high-quality headset route.

## Added in v13

- Returns to the basic microphone request because optional WebKit audio constraints caused silent recordings on the tested iPad.
- Displays the microphone name used by the browser.
- Checks the recorded waveform and warns when the browser captured little or no microphone sound.
- Explains how to set Reference to 0% to test the recorded voice by itself.

## Added in v11–v12

- Uses the most compatible default-microphone request for wired and Bluetooth inputs on iPadOS.
- Shows a specific explanation when browser permission, device availability, or the audio route prevents recording.
- Restores the controls after a failed start so the user can correct the problem and retry.

## Added in v10

- Both selected tracks are saved as local copies in this browser and restored automatically when you reopen the recorder.
- Loaded filenames are displayed prominently, with a **Change file** button for each track.
- **Forget saved files** removes the saved copies while keeping the loaded tracks usable for the current session.
- Microphone guidance now says **Allow microphone access when asked**, without specifying a browser.

## How to use

1. Connect earbuds or headphones to keep the learning track out of the microphone recording.
2. Choose the **Track to sing against**, usually your part-missing track.
3. Choose the **Track to compare with**, usually your solo or predominant-part track.
4. Use **Record from** to choose a starting point, then press **Record** and allow microphone access when asked.
5. Press **Stop**, then **Compare** to hear your voice alongside the reference track.
6. Adjust the voice and reference volumes, and use **Voice timing** to align them. Timing correction can be remembered on this device.

You can replay the same recording, pause/resume comparison, and move the playback slider. **Replay** starts comparison at the recording's original starting position. **Record Again** clears the current take so you can make another.

## Saved tracks and privacy

- Tracks are stored locally using IndexedDB; neither the selected tracks nor your microphone recording is uploaded by the recorder.
- Return using the same browser, device, and site address. Copies saved in the local HTML version do not transfer to the GitHub Pages version.
- The app saves copies, not links to the original files. If you edit an original, use **Change file** to load and save the updated version.
- Private browsing, clearing site data, or browser storage cleanup may remove saved tracks. Keep your original audio files.
- If saving fails, the loaded track can still be used for that session. A warning is shown; a previously saved track may return next time.
- **Forget saved files** does not delete your original audio files or your saved timing correction. Choose files again to save them for future sessions.
- Microphone recordings are held only for the current page session; they are not restored when you reopen the recorder.

## Update GitHub Pages

Upload both `index.html` and this `README.md` to the repository's root on `main`, replacing the existing files, and commit the changes. Keep the filenames unchanged. Once GitHub Pages finishes deploying, refresh the recorder and check that the heading says **prototype v14**.

`README_v9.md`, if retained in the repository, is historical documentation; this README describes the current version.
