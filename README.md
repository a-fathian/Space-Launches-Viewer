![Android CI](https://github.com/a-fathian/Space-Launches-Viewer/actions/workflows/android-ci.yml/badge.svg)

# Space Launches Viewer

Production-style Android application showcasing modern Android development
practices with a strong focus on clean architecture, testability, and
maintainability.

The app allows users to browse space launches, view detailed information,
and bookmark favorite launches using a modern, reactive UI and Offline-first support.

---

## Tech Stack

- **Language:** Kotlin
- **UI:** Jetpack Compose
- **Architecture:** Clean Architecture + MVVM
- **Async:** Kotlin Coroutines & Flow
- **Networking:** Retrofit / OkHttp
- **Dependency Injection:** Hilt
- **Local Storage:** Room
- **Build System:** Gradle (Version Catalog)
- **Testing:** JUnit, Coroutine Test, Mockito
- **Other:** Material Design, Coil

---

## Architecture Overview

The project follows **Clean Architecture** principles to ensure a clear
separation of concerns and high testability.

UI (Compose)

│

├── Presentation Layer (ViewModels, UI State)

│

├── Domain Layer (UseCases, Business Rules)

│

└── Data Layer (Repositories, Remote & Local Data Sources)


- **Presentation layer** handles UI state and user interactions.
- **Domain layer** contains pure business logic with no Android dependencies.
- **Data layer** manages API communication and local persistence.

This structure allows independent testing of each layer and supports
scalability for larger teams.

---

## Modularization

The application is structured into multiple Gradle modules:

- `app` – Application setup and navigation
- `data` – Repositories and data sources
- `domain` – Use cases and business models
- `presentation` – Viewmodels and composables

✅ Improved build times  
✅ Clear ownership boundaries  
✅ High scalability for enterprise projects

---

## Testing

The project includes **unit tests across all major layers**, following
industry best practices.

### Covered Test Types

- **Repository tests**
  - Validate data fetching from remote and local sources
  - Ensure proper error handling and data mapping

- **Use Case tests**
  - Verify business logic in isolation
  - Run as pure JVM tests without Android dependencies

- **ViewModel tests**
  - Validate UI state changes
  - Test coroutine and Flow-based asynchronous logic

### Testing Tools

- JUnit
- Kotlin Coroutines Test
- Mockito

Tests are designed to be **fast, deterministic, and CI-friendly**, enabling
safe refactoring and continuous delivery.

---

## CI Pipeline

The project uses GitHub Actions to automatically build the application
and run unit tests on every pull request and main branch update, ensuring
code quality and stability.

---

## UI & UX

- Built fully with **Jetpack Compose**
- Reactive UI driven by immutable UI state
- Material Design principles applied
- Supports loading, success, and error states

---

## Why This Project Exists

This project was created to demonstrate:
- Senior-level Android architecture decisions
- Real-world modular Android project setup
- Clean, testable, and scalable code
- Modern Android development aligned with industry standards

---

## Future Improvements

- UI tests with Compose Testing
- Pagination for large data sets
- Improved error handling UX

---

## Author

**Ali Fathian**  
Senior Android Engineer  

- GitHub: https://github.com/a-fathian
- LinkedIn: https://linkedin.com/in/ali-fathian
