# 📝 Notes App

A beautiful and feature-rich notes application built with Android, Kotlin, and Room database.

## ✨ Features
- Create, edit, and delete notes
- Search notes instantly
- Pin important notes
- Color-code notes for organization
- Sort by date, title, or last modified
- Dark mode support
- Export notes to text file
- No internet required - works offline

## 🛠️ Tech Stack
- **Language:** Kotlin
- **UI:** Jetpack Compose + Material 3
- **Architecture:** MVVM + Clean Architecture
- **Database:** Room
- **Dependency Injection:** Hilt
- **Min SDK:** 26 (Android 8.0)
- **Target SDK:** 34

## 📸 Screenshots
<div align="center">
<img src="screenshots/home.png" width="250">
<img src="screenshots/editor.png" width="250">
<img src="screenshots/search.png" width="250">
</div>

## 🏗️ Architecture
```
app/
├── data/
│   ├── local/
│   │   ├── NoteDatabase.kt
│   │   └── NoteDao.kt
│   └── repository/
│       └── NoteRepositoryImpl.kt
├── domain/
│   ├── model/
│   │   └── Note.kt
│   ├── repository/
│   │   └── NoteRepository.kt
│   └── usecase/
│       ├── GetNotesUseCase.kt
│       ├── AddNoteUseCase.kt
│       └── DeleteNoteUseCase.kt
├── ui/
│   ├── screens/
│   │   ├── home/
│   │   │   ├── HomeScreen.kt
│   │   │   └── HomeViewModel.kt
│   │   └── editor/
│   │       ├── EditorScreen.kt
│   │       └── EditorViewModel.kt
│   ├── components/
│   │   └── NoteCard.kt
│   └── theme/
│       ├── Color.kt
│       ├── Theme.kt
│       └── Type.kt
└── di/
    └── AppModule.kt
```

## 🚀 Getting Started

### Prerequisites
- Android Studio Arctic Fox or later
- JDK 17
- Android device or emulator (API 26+)

### Installation
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/notes-app.git

# Open in Android Studio
File -> Open -> Select the cloned directory

# Run the app
Click Run button or use Shift+F10
```

## 📦 Dependencies
```kotlin
// Room Database
implementation "androidx.room:room-runtime:2.6.1"
implementation "androidx.room:room-ktx:2.6.1"
kapt "androidx.room:room-compiler:2.6.1"

// Jetpack Compose
implementation "androidx.compose.material3:material3:1.2.0"
implementation "androidx.compose.ui:ui:1.6.0"
implementation "androidx.activity:activity-compose:1.8.2"

// Hilt
implementation "com.google.dagger:hilt-android:2.50"
kapt "com.google.dagger:hilt-compiler:2.50"
implementation "androidx.hilt:hilt-navigation-compose:1.1.0"

// Navigation
implementation "androidx.navigation:navigation-compose:2.7.6"
```

## 🤝 Contributing
Contributions are welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) first.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments
- [Jetpack Compose](https://developer.android.com/jetpack/compose)
- [Material Design 3](https://m3.material.io/)
- [Room Database](https://developer.android.com/training/data-storage/room)

---

Made with ❤️ by [Your Name]
