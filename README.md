# Practice Recorder

A simple browser-based singing practice tool.

## What it does

1. Choose a **Sing Against** learning track, usually your part missing.
2. Put on earbuds or headphones.
3. Record yourself while the learning track plays.
4. Choose a **Compare With** track containing your own part.
5. Play your recording together with the reference track.
6. Adjust the timing if needed.
7. The timing correction can be remembered on that device/browser.

## Privacy

The recording stays in the browser. This prototype does not upload recordings to a server.

## GitHub Pages

This repository is ready for GitHub Pages because the app is named `index.html`.

After uploading the files to a GitHub repository:

1. Open the repository on GitHub.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the **main** branch and **/(root)** folder.
5. Click **Save**.

GitHub will provide an HTTPS address for the site.

## Mobile testing

For iPhone, open the GitHub Pages address in Safari and allow microphone access when prompted.

Connect earbuds before recording so the learning track does not play through the phone speaker and bleed into the microphone.

Wired earbuds will usually have lower latency than Bluetooth earbuds, but the app's timing correction can compensate for stable Bluetooth delay too.
