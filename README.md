# Jarvis Calendar

A responsive, no-build personal calendar and homework dashboard for GitHub Pages. It uses plain HTML, CSS, and JavaScript.

## Run locally

Open `index.html` in a browser, or serve this folder with any static file server. Voice recognition generally requires HTTPS or localhost and microphone permission.

## Publish with GitHub Pages

1. Create a GitHub repository and add `index.html`, `styles.css`, `app.js`, and `README.md` to its root.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select your default branch and the `/ (root)` folder, then save.
4. Open the Pages URL shown in that settings panel.

No build step, account, API key, or server is needed.

## Data, profiles, and sharing

Jarvis stores each profile in that browser's local storage. Its profile ID appears in the URL as `?profile=...`, so you can bookmark a profile on that device. A URL alone cannot make a static GitHub Pages site synchronize private browser storage across devices.

Use **Profile & sharing → Copy share link** to make a link containing a snapshot of the profile at that moment. Anyone with that link can read the included calendar data. Later edits do not update a previously copied link. To transfer changes, make a fresh link or use **Export profile** on one device and **Import profile** on the other. Imported data is saved locally in that browser. Keep exported files and snapshot links private if their event details are personal.

The app starts with an empty calendar and never replaces existing browser data with sample content.

## Voice

Tap the microphone control once to enable listening, then allow microphone access and say “Hey Jarvis.” The browser's SpeechRecognition/Web Speech API support varies, and browsers may stop recognition in the background or require HTTPS. Jarvis restarts recognition when supported. A spoken summary button remains available when recognition is not supported. Voice listening is off until the user enables it.
