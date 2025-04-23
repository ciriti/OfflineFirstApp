# Maintenance Tracker

An offline-first Android application for train technicians to view maintenance tasks, designed to work seamlessly with intermittent connectivity.

## Architecture Overview

### Core Principles
- **Offline-First** - Prioritizes local data
- **Unidirectional Data Flow**
- **Modular Design** - Strict separation of concerns via clean architecture layers

### Tech Stack
- **Kotlin**
- **Jetpack Compose**
- **Koin**
- **Room**
- **Retrofit**
- **Coroutines/Flow**


#### Layer Responsibilities:

1. **Data Layer**
    - `datasource/`: Concrete implementations for API (Remote) and DB (Local)
    - `repository/`: Mediates between sources, handles business logic
    - `sync/`: Manages offline-first synchronization

2. **Domain Layer**
    - Entity definitions
    - Interfaces
    - Pure Kotlin (no Android dependencies)

3. **UI Layer**
    - Compose-based presentation
    - State hoisting to ViewModels
    - Theming and component library

## Setup

1. Clone repository https://github.com/ciriti/OfflineFirstApp.git
2. Open in Android Studio
3. Build and run
