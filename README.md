# TalkingJunction
A simple real time chat application inspired from letschat.

# Tech Stack
- React and TailwindCSS for the frontend
- Firebase for authentication
- Node/Express for creating API endpoints
- MongoDB for storing chat room members and their messages
- Socket.io for making the app real-time

# Functionalities
- Users can `login/register`
- Can update `details` and `avatars` on profile
- Generates random avatar using [DiceBear API](https://avatars.dicebear.com/docs/http-api)
- Can create a room
- Shows active status
- Search other users
- Emojis and dark mode is there

# Run this project locally
1. Clone the repository
2. Installing dependencies
   - navigate to `frontend` and run `npm install`
   - navigate to `server` and run `npm install`
3. Setup Firebase
   - Go to the [Firebase Console](https://console.firebase.google.com/)
   - Create a new project
   - Go to `Project Settings >> Service Accounts`
   - Click on `"Get new private key"`
   - Rename the downloaded JSON file as `serviceAccountKey.json`
   - Put the  `serviceAccountKey.json` in `server/config` directory
   - Now go to the Code symbol in the general settings of the project settings below
   - And register a new project
   - You'll get the `.env` details
4. Set up the environment variables
   - In both the directories rename the `.env.example` file to `.env`
   - Put the actual values of the APIs with the firebase configuration
   - Update the `PORT` and the `MONGO_URI` with your own database url
5. Run the server
   - Navigate to server and do `npm run start`
6. Run the client
   - Navigate to the frontend and do `npm start`

The application will be accessible at `http://localhost:3000`

MAKE SURE NOT TO COMMIT THE `serviceAccountKey.json` FILE IN IN the VerSION CONTROL AS IT CONTAINS SENSITIVE INFORMATION.


## Authors
- Yours Truly, [@Sneha Dwivedi](https://github.com/dwivedisneha)
