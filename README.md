# ShiftTrackr

## Overview  
ShiftTrackr is a web application designed for business owners and employees to manage working hours efficiently. Employees can clock in and out, while employers can review and approve timesheets for accurate payroll processing.  

## Features  
- **User Authentication** – Secure login and registration using Firebase Authentication.  
- **Time Logging** – Employees clock in and out, logging hours accurately.  
- **Approval Workflow** – Employers review and approve hours before payroll processing.  
- **Payroll Calculation** – Automatically calculates total weekly work hours for payroll.  
- **Dashboard** – Employers can view pending and approved hours.  
- **Offline Support** – Employees can log hours offline, syncing when online.  
- **Real-time Updates** – Instant synchronization with Firebase Firestore.  

## Technologies Used  
- **Frontend:** Flutter (Dart)  
- **State Management:** Riverpod (or Provider, to be decided)  
- **Backend:** Firebase Firestore (NoSQL)  
- **Authentication:** Firebase Authentication  
- **Offline Sync:** Firestore local persistence  

## Getting Started  

### Installation  
```bash
# Clone the repository
git clone https://github.com/your-username/ShiftTrackr.git  
cd ShiftTrackr  

# Install dependencies  
flutter pub get  
```

### Firebase Setup  
1. Create a Firebase Project at [Firebase Console](https://console.firebase.google.com/)  
2. Enable Authentication (Email/Password)  
3. Enable Firestore Database (with offline sync)  
4. Download `google-services.json` and place it in `android/app/`  

### Running the App  
```bash
flutter run  
```

## Project Structure  
```
/lib  
 ├── main.dart             # Entry point  
 ├── screens/              # UI screens (Login, Dashboard, Time Tracking)  
 ├── providers/            # State management with Riverpod  
 ├── services/             # Firebase Firestore interactions  
 ├── models/               # Data models (User, Shift, Payroll)  
 ├── utils/                # Utility functions  
```

## Future Features  
- Export payroll reports as CSV  
- Implement overtime and bonus tracking  
- Role-based permissions (Admin, Manager, Employee)  

## Contributing  
1. Fork the repository  
2. Create a feature branch: `git checkout -b feature-name`  
3. Commit changes: `git commit -m "Added feature"`  
4. Push to branch: `git push origin feature-name`  
5. Open a Pull Request  


