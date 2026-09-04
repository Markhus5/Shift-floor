# Shift Floor

A single-page shop-floor tablet app: workers check in/out of tasks, a manager
dashboard shows live yield and fault-rate stats. Static HTML/CSS/JS, backed by
Firebase Firestore for shared state across devices.

## Setup

1. **Firebase config** — edit `firebase-config.js` with your real Firebase
   project's web app config (Firebase Console → Project Settings → General →
   Your apps → Web app). Until this is filled in, the app runs standalone
   with no cross-device sync.
2. **Firestore rules** — paste the rules from `FIRESTORE_RULES.txt` into
   Firebase Console → Firestore Database → Rules. This app has no Firebase
   Auth; it's PIN-gated only at the app level, so the rules intentionally
   allow open read/write to its one data document.
3. **GitHub Pages** — push these files to a GitHub repo, then enable
   Settings → Pages → deploy from the branch containing them, to get a
   public URL.

Fuller walkthrough given separately in chat.
