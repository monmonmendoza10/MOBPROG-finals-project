# Personal Profile App - Flutter Mobile Application

A comprehensive Flutter mobile application developed as an individual student project for Mobile Programming Finals. This app showcases personal profile management with a clean, modern UI using Material Design 3.

## Project Overview

This application demonstrates proficiency in:
- Flutter fundamentals and widget composition
- UI/UX design with Material 3
- Navigation and routing
- Form handling and validation
- State management with StatefulWidget and setState
- Dialog interactions and user confirmations

## Features

### 1. Profile / Home Screen
- Display personal information with an attractive card-based layout
- Profile picture using CircleAvatar
- Name, bio, and contact information
- Hobbies and interests section
- Friends list preview showing first 3 friends
- Navigation buttons to Edit Profile and Friends List screens
- Clean, modern design with blue and red color scheme

### 2. Edit Profile Screen
- Form-based profile editing with validation
- Editable fields:
  - Full Name (required)
  - Bio/Description (required)
  - Email (required, validated)
  - Hobbies & Interests (required)
- Real-time input validation with error messages
- Confirmation dialog before saving changes
- Updates reflected immediately on Profile screen

### 3. Friends List Screen
- ListView displaying all friends
- Each friend shown in a Card with avatar, name, and relationship
- Edit and Delete actions for each friend
- Add new friend using FloatingActionButton
- Delete confirmation dialog for safety
- Empty state with helpful message when no friends exist

### 4. Add / Edit Friend Screen
- Form for adding new friends or editing existing ones
- Fields:
  - Friend Name (required)
  - Relationship (required, e.g., Best Friend, Classmate)
- Input validation
- Save confirmation dialog
- Dynamic title based on Add or Edit mode

## Technical Implementation

### Design Requirements Met
- Material 3 design system
- Blue and red color palette throughout the app
- Consistent spacing and card-based layouts
- Responsive design with proper padding and margins
- Icon usage for better visual communication
- Clean typography hierarchy

### Flutter Concepts Demonstrated
- **Widgets**: StatelessWidget, StatefulWidget, Card, ListTile, CircleAvatar
- **Navigation**: Navigator.push, Navigator.pop with data passing
- **Forms**: Form, TextFormField, GlobalKey<FormState>
- **Validation**: Required fields, email validation, error messages
- **Dialogs**: AlertDialog for confirmations
- **State Management**: setState for local state updates
- **Controllers**: TextEditingController for form inputs
- **Lifecycle**: initState, dispose for proper resource management

### Code Organization
- All code contained in `lib/main.dart` as specified
- Clear widget separation with meaningful names
- Model classes for Profile and Friend data
- Well-commented and properly formatted
- Beginner-friendly structure

## Project Structure

```
personal_profile_app/
├── lib/
│   └── main.dart              # Complete application code
├── android/                    # Android configuration
├── pubspec.yaml               # Flutter dependencies
└── README.md                  # Project documentation
```

## How to Run

### Prerequisites
- Flutter SDK installed (version 3.0.0 or higher)
- Android Studio or VS Code with Flutter extensions
- Android device or emulator

### Steps
1. Clone or download this repository
2. Open terminal in project directory
3. Run `flutter pub get` to install dependencies
4. Connect an Android device or start an emulator
5. Run `flutter run` to launch the app

## Color Scheme

- **Primary Color**: Blue - Used for AppBars, primary buttons, and main accents
- **Secondary Color**: Red - Used for secondary actions and highlights
- **Card Background**: White with elevation shadows
- **Text Colors**: Dark text on light backgrounds for readability

## Validation Rules

### Edit Profile Form
- Name: Required, cannot be empty
- Bio: Required, cannot be empty
- Email: Required, must contain '@' symbol
- Hobbies: Required, cannot be empty

### Add/Edit Friend Form
- Friend Name: Required, cannot be empty
- Relationship: Required, cannot be empty

## User Experience Features

- **Confirmation Dialogs**: All destructive or important actions require user confirmation
- **Input Validation**: Real-time feedback on form errors
- **Visual Feedback**: Clear button states, loading indicators
- **Empty States**: Helpful messages when lists are empty
- **Responsive Layout**: Works on various screen sizes
- **Smooth Navigation**: Proper back navigation with data passing

## Sample Data

The app includes sample data for demonstration:
- Profile: Juan Dela Cruz (Computer Science Student)
- Friends: 3 pre-populated friends with different relationships

## Development Notes

This is an individual student project focusing on:
- Clean code practices
- Proper widget composition
- Flutter best practices for beginners
- Material Design guidelines
- User-friendly interface design

## Platform Support

- **Android**: Fully supported (minSdkVersion 21)
- **iOS**: Compatible (optional, not required for this project)

## License

This is a student project for educational purposes.

## Author

Created as a Mobile Programming Finals Project