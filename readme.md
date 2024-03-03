# Postaway - A Social Networking Platform

## Project Overview

Postaway is a feature-rich Social Networking Platform built using Express and Node.js, incorporating various libraries like JsonWebToken for authentication and Multer for handling file uploads. The application allows users to sign up, create posts, like and comment on posts, bookmark favorites, and more.

## Overview of Functionality

- *Project Architecture:** Follows a API based architecture. Each feature contains dedicated Model, Controller and Router script files for organized and scalable development.
- **User Authentication:** Implements user sign-in and sign-up functionality with JSON Web Tokens (JWT).
- **Post Management:** Provides endpoints for creating, updating, deleting, fetching posts and many other features.
- **Like and Comment System:** Allows users to like and comment on posts.
- **Search and Sorting:** Includes endpoints for filtering and sorting posts based on user preferences.

## Key Features

- **User Authentication:** Secure user authentication with JWT to protect sensitive information.
- **Post Operations:** CRUD operations for posts, including creation, update, delete, and fetching.
- **Like System:** Users can like posts, and the count is tracked for each post.
- **Commenting:** Allows users to add comments to posts, fostering engagement.
- **Search and Sort:** Provides functionality to filter and sort posts for a personalized experience.


## API Details

### Routes

- **User Authentication:**
  - Sign In: `POST /api/signin`
  - Sign Up: `POST /api/signup`
 
- **Swagger UI:**
  - Swagger UI Url: `/api-docs/`

- **Post Operations:**
  - Get All Posts: `GET /api/posts/all`
  - Get User Posts: `GET /api/posts/`
  - Create Post: `POST /api/posts/`
  - Get One Post: `GET /api/posts/{postId}`
  - Delete Post: `DELETE /api/posts/{postId}`
  - Update Post: `PUT /api/posts/{postId}`
  - Filter Posts: `POST /api/posts/filter`
  - Sort Posts: `GET /api/posts/custom/sort`

- **Like System:**
  - Get Post Likes: `GET /api/likes/{postId}`
  - Toggle Like: `GET /api/likes/toggle/{postId}`

- **Comment System:**
  - Get Post Comments: `GET /api/comments/{postId}`
  - Add Comment: `POST /api/comments/{postId}`
  - Delete Comment: `DELETE /api/comments/{commentId}`
  - Update Comment: `PUT /api/comments/{commentId}`


### Middleware

- **Authentication:** Secures endpoints with JWT authentication.
- **Error Page:** Handles invalid routes and errors by displaying the custom error message.
- **File Upload:** Manages image uploads using Multer middleware.

## Project Setup

To run the project locally, follow these steps:

1. Download the zip file
2. Navigate to the project directory: `cd postaway`
3. Install dependencies: `npm install`
4. Start the server: `npm start` or use `nodemon` for development: `npm run dev`

