# Django LittleLemon API Advanced

## Overview

Django LittleLemon API Advanced is a fully functioning API project designed for the Little Lemon restaurant. This project allows client application developers to leverage various APIs to create web and mobile applications. Users with different roles, such as admin, manager, delivery crew, and customers, have distinct capabilities within the system.

## Capabilities

### Admin Capabilities

- Assign users to the manager group
- Access the manager group with an admin token
- Add menu items
- Add categories

### Manager Capabilities

- Log in
- Update the item of the day
- Assign users to the delivery crew
- Assign orders to the delivery crew

### Delivery Crew Capabilities

- Access orders assigned to them
- Update an order as delivered

### Customer Capabilities

- Register
- Log in using username and password to obtain access tokens
- Browse all categories
- Browse all menu items
- Browse menu items by category
- Paginate menu items
- Sort menu items by price
- Add menu items to the cart
- Access previously added items in the cart
- Place orders
- Browse their own orders

## API Endpoints

### User Registration and Token Generation Endpoints

- `/api/users`
- `/api/users/users/me/`
- `/token/login/`

### Menu Item Endpoints

- `/api/menu-items`
- `/api/menu-items/{menuItem}`
- `/api/menu-items/{menuItem}`

### User Group Management Endpoints

- `/api/groups/manager/users`
- `/api/groups/manager/users/{userId}`
- `/api/groups/delivery-crew/users`
- `/api/groups/delivery-crew/users/{userId}`

### Cart Management Endpoints

- `/api/cart/menu-items`

### Order Management Endpoints

- `/api/orders`
- `/api/orders/{orderId}`

## Usage

To make use of these endpoints, developers need to obtain access tokens by registering and logging in through the appropriate user registration and token generation endpoints. With the obtained tokens, users can authenticate themselves and access various functionalities based on their roles.

## Examples

Here are some examples of how to interact with the API:

- To register a new user: `POST /api/users`
- To log in and obtain an access token: `POST /token/login/`
- To browse all menu items: `GET /api/menu-items`
- To place an order: `POST /api/orders`

## Project Structure

The project is structured with clear endpoints and functionalities for each user role. Developers can refer to the provided capabilities and API endpoints to integrate these features into their applications seamlessly.

For detailed information on each endpoint, including request and response structures, developers can refer to the API documentation.

## Dependencies

This project relies on the Django framework and Django Rest Framework for creating robust and scalable APIs. Ensure you have the required dependencies installed before using the API.

## Contributing

If you find any issues or have suggestions for improvement, please feel free to contribute by submitting a pull request or creating an issue in the repository.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute it according to the terms of the license.

