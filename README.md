# First Mobile App with Expo Router

This document outlines the process of scaffolding a mobile application using Expo Router and notes the behavior of the `reset-project` command.

---

### Project Scaffolding Steps

1.  **Navigate to Project Directory**: First, I used the terminal command `cd prodev-mobile-setup` to move into my chosen parent directory.
2.  **Initialize Project**: I ran `npx create-expo-app@latest .` to initialize a new Expo project. This command automatically sets up a new React Native app with the Expo Router template.
3.  **Modify Home Screen**: I edited the `app/(tabs)/index.tsx` file to change the welcome text. I located `Welcome!` and replaced it with **First App Created**.
4.  **Run Application**: I started the development server with `npx expo start`. This generated a QR code that I scanned with my phone's camera (iOS) or the Expo Go app (Android) to view the application on a physical device.

---

### Observations on `npm run reset-project`

Running `npm run reset-project` executes several key actions to clean the project environment:

-   It **deletes the `node_modules` directory** and the `package-lock.json` file, which removes all installed dependencies.
-   It **reinstalls the dependencies** based on the `package.json` file.
-   It **clears the Metro cache**, which can fix various development-related issues.

The primary effect of this command is to create a clean slate, ensuring all dependencies are in a known, working state, which is useful for troubleshooting or resolving installation conflicts.