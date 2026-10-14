# Martfury Shop: Electronics E-commerce Website

A full-stack online store for electronics, with a customer storefront, an admin panel and a REST API backend. Team project (Group 7) for the Introduction to Software Engineering course at PTIT.

## Repository layout

The project is split across three branches:

| Branch | Contents |
|---|---|
| `main` | Backend: Spring Boot REST API (`MartfuryShop/`) |
| [`user`](../../tree/user) | Customer storefront (Angular) |
| [`admin`](../../tree/admin) | Admin panel (Angular) |

## Features

**Customers**
- Sign up, sign in (JWT) and reset a forgotten password by email
- Browse products by category, search, and view product details
- Cart, checkout and order history
- Favorites list and product ratings
- Real-time notifications over WebSocket

**Admins**
- Manage products, categories and customers
- Process orders and update their status
- Inventory overview and moderation of product ratings
- Sales statistics, revenue by category and best-selling products

## Tech stack

| Part | Tools |
|---|---|
| Backend | Java 8, Spring Boot 2.6, Spring Data JPA, Spring Security with JWT, WebSocket, JavaMail, Thymeleaf (email and reset-password pages) |
| Database | MySQL |
| Frontend | Angular 12, TypeScript |

## Backend structure

```
MartfuryShop/src/main/java/vn/fs/
├── api/          # REST endpoints: products, categories, cart, orders, ratings, favorites, statistics, users
├── config/       # Spring Security, JWT filter, WebSocket
├── entity/       # JPA entities
├── repository/   # Spring Data repositories
├── service/      # Mail and user-details services
├── dto/          # Request and response objects
└── handler/      # WebSocket notification handler
```

## Running locally

**Backend**

1. Create a MySQL database named `martfury_shop`.
2. Set the following environment variables:

   | Variable | Purpose |
   |---|---|
   | `DB_PASSWORD` | MySQL password for the `root` user |
   | `MAIL_PASSWORD` | Gmail app password used to send emails |
   | `JWT_SECRET` | Secret key for signing JWTs |

3. Start the API:

   ```bash
   cd MartfuryShop
   ./mvnw spring-boot:run
   ```

   Tables are created automatically on first run (`spring.jpa.hibernate.ddl-auto=update`).

**Frontend**

```bash
git checkout user     # or: git checkout admin
npm install
npx ng serve
```
