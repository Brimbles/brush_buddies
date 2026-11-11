# Brush Buddies

A 30-second toothbrush timer for kids. Pick a buddy, tap **Start!**, and it dances to its own theme tune and does funny tricks at 10 and 20 seconds until brushing is done.

- 17 buddies, including Karl and Bjork the cats, a hobbit, a dinosaur, a unicorn, a dragon, a mermaid, a shark and a fairy
- Every buddy has its own original tune, synthesized in the browser with the Web Audio API (no audio files)
- Tap the buddy any time for a bonus trick
- The screen stays on while the timer runs

It is a single self-contained file: open `index.html` in a browser.

## Android app

Every change to `index.html` (or the `android/` folder) on `main` builds a new APK with GitHub Actions and publishes it under **Releases**.

To install on a phone:
1. Open the latest release on the phone (signed in to GitHub, since the repo is private) and download `BrushBuddies.apk`.
2. Open the downloaded file. Android will ask you to allow installing apps from your browser or Files app; allow it once.
3. Later builds install over the top as updates.

The app runs fully offline. The signing key (`android/app/brushbuddies.keystore`) is committed on purpose so every build is signed the same way and updates install cleanly; it is only for this family app, not for the Play Store.

Fonts: Lilita One and Nunito, bundled under the SIL Open Font License.
