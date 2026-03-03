# PaperMaker – Flutter Wallpaper Browser App

PaperMaker is a Flutter-based wallpaper browsing application that fetches curated wallpapers from the Pexels API and displays them in a clean grid layout. The project focuses on API integration, JSON parsing, and responsive UI development using Flutter.

This app was built as a portfolio project to demonstrate mobile development fundamentals and REST API integration.

---

## Features

- Fetches curated wallpapers from the Pexels API
- Displays wallpapers in a responsive grid layout
- Horizontal category selection (Vectors, Abstract, Space, Computer, Nature)
- Dynamic network image rendering
- Structured Flutter project supporting Android, iOS, and Web

---

## Tech Stack

- Flutter (Dart)
- HTTP package for API requests
- Pexels REST API
- JSON parsing
- Material Design components

---

## Project Structure

```
lib/
│
├── main.dart              # Application entry point
├── home.dart              # Home screen UI and API integration
├── getter.dart            # API key loader
├── model/                 # Data models
├── widget/                # UI components (grid layout)
│
asset/                     # Images and static assets
android/                   # Android platform files
ios/                       # iOS platform files
web/                       # Web platform files
```

---

## Getting Started

### Prerequisites

- Flutter SDK installed
- A free Pexels account
- A valid Pexels API key

---

### API Key Setup

The app sends an Authorization header when making requests to the Pexels API.

Add your API key in the request header (for example inside `getter.dart`):

```dart
headers: {
  "Authorization": "YOUR_PEXELS_API_KEY"
}
```

For better security, consider using environment variables or secure storage instead of hardcoding the key.

---

### Run the Project

```
flutter pub get
flutter run
```

---

## How It Works

1. The home screen sends a request to the Pexels curated endpoint.
2. The JSON response is parsed into a data model.
3. The app dynamically builds a GridView using the returned image URLs.
4. Categories allow users to explore different wallpaper types.

---

## Purpose of the Project

This project was created to:

- Practice API integration in Flutter
- Implement dynamic UI rendering
- Work with structured project architecture
- Demonstrate understanding of REST APIs and mobile app design

---

## Future Improvements

- Implement search functionality
- Add a wallpaper detail screen
- Add download or save capability
- Add pagination (load more results)
- Improve API key security handling
- Add dark mode support

---

## Author

Developed as a portfolio project to demonstrate Flutter development and API integration skills.
