# Setup Instructions

## Environment Variables Required

Create a `.env.local` file in the root directory with the following Firebase configuration:

```bash
# Firebase Configuration
FIREBASE_PROJECT_ID=your-project-id
FIREBASE_CLIENT_EMAIL=your-service-account-email@your-project.iam.gserviceaccount.com
FIREBASE_PRIVATE_KEY="-----BEGIN PRIVATE KEY-----\nYOUR_PRIVATE_KEY_HERE\n-----END PRIVATE KEY-----"
FIREBASE_STORAGE_BUCKET=xensilico-leads.firebasestorage.app
```

## How to Get Firebase Credentials

1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Select your project
3. Go to Project Settings (gear icon)
4. Go to "Service Accounts" tab
5. Click "Generate new private key"
6. Download the JSON file
7. Extract the values:
   - `project_id` → `FIREBASE_PROJECT_ID`
   - `client_email` → `FIREBASE_CLIENT_EMAIL`
   - `private_key` → `FIREBASE_PRIVATE_KEY`

## Running the Project

1. Install dependencies: `npm install`
2. Create `.env.local` with your Firebase credentials
3. Start development server: `npm run dev`
4. Open http://localhost:3000

## Features

- User authentication (signup/login)
- Profile management
- Data upload functionality
- Firebase integration
- Responsive design
- Custom cursor (optional)

## Deployment

The project is ready for deployment to Vercel, Netlify, or other platforms. Make sure to set the environment variables in your deployment platform.
