# Rental Hub

## Project Overview
Rental Hub is a web-based platform designed to streamline the rental process for properties. It connects landlords with potential tenants, providing a user-friendly experience for both parties.

## Features
- **User Authentication**: Secure login and registration for landlords and tenants.
- **Property Listings**: Display properties available for rent with detailed descriptions and images.
- **Search and Filter**: Easy search functionality with various filters for location, price, and more.
- **Booking Management**: Landlords can manage bookings and tenants can view their booking history.
- **Reviews and Ratings**: Tenants can leave reviews for properties to help others in their search.

## Tech Stack
- **Frontend**: React.js
- **Backend**: Node.js with Express.js
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **Deployment**: Heroku / AWS

## Installation Instructions
1. Clone the repository:  `git clone https://github.com/SaucySalamander1/Rental-hub-`
2. Navigate to the project directory: `cd Rental-hub-`
3. Install dependencies for the backend: `npm install` (in the `/backend` directory)
4. Install dependencies for the frontend: `npm install` (in the `/frontend` directory)
5. Create a `.env` file in the `/backend` directory and set your environment variables.
6. Run the backend server: `npm start` (in the `/backend` directory)
7. Run the frontend server: `npm start` (in the `/frontend` directory)

## Project Structure
```
/Rental-hub-
    ├── /frontend    # Frontend code
    ├── /backend     # Backend code
    ├── .env         # Backend environment variables
    └── README.md    # Project documentation
```

## Database Models
- **User**: Contains user details such as name, email, password (hashed), role (landlord/tenant).
- **Property**: Contains property details such as address, price, description, images, and landlord ID.
- **Booking**: Contains booking details such as property ID, user ID, booking dates, and status.
- **Review**: Contains review details such as property ID, user ID, rating, and review text.

## API Routes
- **GET /api/properties**: Retrieve a list of properties.
- **POST /api/properties**: Create a new property (Landlords only).
- **GET /api/users/:id**: Get user details.
- **POST /api/auth/login**: User login.
- **POST /api/auth/register**: User registration.
- **POST /api/bookings**: Create a new booking.

## Setup Guidelines
1. Ensure you have MongoDB installed and running.
2. Set up your environment variables in the `.env` file for the backend.
3. Follow the installation instructions to get the app running locally.
4. For production setup, consider using Heroku or AWS for hosting the app.

## Contribution
Contributions are welcome! Please open an issue or submit a pull request for any changes you'd like to make.

## License
This project is licensed under the MIT License.