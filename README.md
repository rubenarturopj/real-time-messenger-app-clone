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
-   Tailwind CSS Forms (_npm i @tailwindcss/forms_)
-   Cloudinary (package and CDN) API (_https://cloudinary.com/_, _npm install next-cloudinary_)
-   React-icons
-   React-hook-form
-   clsx: A tiny (228B) utility for constructing className strings conditionally. (_npm install --save clsx_)

Backend packages:

Data Management

-   Prisma (_npm install -D prisma_, _npx prisma init_)

Database

-   MongoDB Atlas

Authentication

-   Auth.js --> But "@next-auth/prisma-adapter" 2023, which is the official primsa adapter for Auth.js / NextAuth.js. (Serves to loggin using several social media profiles/accounts like github, google, facebook, etc.) (npm install next-auth @next-auth/prisma-adapter)

Real time messaging and notifications

-   Pusher

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

1. [Environment setup](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/01_environment_setup.md)
2. [Auth setup](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/02_auth.md)
3. [Auth UI](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/03_auth_UI.md)
4. [MongoDB, Prisma setup](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/04_mongodb_prisma.md)
5. [NextAuth setup](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/05_nextauth.md)
6. [Register Functionality](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/06_register.md)
7. [Login Functionality and Social Login (Google and Github)](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/07_login.md)
8. [Sidebar, Navigation and Layout](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/08_sidebar_navigation_layout.md)
9. [Users screen and Conversations screen, Conversation Creation](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/09_user_screen_conversations_screen.md)
10. [Messages creation, Message Image upload](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/10_messenger_creation_message_image.md)
11. [Profile Drawer](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/11_profile_drawer.md)
12. [Settings functionality, Modal component](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/12_settings_func_modal.md)
13. [Group chat functionality, Image Modal, Loading states](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/13_group_chat_imagemodal_loadingstate.md)
14. [Real time messages, conversations, read receipts and active status with Pusher](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/14_real_time_messages_conversations.md)
15. [Deploy to Vercel, fix Google and Github social sign in in deployment](https://github.com/rubenarturopj/real-time-messenger-app-clone/blob/main/01_instructions/15_deploy_vercel_github_google_auth.md)

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
