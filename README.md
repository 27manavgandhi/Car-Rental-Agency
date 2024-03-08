## Car Rental System

This project is a web application designed for a car rental agency to manage their inventory and bookings. It allows two types of users: Customers and Car Rental Agencies. Customers can browse available cars and book them for rental, while agencies can add new cars and view bookings.

### Features

### Features

- Separate registration and login pages for Customers and Car Rental Agencies.
- Car Rental Agencies can add new cars with details such as vehicle model, number, seating capacity, and rent per day.
- Car Rental Agencies can edit details of existing cars.
- Display of available cars for rent to all users.
  - Details include vehicle model, number, seating capacity, and rent per day.
  - Customers can select the number of days and start date for rental.
  - Rent Car button allows customers to book available cars.
  - If not logged in, customers will be redirected to the login page.
  - Agencies cannot book cars.
- Car Rental Agencies can view the list of customers who have booked a particular car added by them.

### Technologies Used

- Frontend: HTML, CSS, JavaScript
  - Bootstrap for responsive design
- Backend: PHP (Core PHP or CodeIgniter)
- Database: MySQL

### Project Structure

- `index.html`: Landing page with options to register or login.
- `customer_registration.html`: Registration page for customers.
- `agency_registration.html`: Registration page for car rental agencies.
- `customer_login.html`: Login page for customers.
- `agency_login.html`: Login page for car rental agencies.
- `add_car.html`: Form for car rental agencies to add new cars.
- `available_cars.html`: Display of available cars with options for customers to rent.
- `view_booked_cars.html`: Page for car rental agencies to view booked cars.

### Database Schema

- **Users**
  - `user_id` (Primary Key)
  - `username`
  - `password`
  - `user_type` (Customer or Agency)

- **Cars**
  - `car_id` (Primary Key)
  - `agency_id` (Foreign Key to Users)
  - `vehicle_model`
  - `vehicle_number`
  - `seating_capacity`
  - `rent_per_day`

- **Bookings**
  - `booking_id` (Primary Key)
  - `car_id` (Foreign Key to Cars)
  - `customer_id` (Foreign Key to Users)
  - `start_date`
  - `number_of_days`

### How to Run

1. Clone the repository to your local machine.
2. Import the SQL file to set up the database.
3. Configure the database connection in the backend PHP files.
4. Run the project using a local server environment (e.g., XAMPP).



---
