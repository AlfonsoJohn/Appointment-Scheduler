# Appointment Scheduler Application

A scheduling desktop user interface application.

![App UI](https://imgur.com/Vk2BX0v.jpg)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup](#setup)
- [User Interface](#user-interface)
- [Application Functionality](#application-functionality)
- [Exception Handling](#exception-handling)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Appointment Scheduler App is designed to help users manage their appointments efficiently. It supports multiple languages and adjusts appointment times based on user time zones.

## Features

- **User Authentication:** Secure sign-up and log-in functionalities.
- **Customer Records:** Manage customer records including name, address, and phone number.
- **Appointment Scheduling:** Schedule and maintain appointments with details like type, date, and time.
- **Calendar View:** View appointments by month and by week.
- **Time Zone Adjustments:** Automatically adjust appointment times based on user time zones and daylight saving time.
- **Reminders and Alerts:** Receive reminders and alerts 15 minutes before an appointment.
- **Reports Generation:** Generate reports on appointment types by month, consultant schedules, and custom reports.
- **User Activity Tracking:** Track user activity by recording log-in timestamps in a .txt file.

## Tech Stack

- **Frontend:** JavaFX for building the user interface, Scene Builder for designing the UI.
- **Backend:** Java for backend logic, MySQL for database management, JDBC for database connectivity.

## Setup

1. Clone this repository.
2. Navigate to the project directory.
3. Install dependencies:
   ```bash
   mvn install     # For the backend
   ```
4. Set up the MySQL database and configure the connection settings.

## User Interface

The application includes the following forms:

### Main Form

- **Controls:**
  - Buttons for “Add Appointment,” “Modify Appointment,” “Delete Appointment,” “View Calendar,” and “Log Out”
  - Lists for displaying appointments
  - Text boxes for searching appointments
  - Title labels for appointments and the application title

### Log-in Form

- **Controls:**
  - Text boxes for username and password
  - Buttons for “Log In” and “Sign Up”
  - Labels for username, password, and error messages

### Sign-up Form

- **Controls:**
  - Text boxes for username, password, and confirm password
  - Buttons for “Sign Up” and “Cancel”
  - Labels for username, password, confirm password, and error messages

### Appointment Form

- **Controls:**
  - Text boxes for appointment type, date, and time
  - Drop-downs for selecting customer
  - Buttons for “Save” and “Cancel”
  - Labels for appointment type, date, time, and customer

## Application Functionality

The application includes the following functionalities:

- **Main Form:**
  - Redirect to the “Add Appointment,” “Modify Appointment,” or “View Calendar” forms
  - Delete a selected appointment from the list
  - Search for an appointment and display matching results
  - Log out of the application

- **Log-in Form:**
  - Enter username and password to log in
  - Redirect to the main form upon successful log-in
  - Display error messages for incorrect log-in attempts

- **Sign-up Form:**
  - Enter username, password, and confirm password to sign up
  - Redirect to the log-in form upon successful sign-up
  - Display error messages for sign-up issues

- **Appointment Form:**
  - Enter appointment details like type, date, and time
  - Select a customer from the drop-down
  - Save the appointment and redirect to the main form
  - Cancel or exit out of this form and go back to the main form

## Exception Handling

The application includes exception handling for the following conditions:

- Prevent scheduling an appointment outside business hours
- Prevent scheduling overlapping appointments
- Validate customer data entries
- Display error messages for incorrect username and password
- Confirm “Delete” actions

## Contributing

Contributions are welcome! Feel free to open issues or pull requests.

## License

This project is licensed under the MIT License.
