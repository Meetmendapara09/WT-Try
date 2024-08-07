# Web Technology - Course Website Project

## Project Overview
This project is a comprehensive course website offering both free and premium courses, featuring coin-based rewards, payment integration, authentication, and user progress tracking. It's built using Angular for the frontend and PHP with MySQL for the backend.

**CSE-D** 
## Team Members
- **Meet Mendapara [IU2241230422]**
- **Prince Ghoda [IU2241230392]**

## Table of Contents
1. [Features](#features)
2. [Technology Stack](#technology-stack)
3. [Project Structure](#project-structure)
4. [Setup and Installation](#setup-and-installation)
5. [Usage](#usage)
6. [API Endpoints](#api-endpoints)
7. [Contributing](#contributing)
8. [License](#license)

## Features
- Home Page with featured, latest, and popular courses, testimonials, and blog highlights.
- User Authentication including login/signup and OAuth integration.
- Detailed course pages with instructor details, curriculum, and user reviews.
- User Dashboard for profile management, course progress tracking, coin balance, and settings.
- Payment Integration for purchasing premium courses.
- Progress tracking and coin-based rewards.
- Video player integration.
- Support and FAQ section.
- Blog/News section.
- Admin panel for managing courses, users, payments, and orders.

## Technology Stack
### Frontend
- HTML
- CSS (Tailwind CSS)
- JavaScript/TypeScript
- Angular

### Backend
- PHP
- MySQL
- PhpMyAdmin

## Project Structure
### Backend Directory (PHP)
```

backend/
├── api/
│   ├── courses/
│   ├── auth/
│   ├── users/
│   ├── payments/
│   ├── coins/
│   ├── config/
│   └── index.php
```
### Frontend Directory (Angular)
```
frontend/
├── e2e/
│   ├── src/
│   │   ├── app.e2e-spec.ts
│   │   └── app.po.ts
│   ├── protractor.conf.js
│   └── tsconfig.e2e.json
├── src/
│   ├── app/
│   │   ├── components/
│   │   │   ├── header/
│   │   │   │   ├── header.ts
│   │   │   │   ├── header.html
│   │   │   │   └── header.css
│   │   │   ├── footer/
│   │   │   │   ├── footer.ts
│   │   │   │   ├── footer.html
│   │   │   │   └── footer.css
│   │   │   ├── home/
│   │   │   │   ├── home.ts
│   │   │   │   ├── home.html
│   │   │   │   └── home.css
│   │   │   ├── auth/
│   │   │   │   ├── login/
│   │   │   │   │   ├── login.ts
│   │   │   │   │   ├── login.html
│   │   │   │   │   └── login.css
│   │   │   │   ├── register/
│   │   │   │   │   ├── register.ts
│   │   │   │   │   ├── register.html
│   │   │   │   │   └── register.css
│   │   │   │   └── password-recovery/
│   │   │   │       ├── password-recovery.ts
│   │   │   │       ├── password-recovery.html
│   │   │   │       └── password-recovery.css
│   │   │   ├── courses/
│   │   │   │   ├── course-list/
│   │   │   │   │   ├── course-list.ts
│   │   │   │   │   ├── course-list.html
│   │   │   │   │   └── course-list.css
│   │   │   │   ├── course-detail/
│   │   │   │   │   ├── course-detail.ts
│   │   │   │   │   ├── course-detail.html
│   │   │   │   │   └── course-detail.css
│   │   │   ├── user-dashboard/
│   │   │   │   ├── profile/
│   │   │   │   │   ├── profile.ts
│   │   │   │   │   ├── profile.html
│   │   │   │   │   └── profile.css
│   │   │   │   ├── my-courses/
│   │   │   │   │   ├── my-courses.ts
│   │   │   │   │   ├── my-courses.html
│   │   │   │   │   └── my-courses.css
│   │   │   │   ├── coin-balance/
│   │   │   │   │   ├── coin-balance.ts
│   │   │   │   │   ├── coin-balance.html
│   │   │   │   │   └── coin-balance.css
│   │   │   │   ├── settings/
│   │   │   │       ├── settings.ts
│   │   │   │       ├── settings.html
│   │   │   │       └── settings.css
│   │   │   ├── payment/
│   │   │   │   ├── checkout/
│   │   │   │   │   ├── checkout.ts
│   │   │   │   │   ├── checkout.html
│   │   │   │   │   └── checkout.css
│   │   │   │   └── order-confirmation/
│   │   │   │       ├── order-confirmation.ts
│   │   │   │       ├── order-confirmation.html
│   │   │   │       └── order-confirmation.css
│   │   │   ├── additional-features/
│   │   │   │   ├── progress-tracking/
│   │   │   │   │   ├── progress-tracking.ts
│   │   │   │   │   ├── progress-tracking.html
│   │   │   │   │   └── progress-tracking.css
│   │   │   │   ├── video-player/
│   │   │   │   │   ├── video-player.ts
│   │   │   │   │   ├── video-player.html
│   │   │   │   │   └── video-player.css
│   │   │   │   ├── support-faq/
│   │   │   │   │   ├── support-faq.ts
│   │   │   │   │   ├── support-faq.html
│   │   │   │   │   └── support-faq.css
│   │   │   │   └── blog-news/
│   │   │   │       ├── blog-news.ts
│   │   │   │       ├── blog-news.html
│   │   │   │       └── blog-news.css
│   │   │   ├── admin-panel/
│   │   │   │   ├── course-management/
│   │   │   │   │   ├── course-management.ts
│   │   │   │   │   ├── course-management.html
│   │   │   │   │   └── course-management.css
│   │   │   │   ├── user-management/
│   │   │   │   │   ├── user-management.ts
│   │   │   │   │   ├── user-management.html
│   │   │   │   │   └── user-management.css
│   │   │   │   ├── payments-orders/
│   │   │   │   │   ├── payments-orders.ts
│   │   │   │   │   ├── payments-orders.html
│   │   │   │   │   └── payments-orders.css
│   │   ├── app.component.html
│   │   ├── app.component.css
│   │   ├── app.component.ts
│   │   ├── app.module.ts
│   │   └── app-routing.module.ts
│   ├── assets/
│   │   ├── images/
│   │   ├── styles/
│   │   │   ├── tailwind.css
│   │   │   ├── main.css
│   │   └── scripts/
│   ├── environments/
│   │   ├── environment.ts
│   │   └── environment.prod.ts
│   ├── index.html
│   ├── main.ts
│   ├── polyfills.ts
│   ├── styles.css
│   └── tsconfig.app.json
```
## Setup and Installation

### Prerequisites
- Node.js and npm
- Angular CLI
- PHP
- MySQL
- PhpMyAdmin

### Backend (PHP) Setup
1. Clone the repository:
  
   git clone https://github.com/Meetmendapara09/WT-Try.git
   <br/>cd course-website/backend

2. Set up the database:
   - Create a database named `course_website`.
   - Import `backend/config/db.sql` into your MySQL database.
3. Update database configuration in `backend/config/db.php`.
4. Start the PHP server:
   `
   php -S localhost:8000
   `

### Frontend (Angular) Setup
1. Navigate to the frontend directory:
   `
   cd ../frontend
   `
2. Install dependencies:
   `
   npm install
   `
3. Start Angular development server:
   `
   ng serve
   `

## Usage
- Access frontend at `http://localhost:4200`.
- Backend API is available at `http://localhost:8000`.

## API Endpoints
### Authentication
- `POST /api/auth/login`: User login
- `POST /api/auth/register`: User registration
- `POST /api/auth/passwordRecovery`: Password recovery

### Courses
- `GET /api/courses/getCourses`: List courses
- `GET /api/courses/getCourseDetails`: Course details
- `POST /api/courses/addCourse`: Add a course
- `PUT /api/courses/updateCourse`: Update a course
- `DELETE /api/courses/deleteCourse`: Delete a course

### Users
- `GET /api/users/getUser`: Get user details
- `PUT /api/users/updateUser`: Update user info
- `DELETE /api/users/deleteUser`: Delete a user

### Payments
- `POST /api/payments/processPayment`: Process payment
- `GET /api/payments/getPaymentHistory`: Payment history

### Coins
- `GET /api/coins/getCoinBalance`: Get coin balance
- `PUT /api/coins/updateCoinBalance`: Update coin balance

## Contributing
Contributions are welcome! Fork this repository and submit a pull request.

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
