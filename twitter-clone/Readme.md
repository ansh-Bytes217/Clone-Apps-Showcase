**Twitter clone**

built in Next.js + TypeScript + Tailwind CSS using Cloud Firestore and Storage

**Features**✨
->Authentication with Firebase Authentication

->Strongly typed React components with TypeScript

->Users can add tweets, like, retweet, and reply

->Users can delete tweets, add a tweet to bookmarks, and pin their tweet

->Users can add images and GIFs to tweet

->Users can follow and unfollow other users

->Users can see their and other followers and the following list

->Users can see all users and the trending list

->Realtime update likes, retweets, and user profile

->Realtime trending data from Twitter API

->User can edit their profile

->Responsive design for mobile, tablet, and desktop

_>Users can customize the site color scheme and color background

->All images uploads are stored on Firebase Cloud Storage

**Tech** 🛠
Next.js
TypeScript
Tailwind CSS
Firebase
SWR
Headless UI
React Hot Toast
Framer Motion
Development 💻
Here are the steps to run the project locally.

**Clone the repository**

git clone https://github.com/ccrsxx/twitter-clone.git
Install dependencies

npm i
Create a Firebase project and select the web app

Add your Firebase config to .env.development. Note that NEXT_PUBLIC_MEASUREMENT_ID is optional

Make sure you have enabled the following Firebase services:

Authentication. Enable the Google sign-in method.
Cloud Firestore. Create a database and set its location to your nearest region.
Cloud Storage. Create a storage bucket.
Install Firebase CLI globally

npm i -g firebase-tools
Log in to firebase::

firebase login
Get your project ID::

firebase projects:list
Select your project ID::

firebase use your-project-id
At this point, you have two choices. Either run this project using the Firebase on the cloud or locally using emulator.

Using the Firebase Cloud Backend:

Deploy Firestore rules, Firestore indexes, and Cloud Storage rules

firebase deploy --except functions
Run the project

npm run dev
Using Firebase Local Emulator:

Install Java JDK version 11 or higher before proceeding. This is required to run the emulators.

Set the environment variable NEXT_PUBLIC_USE_EMULATOR to true in .env.development. This will make the app use the emulators instead of the cloud backend.

At this point, you can run the following command to have a fully functional Twitter clone running locally:

npm run dev:emulators
Note: When you deploy Firestore indexes rules, it might take a few minutes to complete. So before the indexes are enabled, you will get an error when you fetch the data from Firestore.

You can check the status of your Firestore indexes with the link below, replace your-project-id with your project ID: https://console.firebase.google.com/u/0/project/your-project-id/firestore/indexes

