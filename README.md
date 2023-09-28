# Streameo

Streameo is a web-based platform for uploading, streaming, and sharing videos. This project is built using the MERN (MongoDB, Express, React, Node.js) stack and allows users to register, upload videos, and view a list of available videos. When the users click on the video title, the video is streamed 1MB per second.

## Project Description

- **Frontend:** The frontend of the application is developed using React, providing a user-friendly interface for registration, video upload, and video playback.
..

- **Backend:** The backend is powered by Nest.js, a scalable and efficient Node.js framework. It handles user authentication, video storage, and video streaming.
..

- **Database:** MongoDB is used as the database to store user data and video metadata.

## Directory Structure

project_root/  
├── frontend/  
│ ├── public/  
│ ├── src/  
│ │ ├── components/  
│ │ ├── pages/  
│ │ ├── App.js  
│ │ └── ...  
│ ├── package.json  
│ ├── package-lock.json  
│ ├── README.md  
│ └── ...  
├── backend/  
│ ├── src/  
│ │ ├── controllers/  
│ │ ├── middleware/  
│ │ ├── modules/  
│ │ ├── app.module.ts  
│ │ └── ...  
│ ├── package.json  
│ ├── package-lock.json  
│ ├── README.md  
│ └── ...  
├── .gitignore  
├── README.md (This file)  
└── ...  


## Installation Instructions

Follow these steps to set up and run the Video Streaming Application on your local development environment:

### Prerequisites

1. [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) (Node Package Manager) must be installed on your system.

2. [MongoDB](https://www.mongodb.com/) should be installed and running to store user data and video metadata. You can also use MongoDB Atlas at https://www.mongodb.com/

### Backend Setup

Install backend dependencies:

```
Copy code
npm install
```

In /backend/src/utils/constants/ts, add a secret key in line 1:
```
export const secret = '<Enter your secret key here>';
```

In /backend/src/app.module.ts, add your MongoDB connection string in line 22:
```
MongooseModule.forRoot('<Enter your MongoDB connection string here>'),
```

Start the backend server:
```
Copy code
npm start
```

### Backend Setup

Install frontend dependencies:

```
Copy code
npm install
```

Start the frontend development server:

```
Copy code
npm start
Open your web browser and access the application at http://localhost:3000.
```

## Application Usage
* Register a new user account.
* Log in with your newly created account.
* Upload videos with titles and thumbnails.
* View and play videos in the list.
* Log out when finished.

## License
This project is licensed under the MIT License - see the LICENSE file for details.