# Quick Start Guide - Personal Profile App

## For Students: How to Use This Project

This guide will help you understand, run, and demonstrate your Personal Profile App for your Mobile Programming Finals.

## Prerequisites

Before running the app, ensure you have:

1. **Flutter SDK** installed on your computer
   - Download from: https://flutter.dev/docs/get-started/install
   - Verify installation: Run `flutter doctor` in terminal

2. **Android Studio** or **VS Code** with Flutter extensions
   - Android Studio: https://developer.android.com/studio
   - VS Code with Flutter extension

3. **Android Device or Emulator**
   - Physical Android phone with USB debugging enabled, OR
   - Android emulator from Android Studio

## Installation Steps

### Step 1: Get the Project
```bash
# If cloned from Git
cd personal_profile_app

# If downloaded as ZIP
# Extract the ZIP file and navigate to the folder
```

### Step 2: Install Dependencies
```bash
flutter pub get
```

### Step 3: Verify Setup
```bash
flutter doctor
```
Make sure all checks pass (especially Flutter, Android toolchain, and connected devices).

### Step 4: Check Connected Devices
```bash
flutter devices
```
You should see at least one device listed.

### Step 5: Run the App
```bash
flutter run
```

The app will build and launch on your connected device!

## Project Structure Overview

```
personal_profile_app/
├── lib/
│   └── main.dart           ← ALL YOUR CODE IS HERE
├── android/                ← Android platform files
│   ├── app/
│   │   ├── src/
│   │   └── build.gradle
│   ├── build.gradle
│   └── settings.gradle
├── pubspec.yaml           ← Dependencies and app config
├── README.md              ← Full documentation
├── PROJECT_FEATURES.md    ← Features checklist
└── QUICK_START.md         ← This file
```

## Understanding the Code (main.dart)

The `lib/main.dart` file contains everything, organized as follows:

### 1. Main App Setup (Lines 1-20)
```dart
void main() => runApp(PersonalProfileApp());
```
- App entry point
- Material Design 3 theme with blue and red colors

### 2. Data Models (Lines 21-45)
```dart
class Profile { ... }
class Friend { ... }
```
- Simple data structures for Profile and Friend

### 3. Screen 1: ProfileScreen (Lines 46-280)
- Displays user profile and friends preview
- Navigation to other screens
- Sample data initialization

### 4. Screen 2: EditProfileScreen (Lines 281-480)
- Form for editing profile
- Validation logic
- Save confirmation dialog

### 5. Screen 3: FriendsListScreen (Lines 481-650)
- ListView of friends
- Add, edit, delete operations
- Empty state handling

### 6. Screen 4: AddEditFriendScreen (Lines 651-800)
- Form for adding/editing friends
- Dynamic title based on mode
- Save confirmation

## Testing the App

### Test Scenario 1: View Profile
1. Launch the app
2. You'll see the Profile screen with sample data
3. Observe all the information cards

### Test Scenario 2: Edit Profile
1. Tap "Edit Profile" button
2. Try to save with empty fields (see validation)
3. Fill in all fields
4. Tap "Save Changes"
5. Confirm in the dialog
6. See updated data on Profile screen

### Test Scenario 3: Manage Friends
1. Tap "View Friends" button
2. See the list of 3 sample friends
3. Tap the edit icon on any friend
4. Update the friend's information
5. Save and confirm

### Test Scenario 4: Add New Friend
1. On Friends List screen
2. Tap the "Add Friend" button (or FAB)
3. Enter friend name and relationship
4. Save and confirm
5. See new friend in the list

### Test Scenario 5: Delete Friend
1. On Friends List screen
2. Tap delete icon on any friend
3. Confirm deletion
4. Friend is removed from list

## Demonstrating Your Project

When presenting to your instructor, highlight:

### 1. Four Complete Screens ✓
- Show each screen and explain its purpose
- Demonstrate navigation between screens

### 2. Form Validation ✓
- Show what happens with empty fields
- Show email validation
- Show error messages

### 3. Dialogs ✓
- Demonstrate save confirmation
- Demonstrate delete confirmation
- Show cancel and confirm actions

### 4. State Management ✓
- Edit profile and show data updates
- Add friend and show list updates
- Delete friend and show list updates

### 5. UI Design ✓
- Point out Material 3 design
- Show blue and red color scheme
- Highlight card layouts and spacing
- Show icons and visual elements

## Common Issues and Solutions

### Issue: "Flutter command not found"
**Solution**: Add Flutter to your PATH or reinstall Flutter SDK

### Issue: "No devices connected"
**Solution**:
- Enable USB debugging on Android phone
- Or start an Android emulator from Android Studio

### Issue: "Build failed"
**Solution**:
```bash
flutter clean
flutter pub get
flutter run
```

### Issue: "Gradle build error"
**Solution**:
- Check your internet connection (Gradle downloads dependencies)
- Update Android SDK in Android Studio

## Customizing the App

Want to personalize it? Here's how:

### Change Colors
In `main.dart`, find:
```dart
colorScheme: ColorScheme.fromSeed(
  seedColor: Colors.blue,
  primary: Colors.blue,
  secondary: Colors.red,
)
```
Change `Colors.blue` and `Colors.red` to your preferred colors!

### Change Sample Data
In `ProfileScreen`, find the `initState` section:
```dart
Profile profile = Profile(
  name: 'YOUR NAME HERE',
  bio: 'YOUR BIO HERE',
  email: 'YOUR EMAIL HERE',
  hobbies: 'YOUR HOBBIES HERE',
);
```

### Add Your Photo
Currently using icon-based avatars. To add a real photo:
1. Add image to `assets/images/` folder
2. Update `pubspec.yaml` to include assets
3. Replace `CircleAvatar` icon with `AssetImage`

## Tips for Success

1. **Understand the Code**: Read through main.dart and understand each section
2. **Test Everything**: Make sure all features work before presenting
3. **Be Prepared**: Know how to explain navigation, validation, and state management
4. **Have Backup**: Test on emulator AND physical device if possible
5. **Practice Demo**: Run through the demo a few times before presenting

## Key Learning Points

This project teaches you:
- **Widgets**: How to compose UI from Flutter widgets
- **Navigation**: How to move between screens and pass data
- **Forms**: How to handle user input and validation
- **State**: How to manage and update app state
- **Dialogs**: How to show confirmations and alerts
- **Design**: How to create a clean, modern UI

## Support Resources

If you need help:
- Flutter Documentation: https://flutter.dev/docs
- Flutter Widget Catalog: https://flutter.dev/docs/development/ui/widgets
- Stack Overflow: https://stackoverflow.com/questions/tagged/flutter
- Flutter Community: https://flutter.dev/community

## Final Checklist Before Submission

- [ ] App runs without errors
- [ ] All 4 screens are functional
- [ ] All forms validate properly
- [ ] All dialogs work correctly
- [ ] Navigation works smoothly
- [ ] Colors are blue and red as required
- [ ] Code is in main.dart
- [ ] README.md is complete
- [ ] Tested on Android device/emulator

## Good Luck!

You now have a complete, functional Flutter app that demonstrates all required concepts for your Mobile Programming Finals. Practice your demo and be ready to explain the code!

Remember: The goal is not just to have a working app, but to understand HOW and WHY it works!
