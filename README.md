# 📦 MongoDB Data Modeling – Project S2_03

This repository contains three structured MongoDB database models designed for different real-world applications. Each model follows a **non-embedded, reference-based architecture**, ensuring scalability, clarity, and professional standards.

---

## 📁 Level 1 – Òptica Cul d’Ampolla

A modular database for an optical store, modeling suppliers, glasses, customers, employees, and sales.

| Collection   | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `Suppliers`  | Provider details including address, NIF, and contact                        |
| `Glasses`    | Technical specs, pricing, and supplier reference                            |
| `Customers`  | Personal info and optional referral link                                    |
| `Employees`  | Staff roles and contact info                                                |
| `Sales`      | Transaction records linking glasses, customer, and employee                 |

**Highlights:**
- Clear separation of entities
- Referential integrity via `ObjectId`
- Designed for professional presentation and academic review

---

## 📁 Level 2 – TakeAway Food Ordering System

A delivery-focused food ordering system for a fictional restaurant.

| Collection     | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `Clients`      | Delivery address and contact info                                           |
| `Stores`       | Store location and province                                                 |
| `Employees`    | Role-based staff linked to stores                                           |
| `Products`     | Pizzas, burgers, drinks with optional categories                            |
| `Orders`       | One-to-many relationship with clients and stores                            |
| `OrderItems`   | Quantity and product breakdown per order                                    |
| `Deliveries`   | Delivery person and timestamp for home orders                               |

**Highlights:**
- Fully normalized structure
- Delivery logic separated from order metadata
- Supports both pickup and home delivery workflows

---

## 📁 Level 3 – YouTube Simplified Platform

A reduced model of a video-sharing platform inspired by YouTube.

| Collection         | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `Users`            | Account credentials and demographics                                        |
| `Channels`         | Created by users with metadata                                              |
| `Videos`           | Technical details, status, and publishing info                              |
| `Tags`             | Linked to videos individually                                               |
| `Subscriptions`    | User-to-channel relationships                                               |
| `VideoReactions`   | Likes/dislikes with timestamps                                              |
| `Playlists`        | User-curated lists with visibility status                                   |
| `PlaylistItems`    | Video-to-playlist mapping                                                   |
| `Comments`         | Text and timestamp linked to videos and users                               |

**Highlights:**
- No embedded arrays; all relationships are external
- Supports user interaction tracking and playlist management
- Designed for UI-driven applications and scalable querying

---

## 🛠️ Technologies Used

- MongoDB (non-embedded modeling)
- JSON Schema (structure and validation)
- Git for version control
- Todiagram for visual modeling

---

## 📚 Author

**Carlos Cozar**  
Backend Developer | Java, Spring Boot, MongoDB  
GitHub: [carlosPc1987](https://github.com/carlosPc1987)
