
# React Native Projects Repository

This repository contains multiple React Native projects created using Expo. The first app pushed in this repository is `my-app`, which is a basic starter application built using the Expo CLI with a blank template.

---

## Project: `my-app`

This is a simple React Native app created using Expo. The purpose of this project is to set up the development environment and understand the basic folder structure and configuration of a React Native project using Expo.

---

## React Native + Expo App Setup Guide

### Step 1: Create a Project Folder
Choose a directory on your system where you want to create the project. You can use File Explorer or the terminal to create this folder.

```
mkdir React_Native_Practice
cd React_Native_Practice
```

### Step 2: Open Terminal
You can open:
- open folder with CMD (just type cmd in path bar and hit enter/click right click >cmd)
- Or open the folder in **VS Code** and use its **integrated terminal**

### Step 3: Create Your App Using Expo

```
npx create-expo-app my-app --template
```

#### Command Breakdown:
- `npx`: Runs the command using the latest version from the internet without installing globally.
- `create-expo-app`: CLI utility to create an Expo-based React Native app.
- A CLI is a text-based interface that lets you interact with your computer or tools by typing commands into a terminal or command prompt.

  ###### Common Uses of CLI
  - Creating projects (e.g., create-react-app, create-expo-app)
  - Running development servers (e.g., npm start, expo start)
  - Building apps (e.g., eas build)
  - Installing packages (e.g., npm install, yarn add) (https://github.com/kaushalgore/Understanding_Web_Setup/tree/main)
- `my-app`: This is **your project name**. You can change it to whatever name you prefer.
- `--template`: This flag allows you to select a specific template (e.g., blank, with TypeScript, etc.).

> We're using `--template` to select a **JavaScript-based blank template** to avoid unnecessary boilerplate code (like TypeScript setup).

---

### Step 4: Choose Template - Select "Blank"
When prompted, choose:
```
✔ Choose a template: › - Use arrow-keys. Return to submit.
❯   blank     a minimal app as clean as an empty canvas
```
Choosing the **Blank** template is recommended for beginners, as it gives you a clean slate to build your app from scratch, avoiding the complexity of additional dependencies or starter files.

---

### Step 5: Enter Your Project Directory

```
cd my-app
```

---

### Step 6: Install Additional Dependencies (if needed)

These are often required when setting up a React Native web version for the first time:

```
npm install react-dom@19.0.0
npm install react-native-web@^0.20.0
npm install @expo/metro-runtime@~5.0.4
npm install react-native-web --force
```

#### Why These Packages?
- `react-dom`: Required if you're planning to run your app in a browser using Expo web.
- `react-native-web`: Allows React Native components to be rendered on the web.
- `@expo/metro-runtime`: Helps with the runtime setup when using the Expo metro bundler.
- `--force`: Forces installation even if there are peer dependency warnings.

>  Note: These installations are **only needed once** (typically during your first setup).  
> You can install without specifying versions, but the mentioned versions are compatible with React Native 19 and Expo SDK 50+.

---

### Step 7: Start the App

```
npx expo start
```

This command launches the Expo development server. You'll see a QR code in the terminal which you can scan using the Expo Go app on your phone, or you can choose to run the app in an Android/iOS emulator or web browser.

---

## You're all set!

Your React Native environment is now ready. Explore the `my-app` project, make changes to `App.js`, and start building awesome mobile applications 🚀

---


# React Native Cleanup - Hello World App

This document provides steps to simplify your newly created React Native (Expo) project by removing unnecessary boilerplate and making the app minimal.

## Steps to Clean Up Boilerplate Code

- Delete the `assets` folder.
  - This folder usually contains images and icons provided by default in the Expo template.
  - For a basic "Hello World" app, this folder is not required.

- Update the `App.js` file with the following simplified code:

```js
import { Text, View } from 'react-native';

export default function App() {
  return (
    <View>
      <Text style={{fontSize:30}}>Hello React Native</Text>
    </View>
  );
}
```
## Final Outcome

- You will see a white screen with the message "Hello React Native" in large font.
- This is the minimal setup to get started and understand how a React Native app renders text on screen.


## Future Apps

## 🔗 Useful Links

- React Native Docs: https://reactnative.dev/
- Expo Documentation: https://docs.expo.dev/
- React Native Web: https://necolas.github.io/react-native-web/
