# Under construction

# 👷‍♂️🏗️🚧⚠️

# Real-Time Messenger App Clone

### Technologies used:

Language:

-   Typescript

Full Stack Framework:

-   Next.js 13 with APP folder

Frontend packages:

-   React 18
-   Tailwind CSS (_npm install -D tailwindcss postcss autoprefixer_, _npx tailwindcss init -p_)
-   Cloudinary

Backend packages:

Data Management

-   Prisma (_npm install -D prisma_, _npx prisma init_)

Database

-   MongoDB Atlas

Authentication

-   Auth.js --> But "@next-auth/prisma-adapter" 2023, which is the official primsa adapter for Auth.js / NextAuth.js. (Serves to loggin using several social media profiles/accounts like github, google, facebook, etc.) (npm install next-auth @next-auth/prisma-adapter)

### Key Features

-   Real-time messaging using Pusher
-   Message notifications and alerts
-   Tailwind design for sleek UI
-   Tailwind animations and transition effects
-   Full responsiveness for all devices
-   Credential authentication with NextAuth
-   Google authentication integration
-   Github authentication integration
-   File and image upload using Cloudinary CDN
-   Client form validation and handling using react-hook-form
-   Server error handling with react-toast
-   Message read receipts
-   Online/offline user status
-   Group chats and one-on-one messaging
-   Message attachments and file sharing
-   User profile customization and settings
-   How to write POST, GET, and DELETE routes in route handlers (app/api)
-   How to fetch data in server React components by directly accessing the database (WITHOUT API! like Magic!)
-   Handling relations between Server and Child components in a real-time environment
-   Creating and managing chat rooms and channels

### Instructions

1. Environment setup
2. Auth setup
3. Auth UI
4. MongoDB, Prisma setup
5. NextAuth setup
6. Register Functionality
7. Login Functionality and Social Login (Google and Github)
8. Sidebar, Navigation and Layout
9. Users screen and Conversations screen, Conversation Creation
10. Messages creation, Message Image upload
11. Profile Drawer
12. Settings functionality, Modal component
13. Group chat functionality, Image Modal, Loading states
14. Real time messages, conversations, read receipts and active status with Pusher
15. Deploy to Vercel, fix Google and Github social sign in in deployment

### Prerequisites

**Node version 14.x**

### Cloning the repository

```shell
git clone https://github.com/AntonioErdeljac/next13-messenger.git
```

### Install packages

```shell
npm i
```

### Setup .env file

```js
DATABASE_URL=
NEXTAUTH_SECRET=

NEXT_PUBLIC_PUSHER_APP_KEY=
PUSHER_APP_ID=
PUSHER_SECRET=

NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=

GITHUB_ID=
GITHUB_SECRET=

GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
```

### Setup Prisma

```shell
npx prisma db push

```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command | description                              |
| :------ | :--------------------------------------- |
| `dev`   | Starts a development instance of the app |

## Credits

[Code with Antonio](https://www.youtube.com/watch?v=PGPGcKBpAk8)
