# Hello World – React Native (Expo)

**Framework:** React Native with Expo

A simple React Native app that displays "Hello World!" on screen.

---

## Prerequisites

Install these before setting up the project:

| Tool | Version we used | Check with |
|------|-----------------|------------|
| Node.js | v24.15.0 | `node -v` |
| npm | 11.12.1 | `npm -v` |
| Git | 2.50.1 | `git --version` |
| Expo Go (phone app) | latest | App Store / Google Play |

> Your phone and computer must be on the **same Wi-Fi network** for Expo Go to connect.

---

## How This Project Was Created

```bash
npx create-expo-app@latest hello-world --template blank
cd hello-world
```

- `--template blank` creates a minimal project with a single `App.js` file.
- We then edited the `<Text>` component in `App.js` to display `Hello World!`.

---

## How to Run It (for the next team)

1. Clone the repo:
   ```bash
   git clone <your-repo-URL>
   cd hello-world
   ```
2. Install dependencies (the `node_modules` folder is not stored on GitHub):
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npx expo start
   ```
4. Open the **Expo Go** app on your phone and scan the QR code shown in the terminal.
   - Android: scan from inside Expo Go
   - iPhone: scan with the Camera app

Other options from the terminal after `npx expo start`:
- Press `a` to open an Android emulator (requires Android Studio)
- Press `w` to open in a web browser (may prompt you to install extra packages)

---

## Project Structure

```
hello-world/
├── App.js          # Main app component (the "Hello World!" screen)
├── app.json        # Expo configuration (app name, icon, etc.)
├── package.json    # Project dependencies and scripts
├── assets/         # Images and icons
└── README.md       # This file
```

---

## Troubleshooting

- **QR code won't connect:** Make sure the phone and computer are on the same Wi-Fi. If that doesn't work, try `npx expo start --tunnel`.
- **"Need to install the following packages" prompt:** Type `y` to continue.
- **Expo Go says the SDK version is incompatible:** Update Expo Go from the app store.

---
