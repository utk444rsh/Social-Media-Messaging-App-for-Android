# 2gether

2gether Messenger is an Android messaging application that allows users to communicate with each other. It includes features such as user authentication, profile settings, and real-time messaging. This project uses Firebase for backend services, including authentication, real-time database, and storage.
![image](https://github.com/utk444rsh/Social-Media-Messaging-App-for-Android/assets/124518418/7d62dd07-c1dc-4242-9009-719b1ba4412b) ![image](https://github.com/utk444rsh/Social-Media-Messaging-App-for-Android/assets/124518418/7c0f14ff-65a0-4130-a949-e146eccb6a6c) ![image](https://github.com/utk444rsh/Social-Media-Messaging-App-for-Android/assets/124518418/0d3d480e-dd72-4070-a445-b965a4f13fdd) ![image](https://github.com/utk444rsh/Social-Media-Messaging-App-for-Android/assets/124518418/1043bbb7-3188-4dd0-a9aa-573c926a81b1) ![image](https://github.com/utk444rsh/Social-Media-Messaging-App-for-Android/assets/124518418/33651ddd-9a47-4956-ad43-d6c5613d6217)






## Features

- **User Authentication**: Sign up and log in using email and password.
- **Real-time Messaging**: Send and receive messages instantly.
- **Profile Management**: Update profile picture, username, and status.
- **Image Upload**: Users can upload and display profile pictures.
- **Progress Dialogs**: Inform users of ongoing processes, like saving data.

## Major Activities

### MainActivity

The entry point of the application. This activity allows users to either sign in with their existing account or sign up for a new account. It handles the authentication logic and directs users to the appropriate screens based on their authentication status.

**Functions:**
- Handles user authentication.
- Redirects to ChatActivity if the user is already authenticated.
- Redirects to SignUpActivity for new users.

### ChatActivity

Handles the real-time messaging functionality between users. This activity displays the chat interface where users can send and receive messages. It utilizes Firebase Realtime Database to fetch and display messages in real-time.

**Functions:**
- Displays a list of messages in a chat.
- Sends new messages typed by the user.
- Updates the chat in real-time with messages from other users.

### SettingsActivity

Allows users to update their profile information, including profile picture, username, and status. Users can select a new profile picture from their device and upload it to Firebase Storage. The activity also shows a progress dialog while the data is being saved.

**Functions:**
- Fetches and displays current user profile information.
- Allows users to change their profile picture.
- Allows users to update their username and status.
- Saves updated profile information to Firebase.

**Refer to `Report[1].doc` for a detailed description of the application architecture and implementation details.**

## Getting Started

### Prerequisites

- Android Studio
- Firebase Account

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/2gether.git
    ```
2. Open the project in Android Studio.
3. Connect your project to Firebase:
    - Go to Tools > Firebase.
    - Connect your app to Firebase and add the necessary Firebase services (Authentication, Realtime Database, Storage).
4. Update the `google-services.json` file in the `app` directory with your Firebase project configuration.

### Usage

1. Run the app on an emulator or a physical device.
2. Sign up with a new account or log in with an existing one.
3. Update your profile in the SettingsActivity.
4. Start chatting with other users.

## Dependencies

- Firebase Authentication
- Firebase Realtime Database
- Firebase Storage
- Picasso (for image loading)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to Firebase for providing a robust backend service.
- Thanks to the open-source community for the libraries used in this project.
