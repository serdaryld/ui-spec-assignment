# User Management Screen UI Specification

## Overview
The User Management screen allows users to view, create, and manage user accounts within the system. This document specifies the requirements and design details for the User Management interface.


## User Interface Layout

1. **Top Bar**: Positioned at the top of the screen.
2. **User Table**: Positioned on the left half of the screen below the top bar.
3. **New User Registration Form**: Positioned on the right half of the screen below the top bar.


## User Interface Components

### Top Bar
- **"+ New User" Button**: Located on the left side of the top bar. Clicking this button opens the new user registration form.
- **"Hide Disabled User" Checkbox**: Also located on the left side. When checked, hides disabled user accounts from the user table.
- **"Save User" Button**: Positioned on the right side of the top bar. Saves changes made to the new user registration form.

### User Table
- **Columns**: The table contains the following columns:
  - **ID**: Represents the unique identifier of each user.
  - **User Name**: Displays the username of each user.
  - **Email**: Shows the email address associated with each user.
  - **Enabled**: Indicates whether the user account is enabled or disabled.
- **Sorting**: Each column header includes an arrow icon to sort the records based on that column. The currently selected sorting parameter displays a single up arrow, while other parameters display both up and down arrows.
- **Filtering**: Each column header includes a filter icon that allows filtering related to that column

### New User Registration Form
- **Title**: Positioned at the top of the form, displaying "New User".
- **Inputs**:
  1. **Username**: Text input field for entering the new user's username.
  2. **Display Name**: Text input field for specifying the display name of the new user.
  3. **Phone**: Text input field for entering the phone number of the new user.
  4. **Email**: Text input field for providing the email address of the new user.
  5. **User Roles**: Dropdown menu triggered by clicking the input field. Options include "Guest", "Admin", and "SuperAdmin".
  6. **Enabled**: Checkbox to enable or disable the new user account.


## User Interface Behavior
- **Initial View**:
  - Upon loading, the user table displays all existing user records with default sorting (e.g., by ID or username).
  - The new user registration form appears blank, ready for user input.

- **Interaction**:
  - Clicking the "+ New User" button reveals the new user registration form.
  - Users can fill out the form inputs to create a new user account.
  - Toggling the "Hide Disabled User" checkbox updates the visibility of disabled user accounts in the table dynamically.
  - Clicking the sorting arrows on column headers sorts the user table records based on the selected parameter.
  - Clicking the filter icon on column headers allows users to apply filters to the records based on specific criteria.

- **Save User**:
  - Upon filling out the new user registration form and clicking "Save User", the system should validate the inputs and either create a new user or update an existing user account.

## Notes
- Ensure responsive design to accommodate various screen sizes and devices.
- Use consistent styling and color schemes following the application's design guidelines.

---
This document serves as a guide for developing the User Management screen. For any clarifications or additional requirements, please refer to the specifications outlined above.
