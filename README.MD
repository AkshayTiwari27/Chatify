# Chatify ✨

A feature-rich, real-time chat application built with the MERN stack. This project showcases a complete full-stack implementation, from custom authentication to real-time messaging and email notifications.

## 🚀 Highlights

  * 🔐 **Custom JWT Authentication:** Secure, stateless authentication without relying on third-party services.
  * ⚡ **Real-time Messaging:** Instantaneous communication powered by Socket.io.
  * 🟢 **Online/Offline Presence Indicators:** See the real-time status of other users.
  * 🔔 **Notification & Typing Sounds:** Engaging user experience with optional audio cues.
  * 📨 **Welcome Emails on Signup:** Automated welcome emails using Resend.
  * 🗂️ **Image Uploads:** Seamlessly upload and share images with Cloudinary.
  * 🧰 **RESTful API:** A robust backend built with Node.js and Express.
  * 🧱 **MongoDB for Data Persistence:** Scalable and flexible NoSQL database.
  * 🚦 **API Rate-Limiting:** Powered by Arcjet to prevent abuse.
  * 🎨 **Beautiful UI:** A modern and responsive user interface built with React, Tailwind CSS, and DaisyUI.
  * 🧠 **Zustand for State Management:** Simple and powerful state management for React.
  * 🧑‍💻 **Git & GitHub Workflow:** Best practices for version control with branches, PRs, and merges.
  * 🚀 **Easy Deployment:** Free-tier friendly and easy to deploy with services like Sevalla.
  * 🧪 **.env Setup:** Simple configuration for a smooth development experience.

-----

## 🛠️ Tech Stack

| Frontend | Backend | Database |
| :--- | :--- | :--- |
| React | Node.js | MongoDB |
| Tailwind CSS | Express | |
| DaisyUI | Socket.io | |
| Zustand | JWT | |
| Axios | Resend | |
| | Cloudinary | |
| | Arcjet | |

-----

## 🏁 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

  * Node.js (v20.0.0 or higher)
  * npm
  * MongoDB account
  * Cloudinary account
  * Resend account
  * Arcjet account

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/akshaytiwari27/chatify.git
    cd chatify
    ```
2.  **Install backend dependencies:**
    ```sh
    cd backend
    npm install
    ```
3.  **Install frontend dependencies:**
    ```sh
    cd ../frontend
    npm install
    ```

-----

## ⚙️ Configuration

Create a `.env` file in the `backend` directory and add the following environment variables:

```env
PORT=3000
MONGO_URI=your_mongo_uri_here

NODE_ENV=development

JWT_SECRET=your_jwt_secret

RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=your_email_from_address
EMAIL_FROM_NAME=your_email_from_name

CLIENT_URL=http://localhost:5173

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

ARCJET_KEY=your_arcjet_key
ARCJET_ENV=development
```

-----

## 🏃‍♂️ Running the Application

1.  **Run the backend:**
    ```sh
    cd backend
    npm run dev
    ```
2.  **Run the frontend:**
    ```sh
    cd ../frontend
    npm run dev
    ```

The application will be available at `http://localhost:5173`.

-----

## 📝 API Endpoints

### Authentication

  * `POST /api/auth/signup`: Create a new user account.
  * `POST /api/auth/login`: Log in a user.
  * `POST /api/auth/logout`: Log out a user.
  * `PUT /api/auth/update-profile`: Update a user's profile.
  * `GET /api/auth/check`: Check if a user is authenticated.

### Messaging

  * `GET /api/messages/contacts`: Get all contacts.
  * `GET /api/messages/chats`: Get all chat partners.
  * `GET /api/messages/:id`: Get messages with a specific user.
  * `POST /api/messages/send/:id`: Send a message to a specific user.

-----

## 🚀 Deployment

This application is designed to be easily deployable on free-tier services like Sevalla. The `package.json` at the root of the project contains the necessary scripts for building and starting the application.

```json
"scripts": {
  "build": "npm install --prefix backend && npm install --prefix frontend && npm run build --prefix frontend",
  "start": "npm run start --prefix backend"
}
```

## 📜 License

This project is licensed under the MIT License.
