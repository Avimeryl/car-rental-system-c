# 🚗 Car Rental System

A console-based Car Rental Management System in C, designed to manage cars, bookings, schedules, and reports efficiently. It supports full CRUD operations, real-time availability checks, rental receipts, and monthly reports.

# ✨ Features

✅ Car Management

Add new cars with details (brand, model, seat capacity, engine, transmission, year, color, rent/day, plate no., availability)

View the car menu

Update specific car details

Delete cars from the system

✅ Booking Management

Create new bookings with customer details

Validate car availability & license type

Check for date conflicts to prevent double-booking

Auto-calculate rental cost, deposit, and remaining balance

Generate a Booking Receipt

Edit or delete bookings using MyCard ID

View all bookings in a formatted list

✅ Scheduling & Reports

Rental Schedule → View collection & return dates for each car

Car Rental Report → Monthly rental history per car type

Summary Report → Total rental revenue for all cars in the current month

✅ Data Validation & Safety

Uses temporary files for safe updates (tempfile.txt, Temporarystorefile.txt)

Ensures no data corruption during edits/deletions

Validates inputs (e.g., prevents renting unavailable/manual cars for DA licenses)

# 🏗️ Project Structure

CarRentalSystem/
├── carfile.txt        # Stores car details
├── custfile.txt       # Stores customer booking details
├── tempfile.txt       # Temporary file for booking updates
├── Temporarystorefile.txt  # Temporary file for car updates
└── car_rental.c       # Main source code

# 🖥️ Usage

1. Main Menu

========== Car Rental System ==========
1. Manage Car Booking
2. Manage Car Menu
3. Scheduling of the Rental
4. View Reports
5. Exit

2. Manage Car Menu

- Add a new car

- Edit car details

- Remove a car

- Display all cars

3. Manage Bookings

- Place new booking

- Edit booking

- Delete booking

- Display all bookings

4. Scheduling & Reports

- View rental schedules (who booked which car and when)

- Monthly rental reports per car

- Monthly summary report (total revenue)

🧾 Example Booking Receipt

===== Car Booking Receipt =====

Name of customer: John Doe
Booking date(day): 25/07/2025
Collection date(time): 27/07/2025
Duration: 3 day(s)
Licence Type: D
Contact Number: 012-3456789
MyCard ID: 123456789012
Deposit: RM100.0
Type of car: 2 - Toyota Vios
Rent per day: RM120
Total amount to be paid: RM360
Balance to be paid: RM260.00
===============================

# 📊 Example Reports

✅ Monthly Summary Report

Monthly Summary Report (07/2025)

Branch Location: Kuching

Plate No.    Car Brand/Model    Rate/Day(RM)    Total Days    Subtotal
ABC1234      Toyota Vios        120            15            1800
XYZ5678      Honda City         130            10            1300

Total: RM3100

✅ Car Rental Schedule

Monthly Car Rental Schedule (07/2025)

No. Plate: ABC1234

Customer Name   Collection Date   Return Date
John Doe        27/07/2025        30/07/2025
Jane Smith      01/08/2025        04/08/2025

# ⚙️ Tech Stack

Language: C

File Storage: Binary files (.txt) for cars & customers

OS-specific: Uses windows.h and unistd.h for timing

# 🚀 How to Run

1. Compile the code

gcc car_rental.c -o car_rental


2. Run the program

./car_rental


# 👨‍💻 Authors

Ibnu Ameerul Bin Abdul Halim (78038)

Lau Ung Hien (79822)

Christa Tracy Mojikon (77903)

Pretty Malthasia Anak Lingeh (78484)

Muhammad Norqhaiziq Bin Maharuf (80270)

Created on 29/11/2021 – Last Modified 10/01/2022


# 📌 Future Improvements

Replace text file storage with a database (SQLite/MySQL)

Add a GUI version for easier navigation

Implement login system & roles (Admin/User)

Integrate payment gateway simulation

Improve date handling using a proper date library
