
# Ecommerce Platform API Documentation

This repository contains OpenAPI 3.0 specifications for the microservices of the Ecommerce Platform, written in Golang and designed under a microservice architecture.

## 📦 Services Included

Each file corresponds to a separate microservice:

| Microservice       | File Name        | Description                                         |
|--------------------|------------------|-----------------------------------------------------|
| Authentication     | `auth.yaml`      | Handles JWT login, refresh and validation.         |
| Users              | `users.yaml`     | Manages user registration and basic profile data.  |
| Products & Brands  | `products.yaml`  | Lists products and allows filtering by brand.      |
| Cart               | `cart.yaml`      | Manages user shopping cart operations.             |
| Orders             | `orders.yaml`    | Handles order creation and listing.                |
| Payments (Wompi)   | `payments.yaml`  | Processes payments via Wompi.                      |
| Invoices           | `invoices.yaml`  | Generates invoices from paid orders.               |
| Email              | `email.yaml`     | Sends transactional and marketing emails.          |

## 📂 How to Use

You can view these files in any OpenAPI-compatible viewer such as:

- [Swagger Editor](https://editor-next.swagger.io/)
- [ReDocly](https://redocly.github.io/redoc/)

## 🚀 Deployment Notes

- All services are intended to be deployed as independent containers or pods.
- Communication between services can be done using REST.
- JWT is used for authentication across all services (see `bearerAuth` scheme).

## 🧪 Example

To test locally, you can open any `.yaml` file at [Swagger Editor](https://editor.swagger.io/?url=https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/auth.yaml)

## 🛡️ Security

All protected routes require a JWT bearer token as described in the `components.securitySchemes` section of each specification.

---

© 2025 - Ecommerce Microservice Architecture


## 🔗 Open in Swagger Editor

| Microservice       | Swagger Editor Link                                                                                   |
|--------------------|--------------------------------------------------------------------------------------------------------|
| Authentication     | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/auth.yaml)     |
| Users              | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/users.yaml)    |
| Products           | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/products.yaml) |
| Brands             | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/brands.yaml) |
| Cart               | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/cart.yaml)     |
| Orders             | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/orders.yaml)   |
| Payments (Wompi)   | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/payments.yaml) |
| Invoices           | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/invoices.yaml) |
| Email              | [Open in Swagger](https://editor-next.swagger.io/?url=https://raw.githubusercontent.com/JuniorGuerra/open-api-public/refs/heads/dev/email.yaml)     |