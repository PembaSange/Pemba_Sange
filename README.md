VUApp - Android Application
VUApp is an Android application built with Kotlin using the MVVM architecture, Hilt for dependency injection, and Retrofit for network communication. The app includes user login functionality and fetches dashboard data upon successful authentication.
📱 Features
•	• User login with dynamic server location (sydney, footscray, ort)
•	• Retrieves dashboard data using a secure keypass
•	• Clean UI using CardView and ConstraintLayout
•	• Organized project with ViewModel, Repository, and Data Models
•	• Uses Retrofit + Coroutines for network calls
•	• Hilt for dependency injection
🧱 Project Structure

com.example.vuapp

data
api
AuthApiService.kt
DashboardApiService.kt
model
DashboardResponse.kt
Entity.kt
repository
AuthRepository.kt

ui
login
LoginActivity.kt
LoginViewModel.kt
dashboard
DashboardActivity.kt

di
AppModule.kt

MainActivity.kt

🛠️ Setup Instructions
1. Clone the Repository

git clone https://github.com/your-username/vuapp.git
cd vuapp

2. Open in Android Studio
- Open Android Studio.
- Click File > Open and select the cloned project directory.
3. Set Up Dependencies
Ensure you have:
- Android Studio Hedgehog (or newer)
- Kotlin 1.9+
- Gradle 8+
- Internet access (for downloading dependencies)

All required dependencies are defined in build.gradle.kts.
4. Run the App
- Plug in an Android device or start an emulator.
- Click the Run button in Android Studio.
🔐 Login Flow
- Enter a username and password
- Location is hardcoded in LoginActivity.kt (default: sydney)
- On success, a keypass is received and passed to the Dashboard
🎨 UI Customization
To change the background color of the login screen:
1. Open activity_login.xml
2. Set the root layout background to #00ffc0:
<android:background="#00ffc0">
🧪 Dependencies Used
•	• Retrofit – HTTP Client
•	• Hilt – Dependency Injection
•	• Kotlin Coroutines – Async programming
•	• AndroidX ViewModel & LiveData
•	• Material Design Components
💡 Notes
- The app uses dynamic endpoints such as /{location}/auth
- Make sure the backend server is running and supports the login and dashboard routes
📄 License
This project is licensed under the MIT License.
