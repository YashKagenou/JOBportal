# Job Portal Application

A full-stack job portal application built using the MERN stack (MongoDB, Express.js, React.js, and Node.js). The platform connects recruiters and job seekers through dedicated dashboards, allowing recruiters to manage job postings and applicants to explore opportunities and track applications.

## Screenshots

![Job Portal Application](./Prodigy.gif)

## Features

### Recruiters / Companies
- Create and manage job postings.
- View applications received for posted jobs.
- Access a dashboard for job and application management.
- Customize company profiles.

### Applicants
- Search and filter available job listings.
- Apply for jobs with resume/CV submission.
- Track application statuses.
- Manage applicant profiles.

### General
- Authentication using Clerk.
- Error monitoring with Sentry.
- File uploads through Cloudinary.
- Responsive user interface using Tailwind CSS.
- RESTful APIs with JWT-based authentication.

## Tech Stack

### Frontend
- React.js (Vite)
- Tailwind CSS
- React Router
- Axios
- Chart.js

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)
- Bcrypt
- CORS
- Svix (Webhooks)

### Third-Party Services
- Clerk – Authentication
- Sentry – Error Tracking
- Cloudinary – File Storage

## Getting Started

### Prerequisites
- Node.js (v18 or later)
- MongoDB Atlas account
- Clerk account
- Sentry account
- Cloudinary account

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/YashKagenou/JOBportal.git
cd JOBportal
```

**2. Install frontend dependencies**

```bash
cd client
npm install
```

**3. Install backend dependencies**

```bash
cd ../server
npm install
```

### Environment Variables

Create a `.env` file inside the `server` directory:

```env
MONGODB_URI=your_mongodb_uri
CLERK_SECRET_KEY=your_clerk_secret_key
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
SENTRY_DSN=your_sentry_dsn
CLERK_WEBHOOK_SECRET=your_webhook_secret
PORT=5000
```

Create a `.env` file inside the `client` directory:

```env
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
VITE_API_BASE_URL=http://localhost:5000/api
```

### Running the Application

**Start the backend**

```bash
cd server
npm run dev
```

**Start the frontend in a separate terminal**

```bash
cd client
npm run dev
```

The frontend will be available at the local development URL displayed by Vite.


## License

Refer to the original repository's LICENSE file for applicable licensing terms and permissions. Original copyright and attribution notices must be retained as required by the applicable license.