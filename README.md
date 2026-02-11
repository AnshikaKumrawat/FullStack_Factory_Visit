# Visit Factory Project
This is a full-stack web application for managing office visits.  
It contains:
- Backend: Java Spring Boot REST API  
- Frontend: Angular application

## Backend (Java / Spring Boot)
1. Open Eclipse IDE 
2. Import the project from `Backend` folder:  
   - File → Import → Existing Maven Project → select `backend` folder  
3. Run as Spring Boot App  
4. Server runs on: `http://localhost:8080`  

### Backend API Endpoints
Base URL: `http://localhost:8080/api/bookings`

#### Create Booking (POST)
POST http://localhost:8080/api/bookings
  Saves booking to the database
  Generates a QR code with URL: http://localhost:4200/qr/{bookingId}
  Sends email to the user with the QR code
  Returns saved booking as JSON

#### get Booking (GET)
GET http://localhost:8080/api/bookings/{id}
  Fetch booking by ID
  Returns JSON object of the booking

## Frontend (Angular)
1.Open VS Code
2.Navigate to the frontend folder
3.Install dependencies:
  npm install
4.Run Angular application:
 ng serve
5.Frontend runs on: http://localhost:4200
6.Connects to backend API at: http://localhost:8080/api/bookings
