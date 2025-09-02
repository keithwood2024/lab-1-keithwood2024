# Lab Task Squirrel 🐿️

A location-based task management iOS application built with Swift and UIKit. This app allows users to create tasks, attach photos with location data, and track task completion through an intuitive interface.

## 📱 Features

- **Task Management**: Create, view, and manage tasks with titles and descriptions
- **Photo Attachments**: Add photos to tasks to mark them as complete
- **Location Tracking**: Automatically capture and store location data when photos are taken
- **Interactive Map**: View task locations on an embedded MapKit map
- **Task Status**: Visual indicators for completed vs. incomplete tasks
- **Mock Data**: Pre-populated with sample tasks for demonstration

## 🏗️ Architecture

The app follows the Model-View-Controller (MVC) pattern and is built using:

- **Swift** - Primary programming language
- **UIKit** - User interface framework
- **Storyboards** - Interface design and navigation
- **CoreLocation** - Location services
- **MapKit** - Map display and annotations
- **PhotosUI** - Photo library access

## 📁 Project Structure

```
lab-task-squirrel/
├── Models/
│   └── Task.swift                 # Core data model for tasks
├── Task List/
│   ├── TaskListViewController.swift    # Main task list view
│   └── TaskCell.swift                 # Custom table view cell
├── Task Detail/
│   ├── TaskDetailViewController.swift  # Task detail and photo capture
│   ├── TaskAnnotationView.swift       # Custom map annotation view
│   └── PhotoViewController.swift       # Photo viewing interface
├── Task Compose/
│   └── TaskComposeViewController.swift # Task creation interface
├── Assets.xcassets/               # App icons and colors
├── Base.lproj/                    # Localization and storyboards
└── Info.plist                     # App configuration
```

## 🎯 Core Components

### Task Model
- Stores task title, description, completion status, and optional photo with location
- Provides mock data for demonstration purposes
- Automatically determines completion status based on photo presence

### Task List View
- Displays all tasks in a table view format
- Shows empty state when no tasks exist
- Handles navigation to task detail and creation views
- Supports adding new tasks via closure-based communication

### Task Detail View
- Shows complete task information
- Allows photo capture and attachment
- Displays location data on an interactive map
- Provides visual completion status indicators

### Map Integration
- Embedded MapKit view for location visualization
- Custom annotation views for task locations
- Automatic map updates based on task completion status

## 🚀 Getting Started

### Prerequisites
- Xcode 14.0 or later
- iOS 15.0+ deployment target
- macOS (for development)

### Installation
1. Clone the repository
2. Open `lab-task-squirrel.xcodeproj` in Xcode
3. Select your target device or simulator
4. Build and run the project (⌘+R)

### Permissions
The app requires the following permissions:
- **Photo Library Access**: To attach photos to tasks
- **Location Services**: To capture location data when photos are taken

## 📱 Usage

1. **View Tasks**: The main screen displays all existing tasks
2. **Create Tasks**: Tap the compose button to add new tasks
3. **Complete Tasks**: Tap on a task to view details and attach a photo
4. **View Locations**: Completed tasks show their location on an interactive map
5. **Photo Management**: View attached photos and their associated locations

## 🔧 Development Notes

- The app includes mock data for demonstration purposes
- Photo capture functionality integrates with the device's photo library
- Location services automatically capture coordinates when photos are taken
- Map annotations are customized for better visual representation
- The interface adapts based on task completion status

## 🐛 Known Issues

- Some merge conflicts exist in the codebase that need resolution
- Photo picker implementation may require additional authorization handling
- Map view delegate setup is partially implemented

## 👥 Contributors

- **Charlie Hieger** - Original project creation and core implementation
- **Keith Wood** - Project development and modifications

## 📄 License

This project is part of a COP 4655 lab assignment at the University of Central Florida.

## 🤝 Contributing

This is an educational project. For questions or issues, please contact the course instructor or refer to the course materials.

---

*Built with ❤️ for iOS development learning*

## 📱 App Demo

<img src="app-demo.gif" width="200" alt="App Demo" />

*Screen recording demonstrating the app's functionality and user interface*
