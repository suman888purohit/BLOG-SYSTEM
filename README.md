# 📝 Social Blog Platform - Task 5 Complete

A fully-featured blog platform with social networking capabilities built with PHP, MySQL, Bootstrap, and JavaScript.

## ✨ Features Implemented

### 📋 Core Blog Features
- **CRUD Operations**: Create, Read, Update, Delete blog posts
- **User Authentication**: Secure login/registration system
- **Role-Based Access**: Admin/Editor/User roles with different permissions
- **Search Functionality**: Search posts by title or content
- **Pagination**: Browse posts with page navigation
- **File Attachments**: Upload images/documents with posts

### ❤️ Engagement Features
- **Like System**: Like/unlike posts with real-time counters
- **Comment System**: Comment on posts with user attribution
- **Profile Management**: 
  - Edit profile information (bio, location, website)
  - Upload/change profile pictures
  - View post history

### 👥 Social Features
- **Follow System** (Instagram/Twitter style):
  - Follow/unfollow other users
  - View followers/following counts
  - See follower/following lists
  - Real-time updates

- **Direct Messaging**:
  - One-on-one conversations
  - Real-time message updates (polling)
  - Unread message notifications
  - Message read status (sent/delivered/read)
  - Search users to start conversations
  - Conversation history

### 🎨 Design Features
- **Modern UI/UX**: Clean design with gradient effects
- **Responsive Design**: Mobile-friendly layout
- **Interactive Elements**: Hover effects, animations
- **Custom Color Scheme**: Red/orange theme

## 🏗️ Technology Stack

- **Backend**: PHP 7.4+
- **Database**: MySQL 5.7+
- **Frontend**: HTML5, CSS3, JavaScript
- **CSS Framework**: Bootstrap 5.3.2
- **Icons**: Bootstrap Icons 1.11.1
- **Fonts**: Google Fonts (Inter)
- **AJAX**: Real-time message updates

## 📊 Database Schema

### Users Table
```sql
- id (INT, PRIMARY KEY)
- username (VARCHAR)
- email (VARCHAR)
- password (VARCHAR)
- role (ENUM: 'admin', 'editor', 'user')
- bio (TEXT)
- location (VARCHAR)
- website (VARCHAR)
- profile_picture (VARCHAR)
- joined_at (TIMESTAMP)

post table 
- id (INT, PRIMARY KEY)
- user_id (INT, FOREIGN KEY)
- title (VARCHAR)
- content (TEXT)
- file_path (VARCHAR)
- created_at (TIMESTAMP)

