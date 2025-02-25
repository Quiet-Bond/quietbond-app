# QuietBond - Dating App for Demisexuals and Sapiosexuals

Welcome to QuietBond, a React Native mobile application designed for demisexuals and sapiosexuals seeking meaningful, trust-based friendships and connections. Inspired by the nostalgia of 1990s text-based MUDs and 1980s pen-pal exchanges, QuietBond offers a minimalist, cozy, and intellectual experience.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview
QuietBond is a mobile app built with React Native and Expo, using Firebase for real-time data and authentication. It prioritizes deep emotional and intellectual connections, featuring screens like Welcome, Login, Signup, Home, Prompt, and Chat. The app de-emphasizes photos, preferring custom art and avatars to create a unique and authentic user experience.

## Features
- **Text-First Connections**: No photos initially—users connect through thoughtful prompts and bios, echoing MUDs and pen-pal letters.  
- **Abstract Avatars**: Customizable geometric shapes (e.g., hearts, loops) in muted blues and greens.  
- **Daily Matches**: Curated, trust-based matches based on connection style quizzes.  
- **Prompt-Driven Chats**: Mutual prompts unlock conversations, fostering slow, meaningful interactions.
- **Photo Unlock**: Photos can be unlocked once sufficient trust has been established. 
- **Watercolor Glitch Aesthetic**: Cozy, intellectual design with digital glitch effects for a modern MUD vibe.  
- **Accessibility**: High-contrast, screen-reader-compatible UI for inclusive use.

## Getting Started
Clone this repository and follow the instructions below to set up and run QuietBond locally.

## Prerequisites
- Node.js (v16 or later)
- npm or Yarn
- Expo CLI (install via `npm install -g expo-cli` or `yarn global add expo-cli`)
- Android Studio or Xcode (for mobile emulators/simulators)
- Firebase account (for authentication and Firestore setup)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/quietbond-app.git
   cd quietbond-app
   ```
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```
3. Set up Firebase:
   - Create a Firebase project at [firebase.google.com](https://firebase.google.com).
   - Enable Authentication (Email/Password) and Firestore in Firebase Console.
   - Download `google-services.json` (Android) and `GoogleService-Info.plist` (iOS), place them in `android/app/` and `ios/QuietBond/` respectively.
   - Create a `.env` file in the root directory with:
     ```env
     EXPO_PUBLIC_FIREBASE_API_KEY=your-api-key
     EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=your-auth-domain
     EXPO_PUBLIC_FIREBASE_PROJECT_ID=your-project-id
     EXPO_PUBLIC_FIREBASE_STORAGE_BUCKET=your-storage-bucket
     EXPO_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your-sender-id
     EXPO_PUBLIC_FIREBASE_APP_ID=your-app-id
     ```
   - Install Firebase dependencies:
     ```bash
     npm install @react-native-firebase/app @react-native-firebase/auth @react-native-firebase/firestore
     ```
4. Install Expo dependencies:
   ```bash
   npx expo install react-native-svg react-native-linear-gradient
   ```

## Usage
1. Start the Expo development server:
   ```bash
   npx expo start
   ```
2. Open the app in:
   - **Expo Go** on a physical device (scan QR code).
   - **Android Emulator** (via Android Studio).
   - **iOS Simulator** (via Xcode).
3. Navigate through screens: Welcome → Login/Signup → Home → Prompt → Chat to experience QuietBond’s flow.

## Project Structure
```
quietbond-app/
├── .github/                  # GitHub workflows (CI/CD pipeline)
├── android/                  # Android-specific files
├── ios/                      # iOS-specific files
├── src/
│   ├── screens/              # Screen components (WelcomeScreen.js, LoginScreen.js, etc.)
│   ├── components/           # Reusable UI components (MatchCard.js, ConnectionQuiz.js, etc.)
│   ├── navigation/           # Navigation setup (StackNavigator.js, BottomTabNavigator.js)
│   ├── styles/               # CSS-in-JS styles (WelcomeStyles.js, LoginStyles.js, etc.)
│   ├── utils/                # Utility functions (api.js, constants.js)
│   └── assets/               # Static assets (logo/, avatars/, icons/)
├── App.js                    # App entry point
├── package.json              # Project dependencies and scripts
├── .gitignore                # Ignore node_modules, build files, etc.
├── README.md                 # This file
└── .env                      # Environment variables (Firebase config)
```

## Contributing
1. Fork this repository.
2. Create a feature branch (`git checkout -b feature/your-feature`).
3. Commit changes with clear messages (e.g., `git commit -m "Add PromptScreen component"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request against the `develop` branch, following the CI/CD pipeline checks.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
- **Author**: [Your Name or GitHub Username]  
- **Email**: your.email@example.com  
- **GitHub**: [github.com/your-username](https://github.com/your-username)  
- **Project Link**: [github.com/your-username/quietbond-app](https://github.com/your-username/quietbond-app)

Feel free to reach out with questions, feedback, or collaboration ideas!
```
<!-- Notes for You:
- **Customization**: Replace placeholders like `your-username`, `your-email@example.com`, and Firebase credentials with your details. Update the license if you prefer a different one (e.g., Apache, GPL).  
- **Firebase Setup**: Ensure `google-services.json` and `GoogleService-Info.plist` are added, and `.env` is gitignored (update `.gitignore` if needed).  
- **CI/CD Reference**: Mentions the `.github/workflows/` directory—ensure your CI/CD pipeline (from “Suggest a CI/CD pipeline”) is set up and referenced here.  
- **Markdown Formatting**: Use headers (`#`, `##`), lists, code blocks (```), and links for readability on GitHub.  
- **Expansion**: Add sections like “Screenshots” (link to Figma prototypes or app images), “Roadmap” (future features), or “Acknowledgements” (tools like Figma, Expo) as the project grows.  
-->

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/quietbond-app.git
   cd quietbond-app
