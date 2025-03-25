# Law Firm Website - Zafer Tağa

![License: Commercial](https://img.shields.io/badge/License-Commercial-orange)
![React](https://img.shields.io/badge/React-19.0.0-blue)
![MongoDB](https://img.shields.io/badge/MongoDB-8.12.1-green)
![Express](https://img.shields.io/badge/Express-4.21.2-lightgrey)


**⚠️ NOTE:** This repository contains **no source code** as it's a proprietary commercial project.

**⚠️ The project will be deployed when the final features are developed.**

---

## 📋 Project Overview

This project is a full-stack lawyer website and content management system for Attorney Zafer Tağa's law firm based in Aydın, Turkey. The application includes a public-facing website with information about legal services and a secure admin area for managing blog posts and user accounts.


![1](https://github.com/user-attachments/assets/6949bd71-75fc-4031-8955-c2598ed0bd29)


### 🌐 Features

- **Public Website:**
  - Home page with hero section, services overview, and client testimonials
  - About page with lawyer information and firm values
  - Services pages with detailed descriptions of legal services
  - Blog system with categorized articles
  - Contact form with email integration
  - FAQ section
  - Mobile-responsive design

- **Admin Dashboard:**
  - User authentication (JWT-based)
  - Google OAuth integration
  - Blog post creation and management
  - User management system
  - Analytics dashboard
  - Profile management

## 🏗️ Architecture

The project follows the MERN stack architecture:

- **Frontend:** React.js with React Router for client-side routing
- **Backend:** Node.js with Express.js
- **Database:** MongoDB with Mongoose ODM
- **Authentication:** JWT and Google OAuth
- **File Storage:** Cloudinary for image uploads
- **Styling:** Tailwind CSS

## 🚀 Technologies Used

### Frontend
<table>
  <tr>
    <td><img src="https://img.shields.io/badge/-React-61DAFB?style=flat&logo=react&logoColor=black" alt="React" width="100"/></td>
    <td><img src="https://img.shields.io/badge/-Redux-764ABC?style=flat&logo=redux&logoColor=white" alt="Redux" width="100"/></td>
    <td><img src="https://img.shields.io/badge/-Tailwind-38B2AC?style=flat&logo=tailwind-css&logoColor=white" alt="Tailwind" width="100"/></td>
    <td><img src="https://img.shields.io/badge/-Firebase-FFCA28?style=flat&logo=firebase&logoColor=black" alt="Firebase" width="100"/></td>
  </tr>
</table>

- ⚛️ **React 19.0.0** - Modern UI library for component-based architecture
- 🌐 **React Router DOM 7.3.0** - Client-side routing solution
- 🔄 **Redux Toolkit & Redux Persist** - Advanced state management with persistence
- 🎨 **Tailwind CSS 4.0.14** - Utility-first CSS framework for custom designs
- 🔥 **Firebase Authentication** - Secure user authentication and Google OAuth
- 📡 **Axios** - Promise-based HTTP client for API requests
- 🔣 **React Icons** - Comprehensive icon library
- 📧 **EmailJS** - Client-side email sending for contact form
- 📊 **React Circular Progressbar** - Interactive visual components

### Backend
<table>
  <tr>
    <td><img src="https://img.shields.io/badge/-Node.js-339933?style=flat&logo=node.js&logoColor=white" alt="Node.js" width="100"/></td>
    <td><img src="https://img.shields.io/badge/-Express-000000?style=flat&logo=express&logoColor=white" alt="Express" width="100"/></td>
    <td><img src="https://img.shields.io/badge/-MongoDB-47A248?style=flat&logo=mongodb&logoColor=white" alt="MongoDB" width="100"/></td>
    <td><img src="https://img.shields.io/badge/-JWT-000000?style=flat&logo=json-web-tokens&logoColor=white" alt="JWT" width="100"/></td>
  </tr>
</table>

- 🟢 **Node.js** - JavaScript runtime for building scalable server-side applications
- 🚂 **Express.js 4.21.2** - Fast, minimalist web framework for Node.js
- 🍃 **MongoDB with Mongoose 8.12.1** - NoSQL database with elegant MongoDB object modeling
- 🔐 **JWT (JSON Web Token)** - Secure method for authentication and information exchange
- 🔒 **bcryptjs** - Library for secure password hashing
- ☁️ **Cloudinary** - Cloud service for image storage and optimization
- 📁 **Multer** - Middleware for handling multipart/form-data for file uploads
- 🔀 **CORS** - Cross-Origin Resource Sharing middleware
- 🔧 **dotenv** - Module for loading environment variables

## 📱 User Interface

### Public Website
- Clean, professional design with dark theme and gold accents
- Responsive layout for all devices
- Intuitive navigation with floating contact buttons
- Blog categorization system
- Contact form with validation

### Admin Dashboard
- Secure login system with Google OAuth option
- Analytics dashboard with user and post statistics
- Blog post editor with image upload
- User management system with admin privileges
- Profile management with profile picture upload

## 📁 Project Structure

### Backend (API)

#### Main Files
- `index.js` - Main server entry point
- `package.json` - Dependencies and scripts

#### API Routes
- `auth.route.js` - Authentication routes (signup, signin, Google auth)
- `post.route.js` - Blog post management
- `upload.route.js` - File upload handling
- `user.route.js` - User management

#### Controllers
- `auth.controller.js` - Authentication logic
- `post.controller.js` - Blog post CRUD operations
- `upload.controller.js` - Cloudinary integration for uploads
- `user.controller.js` - User management operations

#### Models
- `post.model.js` - Blog post schema
- `user.model.js` - User schema

#### Utilities
- `error.js` - Custom error handling
- `verifyUser.js` - JWT verification middleware

### Frontend (Client)

#### Pages
- `Home.jsx` - Landing page
- `About.jsx` - About the lawyer and firm
- `Services.jsx` - Services overview
- `ServicesDetail.jsx` - Individual service details
- `Articles.jsx` - Blog listing page
- `PostPage.jsx` - Individual blog post
- `Contact.jsx` - Contact form
- `FAQ.jsx` - Frequently asked questions
- `Dashboard.jsx` - Admin dashboard
- `SignIn.jsx`/`SignUp.jsx` - Authentication screens
- `CreatePost.jsx`/`UpdatePost.jsx` - Blog post editor

#### Components
- `Navbar.jsx` - Navigation header
- `Footer.jsx` - Site footer
- `FloatingContactButtons.jsx` - Fixed contact buttons
- `HeroSection.jsx` - Homepage hero
- `ServicesSection.jsx` - Services overview
- `Comments.jsx` - Testimonials carousel
- `PostCard.jsx` - Blog post preview card
- Dashboard components:
  - `DashProfile.jsx` - User profile editor
  - `DashSidebar.jsx` - Dashboard navigation
  - `DashPosts.jsx` - Blog post management
  - `DashUsers.jsx` - User management
  - `DashboardComp.jsx` - Analytics overview

#### State Management
- `redux/` folder containing:
  - `store.js` - Redux store configuration with persist
  - `user/userSlice.js` - User authentication state

#### Utilities
- `firebase.js` - Firebase configuration for Google auth
- `ScrollToTop.jsx` - Scroll restoration utility
- `PrivateRoute.jsx`/`OnlyAdminPrivateRoute.jsx` - Route protection





## 👤 Author

This is a proprietary project by Alperen Emre Candan.

## 📄 License

This is a commercial project with all rights reserved. The code is not available for public use or distribution.
