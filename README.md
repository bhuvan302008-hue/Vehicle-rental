# DriveSphere VRMS – Vehicle Rental Management System

## 1. Project Overview

DriveSphere VRMS is a web-based Vehicle Rental Management System developed to simplify the process of renting two-wheelers and four-wheelers.

The website allows customers to browse available vehicles, check rental prices, select pickup and return dates, and book vehicles. It also provides an Admin Dashboard to manage vehicle inventory and customer reservations.

The project is designed with a user-friendly interface and responsive layout.

## 2. Project Objectives

- To develop an interactive vehicle rental website.
- To provide an easy vehicle booking facility.
- To display vehicle details and rental prices.
- To calculate rental charges automatically.
- To generate GST invoices.
- To provide an admin dashboard for managing vehicles and bookings.
- To store booking information using browser Local Storage.

## 3. Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Website structure |
| CSS3 | Styling and layout |
| JavaScript | Functionality and interactivity |
| Tailwind CSS | Responsive user interface |
| Local Storage | Storing vehicle and booking data |
| Visual Studio Code | Code editor |

## 4. Main Features

### Customer Portal
- Browse available bikes, scooters, cars and SUVs.
- Search vehicles by model name.
- Filter vehicles by category.
- Select pickup and return dates.
- Choose pickup locations in Bengaluru.
- View vehicle specifications and rental prices.
- Book vehicles using customer details.

### Booking and Billing
- Automatic rental fare calculation.
- Optional rental add-ons.
- Promotional discount codes:
  - `STUDENT15` – 15% discount.
  - `FIRST100` – ₹100 discount.
- Automatic GST calculation (18%).
- GST invoice generation.
- Print or save invoices as PDF.

### Admin Dashboard
- View total revenue.
- View active bookings.
- Check available vehicles.
- Monitor fleet utilization.
- Add new vehicles.
- Edit existing vehicle details.
- Delete vehicle records.
- Manage booking status.
- Reset demonstration data.

### Additional Features
- Responsive website design.
- Customer and Admin role switching.
- My Bookings section.
- Vehicle availability management.
- Browser Local Storage for data persistence.
- Project documentation and database schema information.

## 5. Vehicle Categories

The system includes the following categories:

1. Bikes and Scooters
2. Basic Cars
3. Sedan
4. SUV
5. Electric Vehicles

The initial fleet contains 12 vehicles.

## 6. Project Structure

```text
DriveSphere-VRMS/
│
├── index.html
└── README.md
```

The project is implemented in a single HTML file containing HTML, CSS and JavaScript code.

## 7. Installation and Execution

Follow these steps to run the project:

1. Install Visual Studio Code.
2. Create a folder named `DriveSphere-VRMS`.
3. Open the folder in Visual Studio Code.
4. Create a file named `index.html`.
5. Paste the project source code into the file.
6. Save the file.
7. Open `index.html` in your web browser.

Alternatively, use the Live Server extension in Visual Studio Code to run the website.

**Note:** An internet connection is required for Tailwind CSS CDN and externally hosted vehicle images. The project also includes basic CSS fallback styling.

## 8. Data Storage

The project uses the browser's Local Storage to store information.

The following storage keys are used:

- `drivesphere_vrms_v3_vehicles`
- `drivesphere_vrms_v3_bookings`
- `drivesphere_vrms_v3_user`

The stored information remains available in the same browser unless the browser data is cleared or the demonstration data is reset.

## 9. Database Design

The project documentation includes a relational database schema based on Third Normal Form (3NF).

### VEHICLES Table
- vehicle_id (Primary Key)
- model_name
- category
- daily_rate
- license_class
- status

### BOOKINGS Table
- booking_id (Primary Key)
- vehicle_id (Foreign Key)
- customer_name
- dl_number
- pickup_date
- return_date
- gst_amount
- grand_total
- booking_status

**Note:** These tables describe the proposed relational database design. The current implementation uses browser Local Storage rather than a connected SQL database.

## 10. Future Enhancements

- User registration and login system.
- Online payment gateway integration.
- MySQL database connectivity.
- Real-time vehicle availability.
- Email and SMS booking notifications.
- GPS-based vehicle tracking.
- Customer feedback and rating system.

## 11. Conclusion

DriveSphere VRMS provides a simple and interactive platform for vehicle rentals. It demonstrates the practical implementation of HTML, CSS and JavaScript concepts, including dynamic content rendering, booking management, fare calculation, invoice generation and CRUD operations.

This project helps demonstrate the application of web development concepts in solving a real-world vehicle rental management problem.

---

**Project Name:** DriveSphere VRMS  
**Project Type:** First Semester Mini Project  
**Domain:** Web Development  
**Developed Using:** HTML, CSS, JavaScript and Tailwind CSS
