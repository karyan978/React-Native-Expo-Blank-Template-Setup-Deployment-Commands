

1️⃣ React Native + Expo (Blank Template) Setup & Deployment Commands
Step 1: Node.js aur Expo CLI install
# Node.js check
node -v
npm -v

# Expo CLI install globally
npm install -g expo-cli


Link: Expo CLI Install

Step 2: New Project Create (Blank Template)
# Folder banate hue project
expo init MyReactNativeApp

# Option choose karo:
# - blank (TypeScript or JavaScript)
cd MyReactNativeApp

Step 3: Start Development
expo start


Phone me dekhne ke liye QR code scan karein Expo Go app se.

Step 4: Run on Device / Emulator
# Android
npx expo run:android

# iOS
npx expo run:ios

Step 5: Install Required Packages
# Navigation
npm install @react-navigation/native
npm install react-native-screens react-native-safe-area-context
npm install @react-navigation/native-stack

# State management
npm install redux react-redux

# Firebase (agar Firebase backend use karna hai)
npm install firebase

Step 6: Build & Publish
# Build for Android
eas build --platform android

# Build for iOS
eas build --platform ios

# Install EAS CLI if not installed
npm install -g eas-cli

# Publish to Expo
expo publish


Link: Expo Deployment Guide

Step 7: Mobile Responsive

React Native me responsive ke tarike:

Flexbox - Row/Column, justifyContent, alignItems

Dimensions API - Dimensions.get('window').width ke through size adjust

Percentage width/height - width: '80%'

react-native-responsive-screen package

npm install react-native-responsive-screen


Platform-specific styling - Platform.OS === 'ios' ? ... : ...
