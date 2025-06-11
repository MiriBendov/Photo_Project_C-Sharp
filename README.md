# Photo_ssem

Photo_ssem is a system for managing orders, customers, and images, with an emphasis on load balancing between officers and automatic assignment of orders.

## Features

- **Customer Management**: Add new customers to the database.
- **Order Management**: Create new orders and assign each order to the officer with the least workload.
- **Officer Management**: Check if an officer exists by code, view all orders for a specific officer.
- **Image Management**: Read, save, and upload images from files to the system and database.
- **Email Sending**: Send order confirmation emails to customers.
- **Database Integration**: All operations are performed using Entity Framework Core.

## Code Structure

- **insertToDB** - Adds a new customer and order, including officer assignment.
- **ReadFromDB** - Returns the officer code with the fewest orders.
- **ReadFromDBCode** - Checks if an officer exists by code.
- **ReadFromDBAllOrder** - Returns all orders for a specific officer.
- **ReadImage** - Reads an image from a file.
- **newSavaimg** - Saves an image to the database by order.
- **SendPurchaseConfirmationEmail** - Sends a confirmation email to the customer.

## Requirements

- .NET 8.0 or higher
- Entity Framework Core
- Compatible database (e.g., SQL Server)

## Installation & Running

1. Clone the project to your local machine.
2.Open `Photo_ssem.sln` in Visual Studio.
3. Configure the database connection in `appsettings.json`.
4. Build the solution.
5. Run the main project.

## Authors

miri ben-dov
