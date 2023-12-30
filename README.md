# QuizQuest 

## Overview

QuizQuest is a comprehensive quiz management system designed to simplify the creation, management, and completion of quizzes. It provides a user-friendly interface and integrates Firebase authentication and Firestore database, ensuring secure access and management of quizzes for both admin and student roles.

## Tech Stack

- **Next.js**: Full Stack framework for building the web application.
- **Typescript**: Ensuring type safety and improved development experience.
- **Firebase**: Authentication, Firestore database for secure data storage.
- **Tailwind CSS**: Utilized for styling and responsive design.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/Akash-Singh04/QuizQuest.git
   ```

2. Install dependencies:

   ```bash
   cd QuizQuest
   npm install
   ```
   
3. Firebase Configuration Setup
-Contact @Akash-Singh04 to get collaborator access to the firebase project that contains the User Authentication and Firebase Firestore Database. An email will be sent with the invitaion for the same.

4. Steps to Set Firebase Environment Variables

1. **After Getting Collaborator Access**:
   - Visit the Firebase Console
   - Navigate to the project settings.

2. **Retrieve Firebase Configuration**:
   - In the Firebase project settings, locate and select the "General" tab.
   - Scroll down to the "Your apps" section and click on Quiz-Quest

3. **Copy Configuration Details**:
   - After creating the web app, you'll get a configuration object containing keys like `apiKey`, `authDomain`, `projectId`, etc.
   - Copy these configuration details.

4. **Environment Variable Setup**:
   - Create a `.env.local` file in the root directory of your project (ensure it's added to `.gitignore` for security).
   - Add the Firebase configuration details as environment variables:

   ```env
   NEXT_PUBLIC_FIREBASE_API_KEY="YOUR_FIREBASE_API_KEY"
   NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN="YOUR_FIREBASE_AUTH_DOMAIN"
   NEXT_PUBLIC_FIREBASE_PROJECT_ID="YOUR_FIREBASE_PROJECT_ID"
   NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET="YOUR_FIREBASE_STORAGE_BUCKET"
   NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID="YOUR_FIREBASE_MESSAGING_SENDER_ID"
   NEXT_PUBLIC_FIREBASE_APP_ID="YOUR_FIREBASE_APP_ID"
   NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID="YOUR_FIREBASE_MEASUREMENT_ID"  // (Optional, for Analytics)
   ```

5. **Usage in Project**:
   - Access these environment variables in your code as `process.env.VARIABLE_NAME`.

6. **Restart Server**:
   - After setting environment variables, restart the development server to apply the changes.

### Note:
- Ensure that you replace `"YOUR_FIREBASE_XXX"` placeholders with the actual values from your Firebase project configuration.
- Remember to keep your `.env.local` file private and do not expose sensitive credentials in your code repository.

5. Run the project:

   ```bash
   npm run dev
   ```
6. Access the project locally at `http://localhost:3000`.

## Deployment

The live deployment of QuizQuest can be accessed at [QuizQuest](https://quiz-quest-delta.vercel.app/).

## Features

### Admin Panel

- **Firebase Authentication**: Admins can securely log in to access the admin panel.
- **Quiz Data Upload**: Admins can upload Excel files containing quiz data for automatic quiz generation.
- **Interactive UI**: User-friendly interface for entering quiz details and managing quiz data.
- **Firebase Integration**: Firebase Firestore database integration for storing quiz data securely.

### Student Dashboard

- **User Authentication**: Students can securely log in using Firebase authentication.
- **Quiz Access**: Access available quizzes, view details, and track completion status.
- **Real-time Updates**: Firebase ensures real-time updates for quiz status and progress tracking.

## Contributing

-Contributions are welcome! Feel free to fork the repository, make improvements, and create pull requests.
-Please view the list of open issues at [Issues](https://github.com/Akash-Singh04/QuizQuest/issues). Any contributions to them are welcome.

## Authors

* **Akash Singh**(https://github.com/Akash-Singh04)

See also the list of [contributors](https://github.com/Akash-Singh04/QuizQuest/contributors) who participated in this project.

## License

This project is licensed under the [MIT License](LICENSE).
