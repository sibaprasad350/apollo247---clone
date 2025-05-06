# apollo247---clone
The Apollo247 Clone is a web application that mimics the General Physician/Internal Medicine page from Apollo247. It enables users to view a list of doctors, apply filters for searching doctors, and view doctor details such as specialty, location, and rating.

A clone of the [Apollo247 General Physician/Internal Medicine page](https://www.apollo247.com/specialties/general-physician-internal-medicine), featuring doctor listings with filtering and pagination. Built using Next.js for the frontend and Node.js with MongoDB for the backend.

## Project Structure
apollo247-clone/
├── backend/
│ ├── models/Doctor.js
│ ├── routes/doctorRoutes.js
│ ├── server.js
│ └── .env
├── frontend/
│ ├── pages/specialties/general-physician-internal-medicine.js
│ ├── components/Header.js
│ ├── components/Filters.js
│ ├── components/DoctorCard.js
│ └── next.config.js
└── README.md


## Features

- **Doctor Listing**: Displays doctors with details like name, specialty, location, and rating.
- **Filters**: Allows filtering by specialty, location, and rating.
- **Pagination**: Navigate through doctor listings with pagination.
- **APIs**: 
  - `POST /api/doctors/add-doctor`: Add new doctors.
  - `GET /api/doctors/list-doctor-with-filter`: List doctors with optional filters.

## Technologies

- **Frontend**: Next.js, Axios
- **Backend**: Node.js, Express, MongoDB, Mongoose

## Setup

1. **Backend**:
   - Go to the `backend/` directory.
   - Run `npm install`.
   - Create `.env` with MongoDB URI (`DB_URI=mongodb://localhost:27017/doctorDB`).
   - Run `node server.js`.

2. **Frontend**:
   - Go to the `frontend/` directory.
   - Run `npm install`.
   - Run `npm run dev`.

Visit the frontend at `http://localhost:3000` and the backend at `http://localhost:3001`.

## API Endpoints

- **POST /api/doctors/add-doctor**: Add a doctor.
- **GET /api/doctors/list-doctor-with-filter**: List doctors with filters (`page`, `specialty`, `location`, `rating`).

## 🚀 Deployment
Frontend (Vercel):

Push frontend/ to a GitHub repository.

Go to Vercel and import the project.

Set environment variables if needed.

Deploy the project.

Backend (Render):

Push backend/ to a GitHub repository.

Go to Render and create a new Web Service.

Set the build and start commands:

Build Command: npm install

Start Command: node server.js

Add environment variable MONGODB_URI with your MongoDB connection string.

Deploy the service.



## License

MIT License

