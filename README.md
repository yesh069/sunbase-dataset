# Sunbase Java Development internship Assignment


## Table of Contents

1. [Features](#features)
2. [Getting Started](#getting-started)
3. [Usage](#usage)
4. [Functionality](#functionality)

## Features

- **User Authentication**: Users can log in with their username and password through the Sunbase API.

- **Customer List Display**: After logging in, users can view a list of customers with various details.

- **Add New Customer**: Users can add new customers by providing the required information.

- **Edit Customer Information**: Users can edit existing customer information directly from the customer list.

- **Delete Customer**: Users can delete a customer from the list.

## Getting Started

To get started with the application, follow these steps:

1. Clone the repository: `git clone <repository-url>`
2. Open the `index.html` file in a web browser.

## Usage

1. Open the application in a web browser.
2. Log in with your Sunbase credentials.
3. Navigate through the customer list, add new customers, edit existing customer information, or delete customers as needed.

## Functionality

### `login()`

- Authenticates the user by sending a POST request to the Sunbase API with the provided username and password.
- On successful authentication, stores the access token and displays the customer list and add customer screens.

### `addCustomer()`

- Adds a new customer by sending a POST request to the Sunbase API with the provided customer information.
- Checks for mandatory parameters (first name and last name) before making the API call.

### `getCustomerList()`

- Fetches the list of customers from the Sunbase API using a GET request.
- Populates the customer table with the retrieved customer data.

### `deleteCustomer(uuid)`

- Deletes a customer by sending a POST request to the Sunbase API with the customer's UUID.
- Displays a success or failure message based on the API response.

### `makeRowEditable(row)`

- Makes a table row editable by replacing text content with input fields.
- Hides the "Edit" button and adds a "Save" button for updating the row data.

### `saveRowData(row)`

- Saves the edited row data by sending a POST request to the Sunbase API with the updated customer information.
- Refreshes the customer list after a successful update.

