# AI Video Sharing App

This project is a modern React Native mobile application that serves as a social video sharing platform with AI integration. Built using Expo and React Native, it allows users to create, upload, and share video content with AI-generated prompts, creating an engaging community-driven video experience.

## What This Project Is About

The project is designed as a TikTok-like video sharing platform where users can:

- **Create and Share Videos**: Upload video content with custom titles and AI-generated prompts
- **Discover Content**: Browse through a feed of videos from other users with trending and latest content sections
- **Search Functionality**: Find specific videos using the built-in search feature
- **User Authentication**: Secure sign-up and sign-in system with user profiles
- **Social Features**: View creator profiles, avatars, and video metadata

## Technology Stack

### Frontend Framework
- **React Native**: Cross-platform mobile development framework
- **Expo**: Development platform and toolchain for React Native apps
- **Expo Router**: File-based routing system for navigation
- **NativeWind**: Tailwind CSS for React Native styling

### Backend & Database
- **Appwrite**: Backend-as-a-Service (BaaS) platform providing:
  - User authentication and account management
  - Cloud database for storing user and video data
  - File storage for video and thumbnail uploads
  - Real-time data synchronization

### Key Dependencies
- **expo-av**: Video playback and media handling
- **expo-document-picker**: File selection for video and image uploads
- **react-native-appwrite**: Appwrite SDK integration
- **react-native-animatable**: Smooth animations and transitions
- **react-native-reanimated**: Advanced animations
- **react-native-gesture-handler**: Touch gesture handling

## How It Achieves Its Goals

### 1. **Video Content Management**
The app uses Appwrite's cloud storage to handle video uploads and thumbnails. When users create content:
- Videos and thumbnails are uploaded to Appwrite Storage
- Metadata (title, prompt, creator info) is stored in Appwrite Database
- File URLs are generated for efficient content delivery

### 2. **User Authentication & Profiles**
- Implements secure email/password authentication through Appwrite
- Generates user avatars automatically using initials
- Maintains user sessions and profile data across app sessions
- Global context management for user state

### 3. **Content Discovery**
- **Home Feed**: Displays all videos with pull-to-refresh functionality
- **Trending Section**: Shows latest 7 videos in a horizontal scrollable format
- **Search**: Full-text search across video titles using Appwrite's query system
- **Video Cards**: Interactive video previews with play/pause functionality

### 4. **Modern UI/UX**
- **Custom Components**: Reusable UI components (VideoCard, FormField, CustomButton, etc.)
- **Responsive Design**: Adapts to different screen sizes using SafeAreaView
- **Smooth Animations**: Video transitions and loading states
- **Dark Theme**: Consistent dark color scheme throughout the app

### 5. **Navigation & Routing**
- **Tab-based Navigation**: Home, Create, Bookmark, Profile tabs
- **Stack Navigation**: Authentication flow and search results
- **File-based Routing**: Expo Router for intuitive navigation structure

### 6. **AI Integration**
The app includes AI prompt functionality where users can:
- Add AI-generated prompts to their video content
- Store and display AI context alongside video metadata
- Create a unique content categorization system

## App Architecture

The application follows a clean, modular architecture:

- **`/app`**: Main application screens with file-based routing
- **`/components`**: Reusable UI components
- **`/lib`**: Backend integration and utility functions
- **`/context`**: Global state management
- **`/constants`**: App-wide constants and asset references
- **`/assets`**: Images, fonts, and static resources

## Key Features

- **Video Upload**: Support for MP4 and GIF video formats
- **Thumbnail Generation**: Custom thumbnail upload for video previews
- **Real-time Updates**: Pull-to-refresh and automatic content updates
- **Cross-platform**: Runs on both iOS and Android
- **Offline Support**: Cached content and graceful error handling
- **Responsive Design**: Optimized for various device sizes

Aora represents a complete social video sharing ecosystem, combining modern mobile development practices with cloud-based backend services to create an engaging user experience for content creators and viewers alike.
